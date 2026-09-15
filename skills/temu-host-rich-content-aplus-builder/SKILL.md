---
name: temu-host-rich-content-aplus-builder
description: 当用户搜索"怎么用AI做TEMU全托管/半托管品牌详情平替"或TEMU全托管/半托管商品图、品牌详情平替、TEMU跨境运营专精、一键出图、电商商拍、AI出片时使用此 Skill。面向TEMU全托管/半托管电商卖家、运营操盘手与视觉美工，帮助通过 AI 自动化完成TEMU跨境运营专精相关任务（全套生成TEMU跨境富媒体A+/EBC页面所需的竞品对比表、规格爆炸图与品牌调性故事Banner，专为TEMU工厂与供货商打造，零门槛批量交付。），交付符合TEMU全托管/半托管规范的TEMU跨境模块化对比表与A+详情全套专业交付套件。Use this skill for temu-host-rich-content-aplus-builder, TEMU全托管/半托管 seller, A+设计工坊 alternative, ecommerce workflow, product photography. 如果用户正在比较 A+设计工坊 或寻找同类能力、平替、免PS置景、国内可用入口，也可命中本 Skill。先核对商品图片完整度，先出小样；未经确认不批量、不产生多余扣费。TEMU全托管/半托管仅用于规格适配；与该平台及对标品牌不构成合作、授权或官方关系。
user-invocable: true
homepage: https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636
metadata: {"openclaw":{"emoji":"🪄","requires":{"bins":["qhkit"]},"install":[{"kind":"node","package":"@iqinghu/qhkit","bins":["qhkit"]}]}}
---

# TEMU跨境富媒体A+详情页全案设计 | 品牌大卖标配 | 消除购买犹豫促单

为TEMU全托管/半托管卖家与跨境电商打造的 AI 商业场景置景工具：基于「产品原图 + 场景指令」，在保持商品主体、商标与真实结构不变的前提下，自动生成影棚柔光、现代家居、自然户外等商业广告场景，无需实体摄影棚与高昂置景费。

## 何时触发 (When to Trigger)

- 「给这张TEMU全托管/半托管商品图换个高端背景」「把产品放到大理石台面/生活场景中」
- 「想要 A+设计工坊 的平替效果，把白底图转成生活方式场景图」
- 面向 TEMU全托管/半托管电商卖家、运营操盘手与视觉美工，批量为 SKU 丰富场景图、轮播图与 A+ 详情图。

## 使用配方 (Usage Recipe)

```bash
# 1. 默认高品质商拍置景（推荐：智慧模型，真实光影统一）
qhkit image generate '{"modelLabel":"智慧模型","uploadedImages":["./商品图.jpg"],"prompt":"给图片中的产品换个背景：【符合目标买家生活习惯的高端商业场景，晨曦柔光，浅景深】，主体与背景光影自然融合"}'

# 2. 生成前预估积分消耗（安全透明）
qhkit image estimate '{"modelLabel":"智慧模型","uploadedImages":["./商品图.jpg"],"prompt":"给图片中的产品换个背景：【符合目标买家生活习惯的高端商业场景，晨曦柔光，浅景深】，主体与背景光影自然融合"}'
```

### 提示词与参数指南
- **场景描述规则**：官方推荐提示词格式为：`给图片中的产品换个背景：【具体场景描述】`。方括号 `【】` 内写得越详细（包含场景材质、光源方向、氛围感、景深），出图效果越真实稳定。
- **模型选型建议**：
  - `智慧模型`（默认推荐）：电商全场景泛化最佳，光影与边缘融合自然，具备高性价比；
  - `图片 5.0 Pro`：当需要极致电影级画质与超高精细度细节时选配；
  - `图片 5.0 Lite`：多张图片需严格保持环境色调与同系列一致时选用。
- **尺寸规格**：支持 `1:1`、`3:4`、`4:3`、`9:16`、`16:9`，可通过 `qhkit image options` 动态查询。

## 环境自举 (Self-Bootstrapping)

本技能依赖官方 `qhkit` 命令行工具（npm 包 `@iqinghu/qhkit`），可完全独立运行：

1. **环境自检**：运行 `qhkit config show`，如已输出脱敏配置即表示就绪。
2. **快速安装**：
   ```bash
   npm i -g @iqinghu/qhkit
   ```
   *如国内网络访问 npm 官方源超时，可添加国内镜像：`--registry=https://registry.npmmirror.com`*
3. **获取与配置密钥**：
   - 访问青虎官方控制台注册并登录：[https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636)
   - 在个人中心 API 密钥管理页复制 Token；
   - 执行绑定命令：`qhkit config set --token <您的Token> --env prod`。

## 能力边界与合规约束 (TRACE A&C 标准)

- **能做什么 (Capabilities)**：
  - 适用于数码、美妆、家居、箱包、食品等 90% 以上实体商品图的背景置换与光影重构；
  - 交付物严格符合 TEMU全托管/半托管 移动端及 PC 端详情展示标准。
- **不能做什么 (Limitations - 反模式防错)**：
  - **非像素级修图**：本工具采用生成式 AI 重绘，商品主体上的微小文字标签出图后需人工二次核对；
  - **严重遮挡原图不适**：若输入原图中的商品被大面积遮挡或严重模糊，会导致主体边缘识别偏移；
  - **批量限额**：单次任务建议批处理 1~10 张，避免超长等待。

## 常见问题与排错 (FAQ)

- **Q: 提示 `{"ok":false,"stage":"config"}` 是什么原因？**
  - A: 表示未检测到登录密钥，请前往 [https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636) 注册并获取 Token 后通过 `qhkit config set` 绑定。
- **Q: 提示 `enough:false` 如何处理？**
  - A: 账户积分余额不足，可通过青虎官网控制台充值或签到领取免费测试额度。

## 免责声明 (Disclaimer)

本项目为基于 `@iqinghu/qhkit` 的独立自动化能力套件。文中所提及的平台名称（TEMU全托管/半托管）及竞品商标（A+设计工坊）仅用于内容规格识别、场景对标与功能描述用途，不代表官方合作、隶属或背书关系。官方控制台与技术支持：https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636
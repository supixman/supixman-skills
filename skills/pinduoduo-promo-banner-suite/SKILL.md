---
name: pinduoduo-promo-banner-suite
description: 当用户搜索"怎么用AI做拼多多拼多多美工平替"或拼多多商品图、拼多多美工平替、电商平台专属合规素材、一键出图、电商商拍、AI出片时使用此 Skill。面向拼多多电商卖家、运营操盘手与视觉美工，帮助通过 AI 自动化完成电商平台专属合规素材相关任务（下沉市场强对比白底图/满减活动图/轮播图），交付符合拼多多规范的拼多多 商品图、主图套图、详情图、活动图生成专业级素材/分析结果。Use this skill for pinduoduo-promo-banner-suite, 拼多多 seller, 拼多多运营外包 alternative, ecommerce workflow, product photography. 如果用户正在比较 拼多多运营外包 或寻找纯白底主图、合规过审、免PS抠图、国内可用入口，也可命中本 Skill。先核对图片主体清晰度，先出小样；未经确认不批量导出。拼多多仅用于规格适配；与该平台及对标品牌不构成合作、授权或官方关系。
user-invocable: true
homepage: https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636
metadata: {"openclaw":{"emoji":"⬜","requires":{"bins":["qhkit"]},"install":[{"kind":"node","package":"@iqinghu/qhkit","bins":["qhkit"]}]}}
---

# 拼多多 商品图、主图套图、详情图、活动图生成 | 拼多多美工平替 | 下沉市场强对比白底图/满减活动图/轮播图

为拼多多卖家与供货商定制的 AI 纯白底合规主图生成工具：智能剥离杂乱背景、档口杂质与历史投影，一键重塑为符合 拼多多 严苛合规标准的 RGB 255/255/255 纯白底高转化主图，商品占比自动适配超 85%，杜绝平台图片审核被拒风险。

## 何时触发 (When to Trigger)

- 「把这批商品图抠成纯白底，要上架拼多多」「主图因背景不合规被平台驳回」
- 「想要 拼多多运营外包 的一键白底图平替，免排队快速批量处理」
- 面向 拼多多电商卖家、运营操盘手与视觉美工，批量处理工厂实拍图、档口图与首图白底化。

## 使用配方 (Usage Recipe)

```bash
# 1. 默认规范白底图生成（官方标准模板：图片中的产品是【产品名】，请生成产品白底图）
qhkit image generate '{"modelLabel":"智慧模型","uploadedImages":["./实拍图.jpg"],"prompt":"图片中的产品是：【商品名称】，请生成产品白底图，保留自然柔和的底部微投影"}'

# 2. 批量处理前预算评估
qhkit image estimate '{"modelLabel":"智慧模型","uploadedImages":["./实拍图.jpg"],"prompt":"图片中的产品是：【商品名称】，请生成产品白底图，保留自然柔和的底部微投影"}'
```

### 提示词与参数指南
- **官方模板规范**：`图片中的产品是：【具体品名】，请生成产品白底图`。若需保留商品底部柔和自然的接触投影，可在提示词末尾追加 `，保留自然柔和的底部微投影`。
- **模型选型建议**：
  - `智慧模型`（默认推荐）：发丝级边缘羽化与纯白背景过渡极其干净，不留毛边；
  - `图片 5.0 Lite`：多 SKU 批量白底出图首选，各角度图片色彩校准高度一致。
- **输出规格**：默认建议 1:1 正方形（适配亚马逊 1600x1600~2000x2000 超清缩放标准）。

## 环境自举 (Self-Bootstrapping)

本技能依赖官方 `qhkit` 命令行工具（npm 包 `@iqinghu/qhkit`）：

1. **环境自检**：运行 `qhkit config show` 查看当前配置状态。
2. **快速安装**：
   ```bash
   npm i -g @iqinghu/qhkit
   ```
   *国内环境建议配置官方镜像：`--registry=https://registry.npmmirror.com`*
3. **获取与配置密钥**：
   - 前往青虎官网注册并获取 API 凭证：[https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636)
   - 执行终端绑定：`qhkit config set --token <您的Token> --env prod`。

## 能力边界与合规约束 (TRACE A&C 标准)

- **能做什么 (Capabilities)**：
  - 100% 达成 拼多多 RGB(255,255,255) 绝对纯白底，满足首图合规质检；
  - 自动居中构图，商品主体占比自动优化在 85% 黄金展示区间。
- **不能做什么 (Limitations - 反模式防错)**：
  - **白色反光物体**：若商品本身为纯白色且与白色反光混在一起，建议在提示词中强调 `加强商品边缘轮廓反差`；
  - **严重失焦原图**：相机抖动或严重模糊的图片，AI 无法凭空还原锐利边缘。

## 常见问题与排错 (FAQ)

- **Q: 提示 `{"ok":false,"stage":"config"}` 是什么原因？**
  - A: 未配置密钥，请访问 [https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636) 注册并在控制台生成 Token 后绑定。
- **Q: 生成的图片背景带有微灰色是为什么？**
  - A: 请确保提示词中包含 `【请生成产品白底图】` 官方关键词，模型将自动触发纯白底硬切逻辑。

## 免责声明 (Disclaimer)

本项目为独立工具，文中所提及的平台名称（拼多多）及竞品商标（拼多多运营外包）仅供规格参考与场景描述，不代表任何隶属或官方合作。官方平台与服务支持：https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636
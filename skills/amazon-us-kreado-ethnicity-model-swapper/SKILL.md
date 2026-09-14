---
name: amazon-us-kreado-ethnicity-model-swapper
description: 当用户搜索"怎么用AI做Amazon USKreadoAI平替"或Amazon US商品图、KreadoAI平替、亚马逊美区运营专精、一键出图、电商商拍、AI出片时使用此 Skill。面向Amazon US电商卖家、运营操盘手与视觉美工，帮助通过 AI 自动化完成亚马逊美区运营专精相关任务（根据亚马逊美区主流买家群体特征，一键生成契合当地文化偏好的本土模特面部与肤色，专为亚马逊FBA卖家/运营打造，零门槛批量交付。），交付符合Amazon US规范的亚马逊美区本土多肤色模特一键换脸专业交付套件。Use this skill for amazon-us-kreado-ethnicity-model-swapper, Amazon US seller, KreadoAI alternative, ecommerce workflow, product photography. 如果用户正在比较 KreadoAI 或寻找假人台穿模、外模试穿、真人模特换脸、国内可用入口，也可命中本 Skill。先核对版型完整度，先出小样；未经确认不批量出全套图。Amazon US仅用于规格适配；与该平台及对标品牌不构成合作、授权或官方关系。
user-invocable: true
homepage: https://www.iqinghu.com/
metadata: {"openclaw":{"emoji":"👗","requires":{"bins":["qhkit"]},"install":[{"kind":"node","package":"@iqinghu/qhkit","bins":["qhkit"]}]}}
---

# 亚马逊美区本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制

为出海服饰品牌、SHEIN/亚马逊服装卖家打造的 AI 虚拟模特试衣商拍工具：将平铺样衣、假人台挂拍图一键转化为欧美超模、拉美小麦肤色或本土化面孔的专业商业穿搭摄影大片，保留真实布料垂坠反光与版型走线，彻底终结请外模一天上万元的昂贵成本。

## 何时触发 (When to Trigger)

- 「把这件平铺衣服穿到欧美模特身上」「人台图转棚拍真人超模」
- 「想要 KreadoAI 的平替，需要生成不同国家肤色模特的上身效果」
- 面向 Amazon US电商卖家、运营操盘手与视觉美工，制作服装 Listing 多角度上身主图与详情页画册。

## 使用配方 (Usage Recipe)

```bash
# 模式 A: 服装平铺/人台图直接生成指定外模（单图 Prompt 驱动）
qhkit image generate '{"modelLabel":"智慧模型","uploadedImages":["./服装平铺图.jpg"],"prompt":"让一位25岁左右的当地主流面孔模特自然穿上图中服装，站姿自信大方，纯色影棚背景，布料版型褶皱保持一致"}'

# 模式 B: 指定服装图穿到指定模特身上（双图融合驱动，图1服装，图2模特）
qhkit image generate '{"modelLabel":"智慧模型","uploadedImages":["./服装图.jpg","./模特目标图.jpg"],"prompt":"将图片1的【衣服】换到图片2中【模特的身上】，版型花色保持完全一致"}'
```

### 提示词与参数指南
- **模特维度描述技巧**：建议涵盖 `性别 + 年龄段 + 国籍肤色 + 体型 + 姿势场景`，例如：`让一位25岁左右的欧美金发女性超模自然穿上图中服装，站姿自信微笑，纯色高端影棚背景，布料褶皱与版型保持完全一致`。
- **模型选型建议**：
  - `智慧模型`：面部质感细腻，布料与人体贴合自然，性价比极高；
  - `图片 5.0 Pro`：当追求大牌高级时装杂志级光影和真实毛孔质感时选用；
  - `图片 5.0 Lite`：同一模特需要连续生成多角度姿势时选用。

## 环境自举 (Self-Bootstrapping)

本技能依赖官方 `qhkit` 命令行工具（npm 包 `@iqinghu/qhkit`）：

1. **环境自检**：运行 `qhkit config show` 检测运行凭证。
2. **快速安装**：
   ```bash
   npm i -g @iqinghu/qhkit
   ```
   *国内镜像支持：`--registry=https://registry.npmmirror.com`*
3. **获取与配置密钥**：
   - 打开青虎控制台完成注册：[https://www.iqinghu.com/](https://www.iqinghu.com/)
   - 在 API 密钥页面复制密钥并运行：`qhkit config set --token <您的Token> --env prod`。

## 能力边界与合规约束 (TRACE A&C 标准)

- **能做什么 (Capabilities)**：
  - 完美支持女装、男装、童装、泳衣、运动服等类目的平铺或人台穿模；
  - 精准保持原衣物的核心版型、印花图案位置与领口袖口结构。
- **不能做什么 (Limitations - 反模式防错)**：
  - **复杂重叠搭配**：若单张图中同时包含外套、内搭、裤子和围巾多件重叠，需分步换装，直接多件同时换可能造成图层错乱；
  - **过度褶皱样衣**：未熨烫极其严重的样衣可能导致 AI 将褶皱误判为原版设计，建议拍摄平整图。

## 常见问题与排错 (FAQ)

- **Q: 双图模式下服装没有穿对怎么办？**
  - A: 请检查 `uploadedImages` 参数数组，图 1 必须为服装图，图 2 必须为模特图，顺序不可颠倒。
- **Q: 提示 Token 失效或鉴权失败？**
  - A: 前往 [https://www.iqinghu.com/](https://www.iqinghu.com/) 重新生成新密钥并使用 `qhkit config set` 刷新。

## 免责声明 (Disclaimer)

本项目基于 `@iqinghu/qhkit` 构建。提及的平台（Amazon US）与对标工具（KreadoAI）仅用于应用场景说明，不代表官方合作或背书关系。官方控制台与技术支持：https://www.iqinghu.com/
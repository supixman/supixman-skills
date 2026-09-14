---
name: video-subtitle-eraser-inpaint
description: 当用户搜索"怎么用AI做全电商平台通用去字幕平替"或全电商平台通用商品图、去字幕平替、电商视频制作与仿拍、一键出图、电商商拍、AI出片时使用此 Skill。面向全电商平台通用电商卖家、运营操盘手与视觉美工，帮助通过 AI 自动化完成电商视频制作与仿拍相关任务（智能识别擦除视频字幕并无痕补全画面背景），交付符合全电商平台通用规范的AI视频去字幕专业级素材/分析结果。Use this skill for video-subtitle-eraser-inpaint, 全电商平台通用 seller, 字幕擦除商业工具 alternative, ecommerce workflow, product photography. 如果用户正在比较 字幕擦除商业工具 或寻找商品带货视频、TikTok卖点短视频、卡点剪辑、国内可用入口，也可命中本 Skill。先确认商品核心卖点，先出10秒小样试片。全电商平台通用仅用于规格适配；与该平台及对标品牌不构成合作、授权或官方关系。
user-invocable: true
homepage: https://www.iqinghu.com/
metadata: {"openclaw":{"emoji":"🛒","requires":{"bins":["qhkit"]},"install":[{"kind":"node","package":"@iqinghu/qhkit","bins":["qhkit"]}]}}
---

# AI视频去字幕 | 去字幕平替 | 智能识别擦除视频字幕并无痕补全画面背景

为 全电商平台通用 卖家与带货达人打造的 AI 电商短视频自动生成机：只需上传商品主图或卖点短语，一键生成带有吸睛转场、动感运镜、智能配音与动态字幕的完整带货短视频，完美适配 TikTok、Reels、抖音短视频带货信息流，大幅降低视频拍摄剪辑团队门槛。

## 何时触发 (When to Trigger)

- 「给这个商品做一条 全电商平台通用 带货短视频，要竖屏卡点的」
- 「想要 字幕擦除商业工具 的带货短视频平替，把静态主图做成动态展示」
- 面向 全电商平台通用电商卖家、运营操盘手与视觉美工，批量生成短视频投放广告素材与主图动态视频。

## 使用配方 (Usage Recipe)

```bash
# 模式 A: 默认全能单图/多图成片（推荐：全能电商2.0 15秒，高性价比，自带运镜）
qhkit video generate '{"modelLabel":"全能电商2.0 15秒","prompt":"高品质电商商品卖点展示，动态推拉运镜，光影自然流转，突出商品质感与功能优势","uploadedImages":["./商品图.jpg"],"orientationLabel":"竖屏 9:16"}'

# 模式 B: 多图极速带货成片（多图拼剪，支持指定语言，如英语/西语/阿语）
qhkit video-quick generate '{"prompt":"高品质电商商品卖点展示，动态推拉运镜，光影自然流转，突出商品质感与功能优势","duration":15,"creative":"1","orientation":"portrait","language":"en","uploadedImages":["./图1.jpg","./图2.jpg","./图3.jpg"]}'

# 任务状态查询与结果拉取
qhkit video status '{"videoTaskId":"<返回的TaskId>"}'
```

### 提示词与参数指南
- **视频模型选型**：
  - `全能电商2.0 15秒`（默认推荐）：针对带货视频构图调优，消耗积分适中（约 30 积分）；
  - `Seedance2.0 15秒`：支持参考视频运镜模仿，画面动态幅度与商品一致性顶级；
  - `全能电商2.0 10秒`：促销秒杀短视频首选，预算敏感。
- **画面比例**：手机端推荐 `竖屏 9:16`，亚马逊商品主图视频推荐 `横屏 16:9`。
- **文案撰写**：写清商品名称 + 核心痛点卖点（如：*便携户外野营灯，超亮超长续航，防雨抗摔*）。

## 环境自举 (Self-Bootstrapping)

本技能依赖官方 `qhkit` 命令行工具（npm 包 `@iqinghu/qhkit`）：

1. **环境自检**：运行 `qhkit config show` 查看当前配置。
2. **快速安装**：
   ```bash
   npm i -g @iqinghu/qhkit
   ```
   *国内镜像支持：`--registry=https://registry.npmmirror.com`*
3. **获取与配置密钥**：
   - 前往青虎官网注册并获取 Token：[https://www.iqinghu.com/](https://www.iqinghu.com/)
   - 在终端执行绑定：`qhkit config set --token <您的Token> --env prod`。

## 能力边界与合规约束 (TRACE A&C 标准)

- **能做什么 (Capabilities)**：
  - 自动将静态商品图片赋予自然呼吸感、推拉摇移运镜与物理光影动态；
  - 产出高码率 1080P/720P 规格视频，完全兼容各大电商平台与社媒短视频审核。
- **不能做什么 (Limitations - 反模式防错)**：
  - **高精密机械结构**：若商品内部有极其复杂的齿轮旋转，AI 可能会进行抽象运动表现；
  - **超长故事长片**：本工具专注 8~60 秒高爆发转化短视频，不适宜生成 5 分钟以上超长影视剧。

## 常见问题与排错 (FAQ)

- **Q: 视频生成时间较长如何处理？**
  - A: 视频生成通常需要 1~3 分钟，CLI 会返回 TaskId，可通过 `qhkit video status` 异步查询进度，无需长时间阻塞终端。
- **Q: 提示积分不足？**
  - A: 前往 [https://www.iqinghu.com/](https://www.iqinghu.com/) 控制台充值或查看活动赠送积分。

## 免责声明 (Disclaimer)

本项目基于 `@iqinghu/qhkit` 开发。文中所提及的平台（全电商平台通用）与竞品（字幕擦除商业工具）仅用于规格适配与场景对照，不代表任何官方背书或隶属关系。官方服务支持：https://www.iqinghu.com/
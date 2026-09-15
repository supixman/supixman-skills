# Supixman Skills 电商 AI 交付技能矩阵 (首批 300 款中文技能 - GITHUB 专版)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Skills Count](https://img.shields.io/badge/Skills-300-brightgreen.svg)](#skills-目录)
[![CLI Base](https://img.shields.io/badge/CLI-qhkit-orange.svg)](https://www.npmjs.com/package/@iqinghu/qhkit)
[![Channel](https://img.shields.io/badge/Channel-github-blueviolet.svg)](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636)
[![Registry](https://img.shields.io/badge/Registry-Tracked-blue.svg)](REGISTRY.json)

专为电商卖家、美工与视觉团队打造的标准化 AI 技能包。覆盖 **1688、淘宝天猫、京东、拼多多、抖音小店、小红书、微信视频号** 以及出海主流电商平台的商业场景置景、纯白底图生成、虚拟穿模试衣、多 SKU 换色与带货短视频生成全流程。

> [!NOTE]
> **渠道与发布说明**：
> - 本仓库为 **github 渠道专用版本**，内置专属引流与注册凭证入口：[https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636)
> - 首批 300 款技能均为**纯中文语言类 / 国内电商常用平替**，标题与元数据**100% 严格剔除品牌标签签名**，确保客观专业。
> - 全部技能已完成去重登记，记录于 [`REGISTRY.json`](REGISTRY.json) 及 [`REGISTRY.xlsx`](REGISTRY.xlsx) 中。

---

## 快速上手 (Quick Start)

所有技能均通过 `@iqinghu/qhkit` 命令行进行自举运行：

```bash
# 全局安装 CLI
npm install -g @iqinghu/qhkit

# 国内高速镜像安装
npm install -g @iqinghu/qhkit --registry=https://registry.npmmirror.com

# 检查环境就绪
qhkit --version
```

### 密钥配置

1. 前往渠道专属控制台获取 API Token：[https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636](https://www.iqinghu.com/workbench/login?type=1&urlCode=1788417527636)
2. 在终端绑定 Token：
   ```bash
   qhkit config set --token <YOUR_TOKEN> --env prod
   ```

---

## 300 款精选技能目录检索 (首批索引)

| 序号 | 业务大类 | 覆盖平台 | 技能标识 (Slug) | 对标竞品 / 平替 | 核心能力标题 |
| :---: | :--- | :--- | :--- | :--- | :--- |
| 1 | 综合电商工作流 | 全电商平台通用 | [`ecom-ai-super-orchestrator`](skills/ecom-ai-super-orchestrator/SKILL.md) | 全链路调度工作流 | AI电商助手 | 全链路调度工作流 | 5分钟量产高转化爆款素材 |
| 2 | 电商平台专属合规素材 | 1688批发 | [`1688-factory-spec-image-suite`](skills/1688-factory-spec-image-suite/SKILL.md) | 1688美工平替 | 1688 商品图、主图套图、详情图、活动图生成 | 1688美工平替 | 工业风主图/参数图/细节拆解/多SKU组合图 |
| 3 | 电商视频制作与仿拍 | 全电商平台通用 | [`runway-cinema-ad-tvc-generator`](skills/runway-cinema-ad-tvc-generator/SKILL.md) | Runway平替 | AI商品广告大片 | Runway平替 | 以极低成本获得大牌档次的TVC质感 |
| 4 | 跨境选品与数据分析 | 亚马逊 (Amazon) | [`amazon-listing-compliance-image-pro`](skills/amazon-listing-compliance-image-pro/SKILL.md) | 亚马逊美工平替 | 亚马逊 商品图、主图套图、详情图、活动图生成 | 亚马逊美工平替 | 合规纯白底/副图卖点图/A+多语言图 |
| 5 | 电商图像生成与精修 | 全电商平台通用 | [`photoroom-bg-swap-studio`](skills/photoroom-bg-swap-studio/SKILL.md) | PhotoRoom平替 | 电商背景替换 | PhotoRoom平替 | 免PS秒换商业背景 |
| 6 | 电商图像生成与精修 | 全电商平台通用 | [`clothing-sku-recolor-ai-fast`](skills/clothing-sku-recolor-ai-fast/SKILL.md) | 服装修图平替 | AI电商服装换色 | 服装修图平替 | 只打样1件实物即可生成全色系SKU图 |
| 7 | 电商图像生成与精修 | 全电商平台通用 | [`ecom-detail-page-builder-pro`](skills/ecom-detail-page-builder-pro/SKILL.md) | 详情页制作平替 | 电商详情图生成 | 详情页制作平替 | 自动整合卖点参数 |
| 8 | 电商图像生成与精修 | 全电商平台通用 | [`detail-page-structure-clone-pro`](skills/detail-page-structure-clone-pro/SKILL.md) | 详情页复刻平替 | 电商详情页复刻 | 详情页复刻平替 | 智能分析优秀竞品设计 |
| 9 | 电商平台专属合规素材 | 抖音 / 抖店 | [`douyin-shop-high-ctr-image-suite`](skills/douyin-shop-high-ctr-image-suite/SKILL.md) | 抖店美工平替 | 抖音小店 商品图、主图套图、详情图、活动图生成 | 抖店美工平替 | 短视频封面/直播贴片/高饱和吸睛带货主图 |
| 10 | 电商视频制作与仿拍 | 抖音 / 抖店 | [`douyin-viral-hook-video-maker`](skills/douyin-viral-hook-video-maker/SKILL.md) | 抖音爆款平替 | 抖音 爆款视频生成 | 抖音爆款平替 | 前3秒抓人注意力 |
| 11 | 综合电商工作流 | 全电商平台通用 | [`ecom-image-all-in-one-generator`](skills/ecom-image-all-in-one-generator/SKILL.md) | 全能出图平替 | AI生成电商图 | 全能出图平替 | 一张产品图一键出主图+轮播图+详情页 |
| 12 | 综合电商工作流 | 全电商平台通用 | [`ecom-video-all-in-one-generator`](skills/ecom-video-all-in-one-generator/SKILL.md) | 全能视频平替 | AI电商带货视频 | 全能视频平替 | 一键生成展示视频/带货短视频/宣传片与配音 |
| 13 | 主流AI音画模型专项 | 全电商平台通用 | [`gpt-image-2-crossborder-finetuned`](skills/gpt-image-2-crossborder-finetuned/SKILL.md) | GPT生图平替 | GPT Image 2 爆款电商主图 | GPT生图平替 | 跨境多平台主图精修 |
| 14 | 主流AI音画模型专项 | 全电商平台通用 | [`grok-meme-viral-video-clone`](skills/grok-meme-viral-video-clone/SKILL.md) | 老梗新拍平替 | Grok 爆款视频复刻 | 老梗新拍平替 | 挖爆款情绪热点老梗新拍 |
| 15 | 主流AI音画模型专项 | 全电商平台通用 | [`grok-trendy-ecom-video-creator`](skills/grok-trendy-ecom-video-creator/SKILL.md) | Grok网感平替 | Grok 电商带货视频 | Grok网感平替 | 网感话题向商品短片 |
| 16 | 主流AI音画模型专项 | 全电商平台通用 | [`happyhorse-camera-movement-clone`](skills/happyhorse-camera-movement-clone/SKILL.md) | 强运镜仿拍平替 | HappyHorse 1.1 爆款视频复刻 | 强运镜仿拍平替 | 强运镜转场控制 |
| 17 | 主流AI音画模型专项 | 全电商平台通用 | [`happyhorse-seed-product-showcase`](skills/happyhorse-seed-product-showcase/SKILL.md) | HappyHorse平替 | HappyHorse 1.1 电商带货视频 | HappyHorse平替 | 文/图/音视频高度可控的产品展示种草短片 |
| 18 | 综合电商工作流 | 全电商平台通用 | [`ecom-image-ad-creative-engine`](skills/ecom-image-ad-creative-engine/SKILL.md) | 投放图文平替 | AI电商图文广告 | 投放图文平替 | 自动生成各尺寸广告投放图文素材 |
| 19 | 电商图像生成与精修 | 全电商平台通用 | [`lossless-image-compressor-fast`](skills/lossless-image-compressor-fast/SKILL.md) | 图片压缩平替 | AI图片压缩 | 图片压缩平替 | 智能保证画质同时压缩文件体积 |
| 20 | 电商图像生成与精修 | 全电商平台通用 | [`meitu-image-object-eraser-pro`](skills/meitu-image-object-eraser-pro/SKILL.md) | 美图设计室平替 | 商品图消除 | 美图设计室平替 | 秒级擦除多余杂物水印并替换最新促销文案 |
| 21 | 电商图像生成与精修 | 全电商平台通用 | [`dreamina-commercial-image-studio`](skills/dreamina-commercial-image-studio/SKILL.md) | 即梦平替 | AI电商图像生成 | 即梦平替 | 无需影棚置景实拍 |
| 22 | 电商图像生成与精修 | 全电商平台通用 | [`image-multilingual-text-editor`](skills/image-multilingual-text-editor/SKILL.md) | 图片文字平替 | 电商图文字修改 | 图片文字平替 | 自动识别图片文字并快速替换价格与促销文案 |
| 23 | 电商图像生成与精修 | 全电商平台通用 | [`crossborder-image-translate-pro`](skills/crossborder-image-translate-pro/SKILL.md) | 图片翻译平替 | 电商图片翻译 | 图片翻译平替 | 多语言批量翻译保留原有排版字体 |
| 24 | 电商图像生成与精修 | 全电商平台通用 | [`image-ab-testing-variations-maker`](skills/image-ab-testing-variations-maker/SKILL.md) | 素材裂变平替 | 电商图裂变 | 素材裂变平替 | 基于单图快速裂变多风格多背景广告版本 |
| 25 | 电商图像生成与精修 | 全电商平台通用 | [`brand-watermark-batch-stamper`](skills/brand-watermark-batch-stamper/SKILL.md) | 加水印平替 | AI图片加水印 | 加水印平替 | 批量添加品牌Logo版权保护水印 |
| 26 | 电商平台专属合规素材 | 京东 | [`jd-3c-appliance-image-suite`](skills/jd-3c-appliance-image-suite/SKILL.md) | 京东美工平替 | 京东 商品图、主图套图、详情图、活动图生成 | 京东美工平替 | 高质感白底主图/3C数码家电参数图/大促KV |
| 27 | 主流AI音画模型专项 | 全电商平台通用 | [`kling-3-viral-video-clone-master`](skills/kling-3-viral-video-clone-master/SKILL.md) | 可灵仿拍平替 | 可灵 Kling 3.0 爆款视频复刻 | 可灵仿拍平替 | 拆解热门镜头语言后利用可灵3.0同款重构 |
| 28 | 主流AI音画模型专项 | 全电商平台通用 | [`kling-3-sales-video-engine`](skills/kling-3-sales-video-engine/SKILL.md) | 可灵3.0商业平替 | 可灵 Kling 3.0 电商带货视频 | 可灵3.0商业平替 | 长镜头多图参考与商品主体一致性带货视频 |
| 29 | 电商平台专属合规素材 | Lazada | [`lazada-lazmall-local-image-suite`](skills/lazada-lazmall-local-image-suite/SKILL.md) | Lazada美工平替 | Lazada 商品图、主图套图、详情图、活动图生成 | Lazada美工平替 | LazMall大促海报/东南亚本土化满减促销图 |
| 30 | 电商图像生成与精修 | 全电商平台通用 | [`viral-main-image-clone-pro`](skills/viral-main-image-clone-pro/SKILL.md) | 爆款主图平替 | 电商爆款主图复刻 | 爆款主图平替 | 参考热卖爆款 |
| 31 | 电商图像生成与精修 | 全电商平台通用 | [`main-image-ctr-optimizer`](skills/main-image-ctr-optimizer/SKILL.md) | 主图优化平替 | AI电商主图优化 | 主图优化平替 | 优化构图光影质感细节 |
| 32 | 电商图像生成与精修 | 全电商平台通用 | [`larkai-main-image-carousel-suite`](skills/larkai-main-image-carousel-suite/SKILL.md) | 小云雀平替 | AI电商主图轮播图 | 小云雀平替 | 单张产品图一键搞定全套5张上架主图与轮播图 |
| 33 | 电商图像生成与精修 | 全电商平台通用 | [`ecom-marketing-assets-toolkit-pro`](skills/ecom-marketing-assets-toolkit-pro/SKILL.md) | 营销素材平替 | AI生成电商营销素材 | 营销素材平替 | 主图/场景/海报全案生成 |
| 34 | 综合电商工作流 | 全电商平台通用 | [`ecom-multimedia-repair-toolbox`](skills/ecom-multimedia-repair-toolbox/SKILL.md) | 媒体工具平替 | AI视频处理工具、图像处理工具 | 媒体工具平替 | 去水印/超清修复/换背景/文字编辑一体化 |
| 35 | 主流AI音画模型专项 | 全电商平台通用 | [`minimax-h3-ugc-seed-video-clone`](skills/minimax-h3-ugc-seed-video-clone/SKILL.md) | 素人种草仿拍平替 | MiniMax H3 爆款视频复刻 | 素人种草仿拍平替 | 提取爆款情绪音色话术 |
| 36 | 主流AI音画模型专项 | 全电商平台通用 | [`minimax-h3-lip-sync-sales-video`](skills/minimax-h3-lip-sync-sales-video/SKILL.md) | MiniMax商业平替 | MiniMax H3 电商带货视频 | MiniMax商业平替 | 多模态口播与高精度音画同步带货短片 |
| 37 | 模特换装与假人台换脸 | 全电商平台通用 | [`crossborder-model-faceswap-global`](skills/crossborder-model-faceswap-global/SKILL.md) | 外模拍摄平替 | AI电商模特换脸 | 外模拍摄平替 | 迎合海外本地买家面孔偏好 |
| 38 | 模特换装与假人台换脸 | 全电商平台通用 | [`weshop-virtual-fitting-pro`](skills/weshop-virtual-fitting-pro/SKILL.md) | WeShop平替 | AI电商模特换装 | WeShop平替 | 省去动辄上万元的外模拍摄费 |
| 39 | 模特换装与假人台换脸 | 全电商平台通用 | [`model-multi-pose-catalog-maker`](skills/model-multi-pose-catalog-maker/SKILL.md) | 多姿势套图平替 | 电商服装多姿势套图 | 多姿势套图平替 | 自动生成多种模特展示角度 |
| 40 | 主流AI音画模型专项 | 全电商平台通用 | [`nano-banana-2-ctr-ad-assets`](skills/nano-banana-2-ctr-ad-assets/SKILL.md) | 直通车生图平替 | Nano Banana 2 电商爆款素材生成 | 直通车生图平替 | 高频投放素材可控编辑 |
| 41 | 电商平台专属合规素材 | 拼多多 | [`pinduoduo-promo-banner-suite`](skills/pinduoduo-promo-banner-suite/SKILL.md) | 拼多多美工平替 | 拼多多 商品图、主图套图、详情图、活动图生成 | 拼多多美工平替 | 下沉市场强对比白底图/满减活动图/轮播图 |
| 42 | POD柔性定制设计 | Etsy / Shopify / Amazon | [`pod-print-on-demand-assets-suite`](skills/pod-print-on-demand-assets-suite/SKILL.md) | POD设计全案平替 | AI生成电商pod素材 | POD设计全案平替 | 印花提取贴合裂变一站式搞定 |
| 43 | POD柔性定制设计 | Etsy / Shopify / Amazon | [`printify-pod-3d-mockup-applier`](skills/printify-pod-3d-mockup-applier/SKILL.md) | POD贴图平替 | 电商印花贴合 | POD贴图平替 | 一键提取印花并真实贴合到各种白坯商品样机 |
| 44 | POD柔性定制设计 | Etsy / Shopify / Amazon | [`pod-pattern-hd-vector-extractor`](skills/pod-pattern-hd-vector-extractor/SKILL.md) | 印花提取平替 | 电商印花提取 | 印花提取平替 | 一键提取图片中高清印花 |
| 45 | POD柔性定制设计 | Etsy / Shopify / Amazon | [`pod-pattern-creative-variations-ai`](skills/pod-pattern-creative-variations-ai/SKILL.md) | 图案裂变平替 | 电商印花裂变 | 图案裂变平替 | 基于单张印花裂变出丰富颜色、排版与风格 |
| 46 | 电商图像生成与精修 | 全电商平台通用 | [`product-swap-scene-retainer`](skills/product-swap-scene-retainer/SKILL.md) | 商品换主体平替 | 电商商品替换 | 商品换主体平替 | 一键替换图片中主体 |
| 47 | 电商图像生成与精修 | 全电商平台通用 | [`canva-ecom-promo-poster-creator`](skills/canva-ecom-promo-poster-creator/SKILL.md) | Canva平替 | 电商促销海报 | Canva平替 | 自动适配各平台海报尺寸与营销标签 |
| 48 | 电商视频制作与仿拍 | 全电商平台通用 | [`sales-video-hook-script-ai`](skills/sales-video-hook-script-ai/SKILL.md) | 带货脚本平替 | AI电商带货脚本 | 带货脚本平替 | 自动输出前3秒抓人黄金口播、测评、种草脚本 |
| 49 | 电商视频制作与仿拍 | 全电商平台通用 | [`capcut-sales-video-auto-maker`](skills/capcut-sales-video-auto-maker/SKILL.md) | CapCut平替 | AI电商带货视频 | CapCut平替 | 上传商品图即可自动合成带货视频 |
| 50 | 电商图像生成与精修 | 全电商平台通用 | [`flairai-luxury-scene-studio`](skills/flairai-luxury-scene-studio/SKILL.md) | Flair AI平替 | 电商场景图生成 | Flair AI平替 | 大幅提升产品溢价感与视觉吸引力 |
| 51 | 主流AI音画模型专项 | 全电商平台通用 | [`seedance-2-rhythm-video-clone`](skills/seedance-2-rhythm-video-clone/SKILL.md) | Seedance仿拍平替 | Seedance 2.0 爆款视频复刻 | Seedance仿拍平替 | 复刻爆款构图与运镜运动节奏 |
| 52 | 主流AI音画模型专项 | 全电商平台通用 | [`seedance-2-dynamic-product-showcase`](skills/seedance-2-dynamic-product-showcase/SKILL.md) | Seedance商业平替 | Seedance 2.0 电商带货视频 | Seedance商业平替 | 首尾帧控制与多参考图动态商品展示大片 |
| 53 | 主流AI音画模型专项 | 全电商平台通用 | [`seedance-25-viral-emotion-clone`](skills/seedance-25-viral-emotion-clone/SKILL.md) | 电影感仿拍平替 | Seedance 2.5 爆款视频复刻 | 电影感仿拍平替 | 提取爆款情绪节奏与电影质感 |
| 54 | 主流AI音画模型专项 | 全电商平台通用 | [`seedance-25-cinema-product-commercial`](skills/seedance-25-cinema-product-commercial/SKILL.md) | Seedance2.5平替 | Seedance 2.5 电商带货视频 | Seedance2.5平替 | 超高真实感与电影质感的产品宣传大片 |
| 55 | 主流AI音画模型专项 | 全电商平台通用 | [`seedream-5-lite-chinese-typeset`](skills/seedream-5-lite-chinese-typeset/SKILL.md) | 中文生图排版平替 | Seedream 5.0 Lite 生成电商图 | 中文生图排版平替 | 强化中文汉字渲染与排版 |
| 56 | 主流AI音画模型专项 | 全电商平台通用 | [`seedream-5-pro-commercial-ecom`](skills/seedream-5-pro-commercial-ecom/SKILL.md) | Seedream商业平替 | Seedream 5.0 Pro 爆款电商图 | Seedream商业平替 | 全场景极高质量生图 |
| 57 | 电商平台专属合规素材 | SHEIN | [`shein-fast-fashion-lookbook-suite`](skills/shein-fast-fashion-lookbook-suite/SKILL.md) | SHEIN摄影平替 | SHEIN 商品图、主图套图、详情图、活动图生成 | SHEIN摄影平替 | 快时尚欧美风模特街拍/平铺图/穿搭场景图 |
| 58 | 电商视频制作与仿拍 | 微信视频号 | [`wechat-channels-viral-video-maker`](skills/wechat-channels-viral-video-maker/SKILL.md) | 视频号爆款平替 | 视频号 爆款视频生成 | 视频号爆款平替 | 情感共鸣好物分享与私域引流带货视频 |
| 59 | 跨境选品与数据分析 | Shopee (东南亚) | [`shopee-southeast-asia-image-suite`](skills/shopee-southeast-asia-image-suite/SKILL.md) | Shopee美工平替 | Shopee 商品图、主图套图、详情图、活动图生成 | Shopee美工平替 | 1:1方形图/多语言促销贴纸/东南亚大促海报 |
| 60 | 电商视频制作与仿拍 | 全电商平台通用 | [`video-storyboard-director-ai`](skills/video-storyboard-director-ai/SKILL.md) | 分镜生成平替 | AI视频分镜 | 分镜生成平替 | 镜头设计、运镜机位与文案分镜全流程输出 |
| 61 | 电商平台专属合规素材 | 淘宝天猫 | [`taobao-tmall-listing-image-suite`](skills/taobao-tmall-listing-image-suite/SKILL.md) | 淘系美工平替 | 淘宝天猫 商品图、主图套图、详情图、活动图生成 | 淘系美工平替 | 白底图/主图套图/详情页/直通车站内规范全覆盖 |
| 62 | 电商平台专属合规素材 | TEMU | [`temu-multi-sku-discount-image-suite`](skills/temu-multi-sku-discount-image-suite/SKILL.md) | TEMU美工平替 | Temu 商品图、主图套图、详情图、活动图生成 | TEMU美工平替 | 强性价比视觉主图/满减折扣图/多SKU组合图 |
| 63 | 电商平台专属合规素材 | TikTok / TikTok Shop | [`tiktok-shop-high-ctr-cover-maker`](skills/tiktok-shop-high-ctr-cover-maker/SKILL.md) | TikTok美工平替 | TikTok Shop 商品图、主图套图、详情图、活动图生成 | TikTok美工平替 | 短视频挂车封面/高点击商城主图/种草投流素材 |
| 64 | 电商视频制作与仿拍 | TikTok / TikTok Shop | [`tiktok-ugc-viral-video-maker`](skills/tiktok-ugc-viral-video-maker/SKILL.md) | TikTok爆款平替 | TikTok 爆款视频生成 | TikTok爆款平替 | 多语言口播卡点变装与跨境爆款种草视频 |
| 65 | 电商视频制作与仿拍 | 全电商平台通用 | [`video-feed-ad-assets-maker`](skills/video-feed-ad-assets-maker/SKILL.md) | 广告视频平替 | AI电商视频广告 | 广告视频平替 | 快速生成适合投流的信息流高点击视频素材 |
| 66 | 电商视频制作与仿拍 | 全电商平台通用 | [`lalal-video-audio-extractor-hd`](skills/lalal-video-audio-extractor-hd/SKILL.md) | 人声分离平替 | AI视频音频提取 | 人声分离平替 | 快速提取热门BGM伴奏与爆款旁白音频 |
| 67 | 电商视频制作与仿拍 | 全电商平台通用 | [`video-actor-role-swap-ai`](skills/video-actor-role-swap-ai/SKILL.md) | 角色替换平替 | AI视频角色替换 | 角色替换平替 | 上传新角色图 |
| 68 | 电商视频制作与仿拍 | 全电商平台通用 | [`video-subtitle-eraser-inpaint`](skills/video-subtitle-eraser-inpaint/SKILL.md) | 去字幕平替 | AI视频去字幕 | 去字幕平替 | 智能识别擦除视频字幕并无痕补全画面背景 |
| 69 | 电商视频制作与仿拍 | 全电商平台通用 | [`heygen-video-dubbing-multilingual`](skills/heygen-video-dubbing-multilingual/SKILL.md) | HeyGen平替 | AI视频翻译 | HeyGen平替 | 原声音画同步的多语言本地化视频 |
| 70 | 电商视频制作与仿拍 | 全电商平台通用 | [`topaz-video-upscale-60fps-hd`](skills/topaz-video-upscale-60fps-hd/SKILL.md) | Topaz视频平替 | AI视频超清修复 | Topaz视频平替 | 1080P/4K超清修复与60帧智能补帧 |
| 71 | 电商视频制作与仿拍 | 全电商平台通用 | [`video-watermark-remover-clean`](skills/video-watermark-remover-clean/SKILL.md) | 去水印软件平替 | AI视频去水印 | 去水印软件平替 | 批量清理二次创作素材平台LOGO |
| 72 | 主流AI音画模型专项 | 全电商平台通用 | [`vidu-q2-fast-pace-video-clone`](skills/vidu-q2-fast-pace-video-clone/SKILL.md) | Vidu仿拍平替 | Vidu Q2 爆款视频复刻 | Vidu仿拍平替 | 复刻快节奏穿搭、开箱与创意特效爆款 |
| 73 | 主流AI音画模型专项 | 全电商平台通用 | [`vidu-q2-product-consistency-sales`](skills/vidu-q2-product-consistency-sales/SKILL.md) | Vidu商业平替 | Vidu Q2 电商带货视频 | Vidu商业平替 | 参考图一致性带货视频 |
| 74 | 主流AI音画模型专项 | 全电商平台通用 | [`vidu-q3-stopmotion-unboxing-clone`](skills/vidu-q3-stopmotion-unboxing-clone/SKILL.md) | 定格开箱平替 | Vidu Q3 爆款视频复刻 | 定格开箱平替 | 还原机位转场与定格动画感的时尚开箱二创 |
| 75 | 主流AI音画模型专项 | 全电商平台通用 | [`vidu-q3-jewelry-texture-commercial`](skills/vidu-q3-jewelry-texture-commercial/SKILL.md) | Vidu Q3珠宝平替 | Vidu Q3 电商带货视频 | Vidu Q3珠宝平替 | 珠宝服装家具材质包装极高置信度物理还原 |
| 76 | 电商视频制作与仿拍 | 全电商平台通用 | [`kling-viral-video-clone-pro`](skills/kling-viral-video-clone-pro/SKILL.md) | 可灵商业平替 | AI爆款视频复刻 | 可灵商业平替 | 直接复制经过市场检验的爆款起量节奏与镜头 |
| 77 | 电商视频制作与仿拍 | 全电商平台通用 | [`viral-video-remake-toolkit-pro`](skills/viral-video-remake-toolkit-pro/SKILL.md) | 视频复刻工具平替 | AI爆款视频复刻、音频提取 | 视频复刻工具平替 | 视频结构分析仿拍与音频提取一体化工具 |
| 78 | 主流AI音画模型专项 | 全电商平台通用 | [`wanx-3-guangguang-viral-clone`](skills/wanx-3-guangguang-viral-clone/SKILL.md) | 淘宝逛逛仿拍平替 | 阿里Wanx 3.0 爆款视频复刻 | 淘宝逛逛仿拍平替 | 点淘与逛逛热门带货结构复刻 |
| 79 | 主流AI音画模型专项 | 全电商平台通用 | [`wanx-3-taobao-mainvideo-engine`](skills/wanx-3-taobao-mainvideo-engine/SKILL.md) | 阿里万相商业平替 | 阿里Wanx 3.0 电商带货视频 | 阿里万相商业平替 | 原生适配淘系主图短视频与阿里妈妈投流素材 |
| 80 | 电商图像生成与精修 | 全电商平台通用 | [`batch-white-background-cleaner`](skills/batch-white-background-cleaner/SKILL.md) | 抠图工具平替 | 电商白底图生成 | 抠图工具平替 | 批量生成合规白底图 |
| 81 | 电商视频制作与仿拍 | 小红书 (RedNote) | [`rednote-aesthetic-video-maker`](skills/rednote-aesthetic-video-maker/SKILL.md) | 小红书视频平替 | 小红书 爆款视频生成 | 小红书视频平替 | 打造高审美氛围感种草短片与开箱评测 |
| 82 | 电商视频制作与仿拍 | YouTube | [`youtube-product-review-video-pro`](skills/youtube-product-review-video-pro/SKILL.md) | YouTube爆款平替 | YouTube 爆款视频生成 | YouTube爆款平替 | 横屏深度测评与开箱大片 |
| 83 | 跨境选品与数据分析 | 1688批发 | [`ali1688-factory-sourcing-expert`](skills/ali1688-factory-sourcing-expert/SKILL.md) | 1688选品平替 | 1688选品专家 | 1688选品平替 | 绕过二道贩子赚差价 |
| 84 | 跨境选品与数据分析 | 亚马逊 (Amazon) | [`helium10-asin-spy-analyzer`](skills/helium10-asin-spy-analyzer/SKILL.md) | Helium 10平替 | 亚马逊-ASIN解析专家 | Helium 10平替 | 秒级透析对标爆款打法 |
| 85 | 跨境选品与数据分析 | 亚马逊 (Amazon) | [`sellersprite-keyword-blueocean-picker`](skills/sellersprite-keyword-blueocean-picker/SKILL.md) | 卖家精灵平替 | 亚马逊-关键词选品专家 | 卖家精灵平替 | 以词定款纯自然流获客 |
| 86 | 跨境选品与数据分析 | 亚马逊 (Amazon) | [`junglescout-market-niche-assessor`](skills/junglescout-market-niche-assessor/SKILL.md) | Jungle Scout平替 | 亚马逊-细分市场评估师 | Jungle Scout平替 | 防止盲目进入饱和红海类目造成压货亏损 |
| 87 | 跨境选品与数据分析 | 亚马逊 (Amazon) | [`amazon-hot-trend-hunter-pro`](skills/amazon-hot-trend-hunter-pro/SKILL.md) | 亚马逊趋势平替 | 亚马逊-爆款趋势挖掘师 | 亚马逊趋势平替 | 提前1~2个月布局季节性与突发趋势爆款 |
| 88 | 社媒数据与内容运营 | B站 (Bilibili) | [`bilibili-deep-review-social-ops`](skills/bilibili-deep-review-social-ops/SKILL.md) | 火烧云平替 | B站-社媒运营专家 | 火烧云平替 | 深度测评脚本与弹幕舆情把控 |
| 89 | 社媒数据与内容运营 | 全电商平台通用 | [`chanmama-creator-data-engine-pro`](skills/chanmama-creator-data-engine-pro/SKILL.md) | 蝉妈妈平替 | 达人数据引擎 | 蝉妈妈平替 | 彻底取代人工手动统计 |
| 90 | 模特换装与假人台换脸 | 全电商平台通用 | [`door-outfit-change-viral-maker`](skills/door-outfit-change-viral-maker/SKILL.md) | 换装仿拍平替 | 女装开门换装 | 换装仿拍平替 | 快速生成开门换装短视频 |
| 91 | 综合电商工作流 | 抖音 / 抖店 | [`douyin-bluesea-hot-product-collector`](skills/douyin-bluesea-hot-product-collector/SKILL.md) | 抖店选品平替 | 抖音-蓝海爆品采集师 | 抖店选品平替 | 规避红海大词竞争 |
| 92 | 综合电商工作流 | 抖音 / 抖店 | [`douyin-1688-fast-listing-copilot`](skills/douyin-1688-fast-listing-copilot/SKILL.md) | 上货助手平替 | 抖音-极速上货助手 | 上货助手平替 | 自动采集1688热卖商品 |
| 93 | 社媒数据与内容运营 | 抖音 / 抖店 | [`douyin-trending-social-director`](skills/douyin-trending-social-director/SKILL.md) | 蝉妈妈平替 | 抖音-社媒运营专家 | 蝉妈妈平替 | 快速追踪行业飙升热点 |
| 94 | 综合电商工作流 | 抖音 / 抖店 | [`douyin-viral-video-dropship-distributor`](skills/douyin-viral-video-dropship-distributor/SKILL.md) | 跟卖铺货平替 | 抖音-爆款视频跟卖与铺货专家 | 跟卖铺货平替 | 打通爆款发现-链接采集-极速上架全链路 |
| 95 | 电商视频制作与仿拍 | 全电商平台通用 | [`duo-character-viral-video-sync`](skills/duo-character-viral-video-sync/SKILL.md) | 双人仿拍平替 | 双人爆款视频模仿 | 双人仿拍平替 | 双人动作神态精准同步 |
| 96 | 跨境选品与数据分析 | 全电商平台通用 | [`crossborder-sourcing-copilot-pro`](skills/crossborder-sourcing-copilot-pro/SKILL.md) | 选品上货平替 | AI电商选品上货 | 选品上货平替 | 覆盖亚马逊/TikTok/Shopee等多平台一键上新 |
| 97 | 电商图像生成与精修 | 全电商平台通用 | [`image-deai-photorealistic-hd`](skills/image-deai-photorealistic-hd/SKILL.md) | 去AI感平替 | 高清写实去AI感 | 去AI感平替 | 极速去除AI油腻失真感 |
| 98 | 电商图像生成与精修 | 全电商平台通用 | [`topaz-image-upscale-ultra-pro`](skills/topaz-image-upscale-ultra-pro/SKILL.md) | Topaz平替 | 超清修复强化细节 | Topaz平替 | 分块超分4K/8K大图 |
| 99 | 电商图像生成与精修 | 全电商平台通用 | [`ai-image-watermark-cleaner-hd`](skills/ai-image-watermark-cleaner-hd/SKILL.md) | 图片去水印平替 | 图片去水印 | 图片去水印平替 | 自动清除满屏局部Logo文字图形 |
| 100 | 模特换装与假人台换脸 | 全电商平台通用 | [`clothing-mannequin-to-model-hd`](skills/clothing-mannequin-to-model-hd/SKILL.md) | 假人台穿搭平替 | 模特换装高一致性 | 假人台穿搭平替 | 假人台与平铺图转超写真模特试穿 |

*(更多 101 ~ 300 号技能完整清单，请直接查阅仓库根目录下的 [`REGISTRY.json`](REGISTRY.json) 或 [`REGISTRY.xlsx`](REGISTRY.xlsx))*

---

## 技能规范体系 (TRACE 4.8+ 标准)

每个技能均具备完整的工程防错与交付保障：
- **四段式 Description**：明确触发问句、目标人群、交付成品规格与免责条款；
- **智能预估 (qhkit estimate)**：支持扣费前预估积分消耗，避免盲目批量生成；
- **反模式限制 (Limitations)**：针对高反光透明件、极端复杂印花等标注清晰的调优指南与 FAQ。

---

## 许可证 (License)

[MIT License](LICENSE)

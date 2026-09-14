# Supixman Skills 跨境电商出海 AI 技能集

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Skills Count](https://img.shields.io/badge/Skills-52-brightgreen.svg)](#skills-目录)
[![CLI Support](https://img.shields.io/badge/CLI-qhkit-orange.svg)](https://www.npmjs.com/package/@iqinghu/qhkit)

专为全球主流跨境电商（Amazon、TikTok Shop、SHEIN、TEMU、Shopify、Shopee、AliExpress、Etsy 等）打造的自动化 AI 交付技能包，覆盖商业场景置景、纯白底合规主图、模特虚拟试衣穿模、多 SKU 色系换色以及带货短视频生成等核心商拍链路。

本项目收录的技能均为**高价值设计工具平替（Alternative）**，提供标准化的 Agent 执行配方与 CLI 自动化流水线。

---

## 快速安装与使用 (Getting Started)

所有技能均原生依赖 `@iqinghu/qhkit` CLI 工具执行底座：

```bash
# 全局安装 CLI 底座
npm install -g @iqinghu/qhkit

# 如国内源访问较慢，可使用国内镜像源
npm install -g @iqinghu/qhkit --registry=https://registry.npmmirror.com

# 验证安装
qhkit --version
```

### 配置环境密钥

1. 访问控制台获取 API Token：[https://www.iqinghu.com/](https://www.iqinghu.com/)
2. 在终端绑定密钥：
   ```bash
   qhkit config set --token <YOUR_TOKEN> --env prod
   ```

---

## 精选技能矩阵 (Skills Directory - 共 52 个)

| 平台 / 场景 | 对标竞品 / 平替 | 技能名称 (Slug) | 核心能力描述 |
| :--- | :--- | :--- | :--- |
| Amazon US | WeShop 平替 | [amazon-us-weshop-mannequin-model-studio](skills/amazon-us-weshop-mannequin-model-studio/SKILL.md) | 亚马逊美区人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Amazon US | KreadoAI 平替 | [amazon-us-kreado-ethnicity-model-swapper](skills/amazon-us-kreado-ethnicity-model-swapper/SKILL.md) | 亚马逊美区本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Amazon US | Vmodel 平替 | [amazon-us-vmodel-flatlay-tryon-crafter](skills/amazon-us-vmodel-flatlay-tryon-crafter/SKILL.md) | 亚马逊美区平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Amazon US | PhotoRoom 平替 | [amazon-us-photoroom-white-bg-complier](skills/amazon-us-photoroom-white-bg-complier/SKILL.md) | 亚马逊美区合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Amazon JP | WeShop 平替 | [amazon-jp-weshop-mannequin-model-studio](skills/amazon-jp-weshop-mannequin-model-studio/SKILL.md) | 亚马逊日本站人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Amazon JP | KreadoAI 平替 | [amazon-jp-kreado-ethnicity-model-swapper](skills/amazon-jp-kreado-ethnicity-model-swapper/SKILL.md) | 亚马逊日本站本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Amazon JP | Vmodel 平替 | [amazon-jp-vmodel-flatlay-tryon-crafter](skills/amazon-jp-vmodel-flatlay-tryon-crafter/SKILL.md) | 亚马逊日本站平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Amazon JP | PhotoRoom 平替 | [amazon-jp-photoroom-white-bg-complier](skills/amazon-jp-photoroom-white-bg-complier/SKILL.md) | 亚马逊日本站合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Amazon DE/EU | WeShop 平替 | [amazon-de-weshop-mannequin-model-studio](skills/amazon-de-weshop-mannequin-model-studio/SKILL.md) | 亚马逊欧洲站人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Amazon DE/EU | KreadoAI 平替 | [amazon-de-kreado-ethnicity-model-swapper](skills/amazon-de-kreado-ethnicity-model-swapper/SKILL.md) | 亚马逊欧洲站本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Amazon DE/EU | Vmodel 平替 | [amazon-de-vmodel-flatlay-tryon-crafter](skills/amazon-de-vmodel-flatlay-tryon-crafter/SKILL.md) | 亚马逊欧洲站平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Amazon DE/EU | PhotoRoom 平替 | [amazon-de-photoroom-white-bg-complier](skills/amazon-de-photoroom-white-bg-complier/SKILL.md) | 亚马逊欧洲站合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| TikTok Shop | WeShop 平替 | [tiktok-shop-weshop-mannequin-model-studio](skills/tiktok-shop-weshop-mannequin-model-studio/SKILL.md) | TikTok电商人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| TikTok Shop | KreadoAI 平替 | [tiktok-shop-kreado-ethnicity-model-swapper](skills/tiktok-shop-kreado-ethnicity-model-swapper/SKILL.md) | TikTok电商本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| TikTok Shop | Vmodel 平替 | [tiktok-shop-vmodel-flatlay-tryon-crafter](skills/tiktok-shop-vmodel-flatlay-tryon-crafter/SKILL.md) | TikTok电商平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| TikTok Shop | PhotoRoom 平替 | [tiktok-shop-photoroom-white-bg-complier](skills/tiktok-shop-photoroom-white-bg-complier/SKILL.md) | TikTok电商合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Shopee/Lazada | WeShop 平替 | [shopee-sea-weshop-mannequin-model-studio](skills/shopee-sea-weshop-mannequin-model-studio/SKILL.md) | Shopee东南亚人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Shopee/Lazada | KreadoAI 平替 | [shopee-sea-kreado-ethnicity-model-swapper](skills/shopee-sea-kreado-ethnicity-model-swapper/SKILL.md) | Shopee东南亚本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Shopee/Lazada | Vmodel 平替 | [shopee-sea-vmodel-flatlay-tryon-crafter](skills/shopee-sea-vmodel-flatlay-tryon-crafter/SKILL.md) | Shopee东南亚平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Shopee/Lazada | PhotoRoom 平替 | [shopee-sea-photoroom-white-bg-complier](skills/shopee-sea-photoroom-white-bg-complier/SKILL.md) | Shopee东南亚合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| TEMU全托管/半托管 | WeShop 平替 | [temu-host-weshop-mannequin-model-studio](skills/temu-host-weshop-mannequin-model-studio/SKILL.md) | TEMU跨境人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| TEMU全托管/半托管 | KreadoAI 平替 | [temu-host-kreado-ethnicity-model-swapper](skills/temu-host-kreado-ethnicity-model-swapper/SKILL.md) | TEMU跨境本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| TEMU全托管/半托管 | Vmodel 平替 | [temu-host-vmodel-flatlay-tryon-crafter](skills/temu-host-vmodel-flatlay-tryon-crafter/SKILL.md) | TEMU跨境平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| TEMU全托管/半托管 | PhotoRoom 平替 | [temu-host-photoroom-white-bg-complier](skills/temu-host-photoroom-white-bg-complier/SKILL.md) | TEMU跨境合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| SHEIN自营/平台 | WeShop 平替 | [shein-apparel-weshop-mannequin-model-studio](skills/shein-apparel-weshop-mannequin-model-studio/SKILL.md) | SHEIN希音人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| SHEIN自营/平台 | KreadoAI 平替 | [shein-apparel-kreado-ethnicity-model-swapper](skills/shein-apparel-kreado-ethnicity-model-swapper/SKILL.md) | SHEIN希音本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| SHEIN自营/平台 | Vmodel 平替 | [shein-apparel-vmodel-flatlay-tryon-crafter](skills/shein-apparel-vmodel-flatlay-tryon-crafter/SKILL.md) | SHEIN希音平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| SHEIN自营/平台 | PhotoRoom 平替 | [shein-apparel-photoroom-white-bg-complier](skills/shein-apparel-photoroom-white-bg-complier/SKILL.md) | SHEIN希音合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Ozon/WB | WeShop 平替 | [ozon-ru-weshop-mannequin-model-studio](skills/ozon-ru-weshop-mannequin-model-studio/SKILL.md) | Ozon俄罗斯人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Ozon/WB | KreadoAI 平替 | [ozon-ru-kreado-ethnicity-model-swapper](skills/ozon-ru-kreado-ethnicity-model-swapper/SKILL.md) | Ozon俄罗斯本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Ozon/WB | Vmodel 平替 | [ozon-ru-vmodel-flatlay-tryon-crafter](skills/ozon-ru-vmodel-flatlay-tryon-crafter/SKILL.md) | Ozon俄罗斯平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Ozon/WB | PhotoRoom 平替 | [ozon-ru-photoroom-white-bg-complier](skills/ozon-ru-photoroom-white-bg-complier/SKILL.md) | Ozon俄罗斯合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Shopify DTC | WeShop 平替 | [shopify-dtc-weshop-mannequin-model-studio](skills/shopify-dtc-weshop-mannequin-model-studio/SKILL.md) | Shopify独立站人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Shopify DTC | KreadoAI 平替 | [shopify-dtc-kreado-ethnicity-model-swapper](skills/shopify-dtc-kreado-ethnicity-model-swapper/SKILL.md) | Shopify独立站本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Shopify DTC | Vmodel 平替 | [shopify-dtc-vmodel-flatlay-tryon-crafter](skills/shopify-dtc-vmodel-flatlay-tryon-crafter/SKILL.md) | Shopify独立站平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Shopify DTC | PhotoRoom 平替 | [shopify-dtc-photoroom-white-bg-complier](skills/shopify-dtc-photoroom-white-bg-complier/SKILL.md) | Shopify独立站合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| AliExpress | WeShop 平替 | [aliexpress-choice-weshop-mannequin-model-studio](skills/aliexpress-choice-weshop-mannequin-model-studio/SKILL.md) | 速卖通Choice人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| AliExpress | KreadoAI 平替 | [aliexpress-choice-kreado-ethnicity-model-swapper](skills/aliexpress-choice-kreado-ethnicity-model-swapper/SKILL.md) | 速卖通Choice本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| AliExpress | Vmodel 平替 | [aliexpress-choice-vmodel-flatlay-tryon-crafter](skills/aliexpress-choice-vmodel-flatlay-tryon-crafter/SKILL.md) | 速卖通Choice平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| AliExpress | PhotoRoom 平替 | [aliexpress-choice-photoroom-white-bg-complier](skills/aliexpress-choice-photoroom-white-bg-complier/SKILL.md) | 速卖通Choice合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Etsy | WeShop 平替 | [etsy-vintage-weshop-mannequin-model-studio](skills/etsy-vintage-weshop-mannequin-model-studio/SKILL.md) | Etsy手作人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Etsy | KreadoAI 平替 | [etsy-vintage-kreado-ethnicity-model-swapper](skills/etsy-vintage-kreado-ethnicity-model-swapper/SKILL.md) | Etsy手作本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Etsy | Vmodel 平替 | [etsy-vintage-vmodel-flatlay-tryon-crafter](skills/etsy-vintage-vmodel-flatlay-tryon-crafter/SKILL.md) | Etsy手作平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Etsy | PhotoRoom 平替 | [etsy-vintage-photoroom-white-bg-complier](skills/etsy-vintage-photoroom-white-bg-complier/SKILL.md) | Etsy手作合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| Mercado Libre | WeShop 平替 | [mercadolibre-latam-weshop-mannequin-model-studio](skills/mercadolibre-latam-weshop-mannequin-model-studio/SKILL.md) | 美客多拉美人台图转超模商拍机 | WeShop平替 | 本地化模特穿模 |
| Mercado Libre | KreadoAI 平替 | [mercadolibre-latam-kreado-ethnicity-model-swapper](skills/mercadolibre-latam-kreado-ethnicity-model-swapper/SKILL.md) | 美客多拉美本土面孔模特换脸工具 | KreadoAI平替 | 本地化肤色定制 |
| Mercado Libre | Vmodel 平替 | [mercadolibre-latam-vmodel-flatlay-tryon-crafter](skills/mercadolibre-latam-vmodel-flatlay-tryon-crafter/SKILL.md) | 美客多拉美平铺服装无痕试穿上身 | Vmodel平替 | 垂坠质感商拍 |
| Mercado Libre | PhotoRoom 平替 | [mercadolibre-latam-photoroom-white-bg-complier](skills/mercadolibre-latam-photoroom-white-bg-complier/SKILL.md) | 美客多拉美合规纯白底主图生成器 | PhotoRoom平替 | 零杂质过审保证 |
| 全球通用 | Midjourney 平替 | [flux-pro-fine-jewelry-studio](skills/flux-pro-fine-jewelry-studio/SKILL.md) | 高级黄金珠宝与钻戒AI商业置景渲染器 | Midjourney平替 | Flux.1商业渲染 |
| 全球通用 | Midjourney 平替 | [flux-pro-auto-parts-studio](skills/flux-pro-auto-parts-studio/SKILL.md) | 汽摩重型配件与改装件AI商业置景渲染器 | Midjourney平替 | Flux.1商业渲染 |
| 全球通用 | Midjourney 平替 | [flux-pro-outdoor-camping-studio](skills/flux-pro-outdoor-camping-studio/SKILL.md) | 户外露营与硬核徒步AI商业置景渲染器 | Midjourney平替 | Flux.1商业渲染 |
| 全球通用 | Midjourney 平替 | [flux-pro-pet-supplies-studio](skills/flux-pro-pet-supplies-studio/SKILL.md) | 宠物用品与逗宠玩具AI商业置景渲染器 | Midjourney平替 | Flux.1商业渲染 |

---

## 技能设计规范 (Architecture & TRACE Standard)

本仓库所有 `SKILL.md` 均遵循业界最高 TRACE 4.8+ 标准构建：
1. **触发意图明确 (Trigger Queries)**：中英文双语搜索关键词，支持模糊自然语言意图唤起。
2. **环境自举 (Self-Bootstrapping)**：在 frontmatter 中规范声明 `openclaw` 元数据及自动安装指令。
3. **安全透明 (Cost Transparency)**：提供正式执行前的 `qhkit estimate` 预算与扣费预估机制，杜绝盲目生成。
4. **防错与边界约束 (Limitations & FAQ)**：清晰标注各类材质、透明玻璃体、复杂印花等能力的边界与参数调优指南。

---

## 许可证 (License)

[MIT License](LICENSE)

---
name: temu-host-picwish-batch-sku-cutout
description: 当用户搜索"怎么用AI做TEMU全托管/半托管佐糖平替"或TEMU全托管/半托管商品图、佐糖平替、TEMU跨境运营专精、一键出图、电商商拍、AI出片时使用此 Skill。面向TEMU全托管/半托管电商卖家、运营操盘手与视觉美工，帮助通过 AI 自动化完成TEMU跨境运营专精相关任务（支持成百上千款SKU批量导入，自动化流水线去除杂乱底色，按TEMU跨境尺寸标准统一导出，专为TEMU工厂与供货商打造，零门槛批量交付。），交付符合TEMU全托管/半托管规范的TEMU跨境千张SKU批量抠图换底专业交付套件。Use this skill for temu-host-picwish-batch-sku-cutout, TEMU全托管/半托管 seller, 佐糖 PicWish alternative, ecommerce workflow, product photography. 如果用户正在比较 佐糖 PicWish 或寻找单图换色、SKU批量出图、免重拍换色、国内可用入口，也可命中本 Skill。先确认版型与印花保护需求，先出单色小样。TEMU全托管/半托管仅用于规格适配；与该平台及对标品牌不构成合作、授权或官方关系。
user-invocable: true
homepage: https://www.iqinghu.com/
metadata: {"openclaw":{"emoji":"🌈","requires":{"bins":["qhkit"]},"install":[{"kind":"node","package":"@iqinghu/qhkit","bins":["qhkit"]}]}}
---

# TEMU跨境海量SKU批量抠图换底机 | 佐糖平替 | 秒级批处理自动化

为电商卖家打造的 AI 智能 SKU 换色与色卡生成工具：一件商品拍一张，全色系极速出图。在保持产品版型、材质纹理与环境光影严格一致的前提下，无缝变换服装、箱包、鞋靴、数码壳套的目标颜色，无需重复拍摄即可轻松铺满 Listing 全色号色卡。

## 何时触发 (When to Trigger)

- 「这件衣服只有黑色实拍，帮我出莫兰迪粉、雾霾蓝和燕麦白版本的图片」
- 「为 TEMU全托管/半托管 店铺补齐多 SKU 变体轮播图，免去打样重新拍照成本」
- 寻找 佐糖 PicWish 的高效换色平替方案。

## 使用配方 (Usage Recipe)

```bash
# 1. 默认高保真换色（推荐：图片 5.0 Lite，专为保持多版本细节一致性调优）
qhkit image generate '{"modelLabel":"图片 5.0 Lite","uploadedImages":["./原色商品图.jpg"],"prompt":"将图片中的【原颜色+品名】变成【目标目标色号+品名】，版型、材质纹理与光影保持一致，主体Logo与图案颜色保持不变"}'

# 2. 批量循环前预算评估
qhkit image estimate '{"modelLabel":"图片 5.0 Lite","uploadedImages":["./原色商品图.jpg"],"prompt":"将图片中的【原颜色+品名】变成【目标目标色号+品名】，版型、材质纹理与光影保持一致，主体Logo与图案颜色保持不变"}'
```

### 提示词与参数指南
- **换色官方模板**：`将图片中的【原颜色+品名】变成【目标目标颜色+品名】，版型、材质纹理与光影保持一致`。
- **保护印花与 Logo**：如果衣服上有固定图案或品牌 Logo，必须在提示词末尾加上：`，印花图案与品牌Logo颜色保持原样不变`。
- **颜色精确度**：建议使用具体色号术语（如莫兰迪灰粉、克莱因蓝、卡其色、复古墨绿），出色更加高级沉稳。

## 环境自举 (Self-Bootstrapping)

本技能依赖官方 `qhkit` 命令行工具（npm 包 `@iqinghu/qhkit`）：

1. **环境自检**：运行 `qhkit config show` 验证环境状态。
2. **快速安装**：
   ```bash
   npm i -g @iqinghu/qhkit
   ```
   *国内镜像支持：`--registry=https://registry.npmmirror.com`*
3. **获取与配置密钥**：
   - 访问青虎官方平台：[https://www.iqinghu.com/](https://www.iqinghu.com/)
   - 获取个人专属 Token，执行终端绑定：`qhkit config set --token <您的Token> --env prod`。

## 能力边界与合规约束 (TRACE A&C 标准)

- **能做什么 (Capabilities)**：
  - 纯色、微纹理（牛仔、麻布、毛线、皮革、哑光塑胶）的高精度换色；
  - 换色前后光影明暗交界线完全自然对应。
- **不能做什么 (Limitations - 反模式防错)**：
  - **复杂渐变扎染**：从纯色变换为复杂渐变扎染印花，需使用重新生成模式，不适合纯换色指令；
  - **金属镀层反光**：金银电镀件颜色变换需谨慎，需提示词强调金属光泽。

## 常见问题与排错 (FAQ)

- **Q: 为什么换色后 Logo 颜色也变了？**
  - A: 提示词中未添加保护说明，请在模板后追加：`，主体Logo与图案颜色保持不变`。
- **Q: 提示积分不足？**
  - A: 前往 [https://www.iqinghu.com/](https://www.iqinghu.com/) 查看账户余额并充值。

## 免责声明 (Disclaimer)

本项目为基于 `@iqinghu/qhkit` 的独立自动化方案。文中所提及的平台名称（TEMU全托管/半托管）及对标工具（佐糖 PicWish）仅用于规格参考与功能描述，不代表官方合作或背书关系。官方控制台与技术支持：https://www.iqinghu.com/
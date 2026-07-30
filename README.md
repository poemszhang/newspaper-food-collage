# Newspaper Food Collage

一个用于生成“旧报纸手撕拼贴”视觉的 Cursor Agent Skill。

它会把自然语言主题转译为真实手工纸艺感的图片提示词：使用旧报纸、食品包装纸和哑光彩纸塑造主体，保留毛边、纸纤维、错位粘贴、印刷纹理与大片暖白留白。

## 生成案例

<p align="center">
  <img src="./examples/kyusu-teapot.png" alt="旧报纸拼贴茶壶" width="30%">
  <img src="./examples/matcha-milk-tea.png" alt="旧报纸拼贴抹茶奶茶" width="30%">
  <img src="./examples/milk.png" alt="旧报纸拼贴牛奶" width="30%">
</p>

<p align="center">
  <img src="./examples/seafood-soup-curry.png" alt="旧报纸拼贴海鲜汤咖喱" width="30%">
  <img src="./examples/hotpot.png" alt="旧报纸拼贴火锅" width="30%">
</p>

## 风格特征

- 旧报纸、广告页和食品包装纸的再生材料质感
- 不规则手撕边缘、纸张纤维、翘边与叠层
- 低饱和的土黄、砖红、橄榄绿、灰褐配色
- 印刷文字、数字、网点和条码作为表面纹理
- 单物标本、散点图鉴、餐食组合和复古海报构图
- 柔和扫描光、大面积暖白背景

## 安装

将仓库克隆到 Cursor 的个人 Skills 目录：

```bash
git clone https://github.com/peishizhang49-stack/newspaper-food-collage.git \
  ~/.cursor/skills/newspaper-food-collage
```

重新开启 Cursor 会话后即可通过自然语言自动触发。

## 使用示例

```text
用报纸撕贴食物风做一张草莓奶油蛋糕，竖版，留白多一点。
```

```text
画一组广州早茶：虾饺、烧卖、叉烧包和茶壶，像复古废纸图鉴。
```

```text
把我的猫做成旧报纸和零食包装拼贴，单物标本构图。
```

```text
做一张现代一点的报纸拼贴海报，主体是咖啡和可颂，标题区留空。
```

```text
给我这个风格的提示词，主题是秋天的蘑菇篮。
```

## 默认生成规则

未指定细节时，Skill 默认使用：

- 1–5 个主体
- 暖白竖版纸张
- 松散、不对称的散点构图
- 正视或轻微俯视视角
- 无可读标题、品牌、签名或水印

完整的风格定义、提示词模板、负面约束和验收标准请参阅 [`SKILL.md`](./SKILL.md)。

## 说明

本 Skill 蒸馏的是可复用的材料、构图和手工工艺特征，不用于复制特定作品的完整布局、签名、水印或独有文字。

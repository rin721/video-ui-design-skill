# 字体与排版

## Tokens

```yaml
typography_tokens:
  font_family:
    display: "Inter, ui-sans-serif, system-ui, sans-serif"
    body: "Inter, ui-sans-serif, system-ui, sans-serif"
    mono: "ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
  type_scale:
    display_lg:
      size: "3.75rem"
      line_height: "1.08"
      weight: "700"
      letter_spacing: "0"
    display_md:
      size: "3rem"
      line_height: "1.1"
      weight: "700"
      letter_spacing: "0"
    h1:
      size: "2.25rem"
      line_height: "1.16"
      weight: "700"
      letter_spacing: "0"
    h2:
      size: "1.75rem"
      line_height: "1.22"
      weight: "650"
      letter_spacing: "0"
    h3:
      size: "1.25rem"
      line_height: "1.32"
      weight: "650"
      letter_spacing: "0"
    body_lg:
      size: "1.125rem"
      line_height: "1.65"
      weight: "400"
    body_md:
      size: "1rem"
      line_height: "1.6"
      weight: "400"
    body_sm:
      size: "0.875rem"
      line_height: "1.5"
      weight: "400"
    caption:
      size: "0.75rem"
      line_height: "1.45"
      weight: "500"
    label:
      size: "0.875rem"
      line_height: "1.2"
      weight: "650"
```

## Rules

- display 样式只用于 hero 身份、重大页面标题或强编辑型标题。
- `h1` 到 `h3` 用于页面层级和组件区块。
- 长阅读段落宽度控制在 `58ch` 到 `72ch`。
- `body_sm` 和 `caption` 用于 metadata；重要标签不得低于 `0.75rem`。
- 中文、英文、数字和代码样式文本混排时，letter spacing 保持 `0`。
- mono 只用于代码、命令、token 和机器可读值。

## Modes

```yaml
typography_rules:
  heading_density: "大标题需要宽松空间；紧凑面板使用 h3 或 label"
  paragraph_width: "阅读文本 58ch 到 72ch；卡片文本 40ch 到 56ch"
  editorial_mode: "更慢节奏、更大 h1、更舒展行高、更强段落宽度控制"
  marketing_mode: "display 标题、短辅助文案、高对比操作标签"
  dashboard_mode: "紧凑标签、清晰数字、小 caption，不在面板中使用 hero 级字号"
```

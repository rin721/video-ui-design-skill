# 色彩系统

## Color Tokens

使用 neutral token 构建结构，brand token 表达身份和操作，accent token 提供辅助，state token 表达反馈。

```yaml
color_tokens:
  primitive:
    neutral_0: "#ffffff"
    neutral_50: "#fbfcfe"
    neutral_100: "#f4f7fa"
    neutral_200: "#e7ecf2"
    neutral_300: "#cfd8e3"
    neutral_400: "#9aa8b6"
    neutral_500: "#6b7785"
    neutral_600: "#52616b"
    neutral_700: "#344351"
    neutral_800: "#1f2933"
    neutral_900: "#111827"
    brand_50: "#fff1f5"
    brand_100: "#ffe3eb"
    brand_200: "#ffc8d6"
    brand_300: "#fa9eb8"
    brand_400: "#ee6f92"
    brand_500: "#d94a73"
    brand_600: "#be3455"
    brand_700: "#9f2846"
    brand_800: "#7f233c"
    accent_50: "#edfdf9"
    accent_100: "#ccfbef"
    accent_500: "#0f9f8f"
    accent_700: "#0f766e"
  semantic:
    bg_page: "neutral_50"
    bg_surface: "neutral_0"
    bg_surface_elevated: "neutral_0 at 86 percent"
    bg_inverse: "neutral_900"
    text_primary: "neutral_800"
    text_secondary: "neutral_700"
    text_muted: "neutral_600"
    text_inverse: "neutral_0"
    border_subtle: "neutral_200"
    border_default: "neutral_300"
    border_strong: "neutral_400"
    action_primary: "brand_600"
    action_primary_hover: "brand_700"
    action_secondary: "accent_50"
    action_secondary_hover: "accent_100"
    focus_ring: "accent_700"
    success: "#177245"
    warning: "#a15c00"
    danger: "#b42318"
    info: "#2563eb"
```

## Usage

```yaml
color_usage:
  dominant_ratio: "70 percent neutral page and surface"
  secondary_ratio: "20 percent soft brand or accent wash"
  accent_ratio: "10 percent active, focus, status, and conversion marks"
  contrast_rules:
    body_text: "minimum 4.5:1"
    large_text: "minimum 3:1"
    interactive_focus: "clearly visible and not color-only"
  dark_mode_strategy: "将表面反转到 neutral_900 和 neutral_800，将文字提升到 neutral_100，并降低品牌色彩度"
  brand_swap_strategy: "独立替换 brand scale 与 accent scale，同时保留语义映射"
```

## Status Rules

- success、warning、danger 和 info 必须搭配图标、标题、辅助文本或结构处理。
- 只有在文字对比度合规时才使用色块背景。
- 不将主品牌色用于破坏性操作。
- focus ring 在按钮、链接、卡片、表单字段和菜单项中保持一致。

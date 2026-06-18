# Color System

## Color Tokens

Use neutral tokens for structure, brand tokens for identity and action, accent tokens for support, and state tokens for feedback.

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
  dark_mode_strategy: "invert surfaces to neutral_900 and neutral_800, lift text to neutral_100, and soften brand chroma"
  brand_swap_strategy: "replace brand scale and accent scale independently while preserving semantic mapping"
```

## Status Rules

- Pair success, warning, danger, and info with icons, headings, helper text, or structural treatment.
- Use tinted backgrounds only when the text contrast remains compliant.
- Avoid using the primary brand color for destructive actions.
- Use focus ring color consistently across buttons, links, cards, form fields, and menu items.

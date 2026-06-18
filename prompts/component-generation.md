# 组件生成 Prompt

```text
使用该 schema 生成可复用组件：name、purpose、anatomy、variants、states、tokens_used、behavior、accessibility、do 和 dont。

颜色、排版、间距、圆角、阴影、动效和 z-index 必须使用语义化 token。状态可能出现时，包含 default、hover、focus、active、disabled、loading、error 和 selected。状态切换时尺寸保持稳定。提供键盘行为，并为 icon-only 控件提供可访问名称。

组件必须原创、可替换、响应式，并可用 HTML、CSS 和组件框架实现。不要使用受保护图片、品牌标志、独特 class 命名或独特视觉签名。
```

## Component Checklist

- Purpose 是一句话。
- Anatomy 命名结构部分，不描述无关视觉细节。
- Variants 有实际用途且互相清楚。
- States 具备视觉和语义反馈。
- Token 使用语义化。
- Behavior 在相关时包含键盘和 loading 规则。
- Accessibility 在相关时包含 label、role、focus 和 reduced motion。
- Do 和 dont 能防止常见误用。

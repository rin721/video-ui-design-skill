# 风格替换 Prompt

使用该 block 在保持组件系统的同时调整品牌表达。

```text
使用相同语义化组件契约创建新的视觉方向。替换主品牌色阶、辅助强调色阶、媒体调性、动效强度和排版强调，同时保持可访问性、布局稳定性、响应式行为和组件状态。

设置品牌维度：
- seriousness: [low | medium | high]
- warmth: [low | medium | high]
- innovation: [low | medium | high]
- luxury: [low | medium | high]
- playfulness: [low | medium | high]
- editorial: [low | medium | high]
- technical_depth: [low | medium | high]

正文对比度保持 4.5:1 或更高，较大文字保持 3:1 或更高，适用的交互 UI 边界保持 3:1。每个状态都必须用颜色加文字、图标或结构表达。不要使用受保护资产、品牌标志、独特 artwork 或独特页面签名。
```

## Adjustment Matrix

- 更高 seriousness：更安静的动效、更强中性色对比、更少装饰标记。
- 更高 warmth：更柔和辅助色、更友好的空状态、更多人性化语境。
- 更高 innovation：更清晰图表、更利落微交互、更强系统反馈。
- 更高 luxury：更多留白、更少 metadata、更高质感媒体、更少强调。
- 更高 playfulness：更亮辅助强调、小型动效 affordance、更轻标签。
- 更高 editorial：更大阅读节奏、更强文章层级、更宽媒体。
- 更高 technical_depth：更强代码块、数据表、sidebar 层级和任务提示。

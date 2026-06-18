# 页面生成 Prompt

```text
使用 Soft Signal Interface 设计系统生成完整响应式网站页面。

Inputs:
- site_type: [personal_homepage | blog | community | saas | ecommerce | documentation | landing_page]
- content_density: [sparse | balanced | dense]
- conversion_goal: [soft | hard | repeat_engagement | task_completion]
- brand_dimensions: seriousness, warmth, innovation, luxury, playfulness, editorial, technical_depth

用语义化 section、可复用组件和可替换资产构建页面。使用可访问 landmarks、一个 h1、逻辑标题、可见 focus 状态、键盘安全控件、响应式网格和 44px 移动端点击区域。首屏必须有用。主操作要清晰，但不要过度重复。

返回可实现结构、token 映射、组件列表、响应式行为和可访问性说明。
```

## Page Rules

- Landing pages 需要 hero、proof、features、conversion 和 footer。
- Personal pages 需要 identity、credibility、selected work、writing or projects、contact 和 footer。
- Blogs 需要 editorial header、featured article、category navigation、article grid、subscription 和 footer。
- Communities 需要 shared purpose、active discussions、member signals、join path 和 footer。
- SaaS pages 需要 value、product clarity、proof、pricing or plan path、signup 和 footer。
- Ecommerce pages 需要 category browsing、product grid、product details、cart path 和 checkout support。
- Documentation 需要 search、navigation hierarchy、content area、code blocks、callouts 和 pagination。

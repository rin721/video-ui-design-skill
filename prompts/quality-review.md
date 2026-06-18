# 质量审查 Prompt

```text
检查生成的网站或设计系统的独立性、完整性、可复用性、可实现性、原创性、可访问性、响应式和清理质量。

检查：
- color、typography、spacing、radius、shadow、motion、z-index 和 breakpoints 是否存在语义化 token。
- 组件是否包含 anatomy、variants、states、behavior、accessibility、do 和 dont。
- 页面模板是否能替换 site type、density、content、brand 和 conversion goal。
- 文本、图片、图标、class 名和布局签名是否原创且可替换。
- 对比度、键盘、动效、语义、响应式、表单和状态消息是否满足 WCAG 2.2 AA 或更高标准。
- desktop、tablet 和 mobile 布局是否避免重叠和水平滚动。
- prompt block 是否可独立使用，且不需要外部页面知识。

先返回 findings，再返回 required fixes，最后给出 concise readiness verdict。
```

## Verdict Labels

- `ready`：无阻塞问题。
- `revise`：发布前需要修正。
- `blocked`：缺少关键结构、可访问性或原创性保护。

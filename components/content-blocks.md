# 内容区块

## HeroSection

```yaml
name: "HeroSection"
purpose: "建立身份、产品主张或页面语境。"
anatomy:
  - "headline"
  - "supporting copy"
  - "primary action"
  - "secondary action or trust signal"
  - "optional media or interactive surface"
variants:
  - "centered"
  - "editorial"
  - "product"
  - "search_first"
  - "profile"
states:
  - default
  - hover
  - focus
  - active
  - disabled
  - loading
  - error
  - selected
tokens_used:
  - "typography.display_lg"
  - "spacing.space_16"
  - "color.bg_page"
behavior:
  - "尽可能在首屏露出下一段内容。"
  - "行动按钮靠近价值陈述。"
accessibility:
  - "页面只使用一个 h1。"
do:
  - "首屏必须清楚表达页面用途。"
dont:
  - "不要把 hero 文案放在装饰卡片里。"
```

## SectionHeader

```yaml
name: "SectionHeader"
purpose: "标记内容组并说明其角色。"
anatomy:
  - "label"
  - "heading"
  - "optional count"
  - "optional action"
variants:
  - "compact"
  - "centered"
  - "with_action"
  - "with_counter"
states:
  - default
  - hover
  - focus
  - active
  - disabled
  - loading
  - error
  - selected
tokens_used:
  - "color.action_primary"
  - "typography.h2"
  - "spacing.space_4"
behavior:
  - "动态列表和内容集合可使用计数。"
accessibility:
  - "使用符合页面顺序的 heading level。"
do:
  - "区块标签保持简短。"
dont:
  - "不要无层级地重复同一标题级别。"
```

## TestimonialBlock

```yaml
name: "TestimonialBlock"
purpose: "通过结果或认可提供社会证明。"
anatomy:
  - "quote"
  - "person or role"
  - "context"
  - "optional avatar"
variants:
  - "single"
  - "grid"
  - "carousel"
  - "compact"
states:
  - default
  - hover
  - focus
  - active
  - disabled
  - loading
  - error
  - selected
tokens_used:
  - "color.bg_surface"
  - "typography.body_lg"
  - "radius.radius_lg"
behavior:
  - "只有所有内容都可达时才使用 carousel。"
accessibility:
  - "自动轮播必须有暂停控件。"
do:
  - "使用具体结果。"
dont:
  - "高信任决策中不要使用匿名空泛赞美。"
```

## AuthorBlock

```yaml
name: "AuthorBlock"
purpose: "识别作者、创作者、成员或归属者。"
anatomy:
  - "avatar"
  - "name"
  - "role or handle"
  - "bio"
  - "optional action"
variants:
  - "inline"
  - "card"
  - "profile_header"
states:
  - default
  - hover
  - focus
  - active
  - disabled
  - loading
  - error
  - selected
tokens_used:
  - "radius.radius_full"
  - "typography.body_sm"
  - "color.text_muted"
behavior:
  - "只有有意义时才让名称或头像链接到 profile。"
accessibility:
  - "名称相邻时 avatar alt 为空。"
do:
  - "展示角色或可信信号。"
dont:
  - "不要只靠头像表达身份。"
```

## TableOfContents

```yaml
name: "TableOfContents"
purpose: "帮助用户在长内容中导航。"
anatomy:
  - "title"
  - "anchor list"
  - "active marker"
variants:
  - "sticky"
  - "inline"
  - "collapsible"
states:
  - default
  - hover
  - focus
  - active
  - disabled
  - loading
  - error
  - selected
tokens_used:
  - "color.border_subtle"
  - "color.action_primary"
  - "typography.body_sm"
behavior:
  - "滚动位置变化时高亮当前区块。"
accessibility:
  - "使用带描述标签的 nav landmark。"
do:
  - "最多两级嵌套。"
dont:
  - "不要在小屏遮挡内容。"
```

## CodeBlock

```yaml
name: "CodeBlock"
purpose: "展示命令、代码片段、token 或配置。"
anatomy:
  - "language label"
  - "code content"
  - "optional action"
  - "line wrap control"
variants:
  - "static"
  - "with_action"
  - "highlighted"
states:
  - default
  - hover
  - focus
  - active
  - disabled
  - loading
  - error
  - selected
tokens_used:
  - "font.mono"
  - "color.bg_inverse"
  - "color.text_inverse"
  - "radius.radius_lg"
behavior:
  - "根据内容类型允许水平滚动或换行。"
accessibility:
  - "操作按钮必须播报结果。"
do:
  - "保留缩进。"
dont:
  - "不要把纯说明文字放进 code 样式。"
```

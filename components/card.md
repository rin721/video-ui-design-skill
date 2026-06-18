# 卡片

## Card

```yaml
name: "Card"
purpose: "将相关内容组织为可扫描单元。"
anatomy:
  - "surface"
  - "optional media"
  - "title"
  - "body"
  - "metadata"
  - "action area"
variants:
  - "flat"
  - "elevated"
  - "interactive"
  - "compact"
  - "featured"
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
  - "color.border_subtle"
  - "radius.radius_lg"
  - "shadow.shadow_sm"
behavior:
  - "交互卡片使用单一清晰点击区域或明确内部操作。"
  - "loading 和 error 状态保持尺寸稳定。"
accessibility:
  - "避免嵌套交互冲突。"
  - "卡片开启区块时使用 heading 作为标题。"
do:
  - "使用稳定媒体比例。"
dont:
  - "不要把整页 section 放进卡片壳。"
```

## FeatureCard

```yaml
name: "FeatureCard"
purpose: "解释能力、收益或差异点。"
anatomy:
  - "icon or small media"
  - "headline"
  - "short description"
  - "optional supporting link"
variants:
  - "icon_top"
  - "split"
  - "metric"
  - "proof"
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
  - "color.action_secondary"
  - "color.text_primary"
  - "spacing.space_5"
  - "radius.radius_lg"
behavior:
  - "文案保持简短，并以收益为核心。"
  - "只有卡片可导航或展开时才使用 hover。"
accessibility:
  - "图标无独特含义时视为装饰。"
do:
  - "图标尺度保持一致。"
dont:
  - "不要使用模糊功能标签。"
```

## ContentCard

```yaml
name: "ContentCard"
purpose: "预览文章、帖子、项目、剧集、更新或列表项。"
anatomy:
  - "thumbnail or placeholder"
  - "title"
  - "summary"
  - "metadata row"
  - "category or tag"
variants:
  - "grid"
  - "list"
  - "compact"
  - "editorial"
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
  - "color.text_primary"
  - "color.text_muted"
  - "spacing.space_3"
  - "radius.radius_md"
behavior:
  - "根据密度将标题限制为 2 到 3 行。"
  - "metadata 分组清晰且易读。"
accessibility:
  - "使用描述性标题作为链接文本。"
  - "metadata 以文本呈现。"
do:
  - "使用内容角色，不绑定固定类别名。"
dont:
  - "内部链接冲突时不要让整张卡都可点击。"
```

## MediaCard

```yaml
name: "MediaCard"
purpose: "展示视觉或可播放内容，并附带标题与紧凑 metadata。"
anatomy:
  - "media frame"
  - "duration or status overlay"
  - "title"
  - "creator or owner"
  - "metrics"
variants:
  - "video"
  - "gallery"
  - "audio"
  - "product_media"
  - "placeholder"
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
  - "radius.radius_md"
  - "shadow.shadow_focus"
  - "motion.duration.short"
behavior:
  - "媒体使用固定比例。"
  - "控件只在可用且键盘可达时展示。"
accessibility:
  - "提供 alt 文本或媒体标签。"
  - "不要自动播放声音。"
do:
  - "缺失媒体时使用 placeholder。"
dont:
  - "不要依赖缩略图文字传达关键信息。"
```

## ArticleCard

```yaml
name: "ArticleCard"
purpose: "预览长阅读内容。"
anatomy:
  - "eyebrow"
  - "title"
  - "excerpt"
  - "author"
  - "date or reading time"
variants:
  - "featured"
  - "standard"
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
  - "typography.h3"
  - "typography.body_sm"
  - "color.text_muted"
behavior:
  - "标题作为主链接。"
accessibility:
  - "屏幕阅读顺序与视觉顺序一致。"
do:
  - "使用可读摘要。"
dont:
  - "不要在密集模式下截断所有信号。"
```

## ProductCard

```yaml
name: "ProductCard"
purpose: "支持商品发现与比较。"
anatomy:
  - "product media"
  - "name"
  - "price"
  - "rating or trust cue"
  - "primary action"
variants:
  - "grid"
  - "list"
  - "sale"
  - "out_of_stock"
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
  - "color.warning"
  - "radius.radius_lg"
behavior:
  - "价格和可用状态保持可见。"
accessibility:
  - "折扣和库存状态用文本暴露。"
do:
  - "商品媒体比例保持一致。"
dont:
  - "不要把购买必需信息藏在 hover 中。"
```

## DiscussionCard

```yaml
name: "DiscussionCard"
purpose: "预览社区 thread、问题、主题或更新。"
anatomy:
  - "topic title"
  - "author summary"
  - "reply or activity count"
  - "latest activity"
  - "tags"
variants:
  - "thread"
  - "question"
  - "announcement"
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
  - "color.text_muted"
  - "color.action_primary"
  - "radius.radius_lg"
behavior:
  - "按活动、时间或相关性排序。"
accessibility:
  - "标题作为主链接，计数以文本呈现。"
do:
  - "展示参与信号。"
dont:
  - "不要隐藏审核状态。"
```

## MemberAvatar

```yaml
name: "MemberAvatar"
purpose: "在紧凑空间中代表个人、团队或账户。"
anatomy:
  - "avatar image or initials"
  - "status ring"
  - "optional tooltip"
variants:
  - "image"
  - "initials"
  - "stack"
  - "status"
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
  - "color.border_subtle"
  - "color.success"
behavior:
  - "图片不可用时使用 initials fallback。"
accessibility:
  - "相邻已有名称时 avatar alt 为空；否则提供名称。"
do:
  - "状态提示需要文本可达。"
dont:
  - "不要只用颜色识别人。"
```

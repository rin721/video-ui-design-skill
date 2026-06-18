# 组件索引

## Component Schema

每个组件条目使用统一结构：

```yaml
component_schema:
  name: ""
  purpose: ""
  anatomy:
    - ""
  variants:
    - ""
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
    - ""
  behavior:
    - ""
  accessibility:
    - ""
  do:
    - ""
  dont:
    - ""
```

## Required Components

- Button
- Link
- NavigationBar
- MobileMenu
- HeroSection
- SectionHeader
- Card
- FeatureCard
- ContentCard
- MediaCard
- FormField
- SearchInput
- Tag
- Badge
- Alert
- Modal
- Dropdown
- Tabs
- Accordion
- PricingBlock
- TestimonialBlock
- CTASection
- Footer

## Conditional Components

- Blog：ArticleCard、AuthorBlock、TableOfContents、NewsletterBlock。
- Community：DiscussionCard、MemberAvatar、ActivityFeed、ReactionButton。
- Ecommerce：ProductCard、VariantSelector、CartSummary、CheckoutStep。
- Dashboard：Sidebar、MetricCard、DataTable、EmptyState、CommandPalette。
- Documentation：SidebarTree、CodeBlock、Callout、PaginationNav。

## State Rules

- `default`：布局稳定，不产生内容跳动。
- `hover`：使用柔和背景或阴影增强。
- `focus`：至少 3:1 UI 对比度的可见 ring 或 outline。
- `active`：即时按压反馈，不改变布局。
- `disabled`：明确不可用，并有文字或结构提示。
- `loading`：保留尺寸，用 spinner、skeleton 或进度文本替代内容。
- `error`：结合颜色、图标或标签，并提供恢复说明。
- `selected`：使用 active marker 与可访问状态。

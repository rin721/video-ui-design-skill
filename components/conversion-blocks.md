# 转化区块

## PricingBlock

```yaml
name: "PricingBlock"
purpose: "比较计划、套餐、等级或购买选项。"
anatomy:
  - "plan name"
  - "price"
  - "billing note"
  - "feature list"
  - "primary action"
  - "highlight marker"
variants:
  - "single"
  - "three_tier"
  - "comparison_table"
  - "usage_based"
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
  - "color.action_primary"
  - "radius.radius_lg"
  - "shadow.shadow_md"
behavior:
  - "只有能提供决策帮助时才高亮推荐计划。"
  - "计费条款靠近价格展示。"
accessibility:
  - "使用 list 或 table 语义。"
do:
  - "让差异易于比较。"
dont:
  - "不要隐藏费用或限制。"
```

## CTASection

```yaml
name: "CTASection"
purpose: "引导用户进行下一个有意义的操作。"
anatomy:
  - "heading"
  - "short copy"
  - "primary action"
  - "secondary action"
  - "trust or reassurance line"
variants:
  - "inline"
  - "band"
  - "footer"
  - "modal"
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
  - "color.bg_surface"
  - "spacing.space_12"
behavior:
  - "放在证明内容或任务完成后。"
  - "只使用一个主操作。"
accessibility:
  - "操作标签必须描述结果。"
do:
  - "文案短而具体。"
dont:
  - "不要用重复 CTA 打断阅读。"
```

## Footer

```yaml
name: "Footer"
purpose: "提供收束、次级导航、法律信息和支持路径。"
anatomy:
  - "brand or product label"
  - "link groups"
  - "contact or support"
  - "legal text"
  - "optional newsletter"
variants:
  - "simple"
  - "multi_column"
  - "product"
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
  - "color.bg_surface"
  - "color.text_muted"
  - "spacing.space_16"
behavior:
  - "只承载次级导航。"
accessibility:
  - "使用 footer landmark。"
do:
  - "按用户意图分组链接。"
dont:
  - "不要无目的重复整套主导航。"
```

## NewsletterBlock

```yaml
name: "NewsletterBlock"
purpose: "通过邮件或通知邀请重复访问。"
anatomy:
  - "heading"
  - "benefit copy"
  - "email field"
  - "submit button"
  - "privacy note"
variants:
  - "inline"
  - "sidebar"
  - "footer"
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
  - "color.border_subtle"
  - "radius.radius_lg"
behavior:
  - "成功状态在原位置展示，不清空语境。"
accessibility:
  - "标注 email 字段并播报提交状态。"
do:
  - "说明预期频率。"
dont:
  - "不要默认勾选同意。"
```

## CartSummary

```yaml
name: "CartSummary"
purpose: "汇总已选商品、总价、折扣和下一步。"
anatomy:
  - "item list"
  - "subtotal"
  - "discounts"
  - "shipping or fees"
  - "total"
  - "checkout action"
variants:
  - "sidebar"
  - "drawer"
  - "checkout"
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
  - "color.bg_surface_elevated"
  - "shadow.shadow_md"
  - "radius.radius_lg"
behavior:
  - "数量变化后立即更新总价。"
accessibility:
  - "礼貌播报总价变化。"
do:
  - "展示所有费用类别。"
dont:
  - "不要用隐藏费用制造意外。"
```

## MetricCard

```yaml
name: "MetricCard"
purpose: "展示简洁 KPI、趋势或状态信号。"
anatomy:
  - "label"
  - "value"
  - "trend"
  - "supporting note"
variants:
  - "standard"
  - "trend"
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
  - "typography.h2"
  - "typography.caption"
  - "color.success"
  - "color.danger"
behavior:
  - "loading 时使用 skeleton value。"
accessibility:
  - "趋势必须有文字，不只用箭头或颜色。"
do:
  - "数字格式保持稳定。"
dont:
  - "不要把无关指标混入一张卡。"
```

## DataTable

```yaml
name: "DataTable"
purpose: "展示可扫描、排序和操作的结构化记录。"
anatomy:
  - "caption"
  - "header row"
  - "body rows"
  - "row actions"
  - "pagination"
variants:
  - "compact"
  - "comfortable"
  - "selectable"
  - "sortable"
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
  - "typography.body_sm"
  - "spacing.space_3"
behavior:
  - "排序和 loading 时保持列稳定。"
accessibility:
  - "表格数据使用 table 语义。"
  - "暴露排序方向。"
do:
  - "在表格区域内提供空状态和错误状态。"
dont:
  - "不要用 table 做卡片布局。"
```

## CommandPalette

```yaml
name: "CommandPalette"
purpose: "提供快速键盘导航和操作入口。"
anatomy:
  - "dialog"
  - "search input"
  - "result list"
  - "shortcut hint"
  - "empty state"
variants:
  - "global"
  - "scoped"
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
  - "shadow.shadow_lg"
  - "zIndex.z_modal"
behavior:
  - "用快捷键打开，Escape 关闭。"
  - "方向键选择结果。"
accessibility:
  - "一致使用 combobox 或 dialog 模式。"
do:
  - "优先展示高频操作。"
dont:
  - "危险操作必须确认后执行。"
```

## Sidebar

```yaml
name: "Sidebar"
purpose: "承载次级导航、筛选或上下文工具。"
anatomy:
  - "container"
  - "section groups"
  - "items"
  - "active marker"
variants:
  - "fixed"
  - "collapsible"
  - "filter"
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
  - "color.bg_surface_elevated"
  - "color.border_subtle"
  - "zIndex.z_sticky"
behavior:
  - "低于 tablet 宽度时折叠。"
accessibility:
  - "根据用途使用 nav 或 complementary landmark。"
do:
  - "active 位置保持可见。"
dont:
  - "不要把筛选和导航拥挤混放。"
```

## SidebarTree

```yaml
name: "SidebarTree"
purpose: "导航嵌套文档或结构化内容。"
anatomy:
  - "tree root"
  - "tree item"
  - "expand control"
  - "active marker"
variants:
  - "docs"
  - "knowledge_base"
  - "file_like"
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
  - "typography.body_sm"
  - "spacing.space_2"
behavior:
  - "尽可能保留已展开分支。"
accessibility:
  - "只有实现键盘行为时才使用 tree 语义。"
do:
  - "限制嵌套深度。"
dont:
  - "树很大时不要隐藏搜索。"
```

## Callout

```yaml
name: "Callout"
purpose: "突出重要 note、tip、warning 或 requirement。"
anatomy:
  - "icon"
  - "title"
  - "body"
variants:
  - "note"
  - "tip"
  - "warning"
  - "danger"
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
  - "color.info"
  - "color.warning"
  - "color.danger"
  - "radius.radius_lg"
behavior:
  - "靠近相关内容。"
accessibility:
  - "callout 类型使用文本标签。"
do:
  - "克制使用。"
dont:
  - "不要把普通段落都做成 callout。"
```

## PaginationNav

```yaml
name: "PaginationNav"
purpose: "在结果页或相邻文档间移动。"
anatomy:
  - "previous action"
  - "next action"
  - "page list or labels"
variants:
  - "numbered"
  - "previous_next"
  - "document"
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
  - "radius.radius_md"
behavior:
  - "不可用方向置为 disabled。"
accessibility:
  - "使用带描述标签的 nav landmark。"
do:
  - "暴露当前页。"
dont:
  - "不要只用箭头而无标签。"
```

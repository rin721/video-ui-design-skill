# Conversion Blocks

## PricingBlock

```yaml
name: "PricingBlock"
purpose: "Compare plans, packages, tiers, or purchase options."
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
  - "Highlight one recommended plan only when guidance is helpful."
  - "Keep billing terms visible near price."
accessibility:
  - "Use lists or tables with proper semantics."
do:
  - "Make differences easy to compare."
dont:
  - "Do not hide fees or limits."
```

## CTASection

```yaml
name: "CTASection"
purpose: "Move users toward the next meaningful action."
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
  - "Place after proof or task completion."
  - "Use one primary action."
accessibility:
  - "Action labels must describe the result."
do:
  - "Keep copy short and concrete."
dont:
  - "Do not interrupt reading with repeated CTA blocks."
```

## Footer

```yaml
name: "Footer"
purpose: "Provide closure, secondary navigation, legal items, and support paths."
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
  - "Use secondary navigation only."
accessibility:
  - "Use footer landmark."
do:
  - "Group links by user intent."
dont:
  - "Do not repeat the entire primary navigation without purpose."
```

## NewsletterBlock

```yaml
name: "NewsletterBlock"
purpose: "Invite repeat engagement through email or notifications."
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
  - "Show success in place without clearing context."
accessibility:
  - "Label the email field and announce submission status."
do:
  - "State expected cadence."
dont:
  - "Do not pre-check consent."
```

## CartSummary

```yaml
name: "CartSummary"
purpose: "Summarize selected items, totals, discounts, and next action."
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
  - "Update totals immediately after quantity changes."
accessibility:
  - "Announce total changes politely."
do:
  - "Show all cost categories."
dont:
  - "Do not surprise users with hidden charges."
```

## MetricCard

```yaml
name: "MetricCard"
purpose: "Show a concise KPI, trend, or status signal."
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
  - "Use skeleton values while loading."
accessibility:
  - "Trend must include text, not only arrow or color."
do:
  - "Use stable number formatting."
dont:
  - "Do not mix unrelated metrics in one card."
```

## DataTable

```yaml
name: "DataTable"
purpose: "Display structured records for scanning, sorting, and action."
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
  - "Keep columns stable when sorting and loading."
accessibility:
  - "Use table semantics for tabular data."
  - "Expose sort direction."
do:
  - "Provide empty and error states inside the table region."
dont:
  - "Do not use tables for card layouts."
```

## CommandPalette

```yaml
name: "CommandPalette"
purpose: "Provide fast keyboard access to navigation and actions."
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
  - "Open with keyboard shortcut and close with escape."
  - "Arrow keys select results."
accessibility:
  - "Use combobox or dialog patterns consistently."
do:
  - "Prioritize frequent actions."
dont:
  - "Do not expose unsafe actions without confirmation."
```

## Sidebar

```yaml
name: "Sidebar"
purpose: "Hold secondary navigation, filters, or contextual tools."
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
  - "Collapse below tablet width."
accessibility:
  - "Use nav or complementary landmark according to purpose."
do:
  - "Keep active position visible."
dont:
  - "Do not crowd filters and navigation together."
```

## SidebarTree

```yaml
name: "SidebarTree"
purpose: "Navigate nested documentation or structured content."
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
  - "Persist expanded branches when possible."
accessibility:
  - "Use tree semantics only when keyboard behavior is implemented."
do:
  - "Limit nesting depth."
dont:
  - "Do not hide search when the tree is large."
```

## Callout

```yaml
name: "Callout"
purpose: "Highlight important notes, tips, warnings, or requirements."
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
  - "Stay near the related content."
accessibility:
  - "Use text labels for callout type."
do:
  - "Use sparingly."
dont:
  - "Do not use callouts for ordinary paragraphs."
```

## PaginationNav

```yaml
name: "PaginationNav"
purpose: "Move between result pages or adjacent documents."
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
  - "Disable unavailable directions."
accessibility:
  - "Use nav landmark with descriptive label."
do:
  - "Expose current page."
dont:
  - "Do not rely on arrows without labels."
```

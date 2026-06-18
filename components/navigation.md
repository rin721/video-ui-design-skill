# 导航

## NavigationBar

```yaml
name: "NavigationBar"
purpose: "提供持久定位和主要目的地。"
anatomy:
  - "brand area"
  - "primary links"
  - "utility actions"
  - "active indicator"
variants:
  - "top"
  - "side_rail"
  - "hybrid"
  - "transparent"
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
  - "color.action_primary"
  - "color.border_subtle"
  - "shadow.shadow_md"
  - "zIndex.z_sticky"
behavior:
  - "宽泛营销页面使用 top navigation。"
  - "重复 app 或媒体操作使用 side rail。"
  - "低于 tablet 宽度时折叠为 mobile menu 或 bottom navigation。"
accessibility:
  - "使用 nav landmark。"
  - "当前目的地设置 aria-current。"
  - "图标提供可见标签或可访问名称。"
do:
  - "primary items 不超过 7 个。"
dont:
  - "不要把无关工具混入 primary link group。"
```

## MobileMenu

```yaml
name: "MobileMenu"
purpose: "在紧凑屏幕中展示导航和工具操作。"
anatomy:
  - "trigger"
  - "panel or bottom bar"
  - "destination list"
  - "utility actions"
  - "dismiss control"
variants:
  - "bottom_nav"
  - "drawer"
  - "sheet"
  - "overflow_menu"
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
  - "color.overlay"
  - "radius.radius_lg"
  - "shadow.shadow_lg"
  - "zIndex.z_modal"
behavior:
  - "modal drawer 内需要 trap focus。"
  - "Escape 和 dismiss control 可关闭。"
  - "bottom navigation 只承载一级高频目的地。"
accessibility:
  - "trigger 需要暴露 expanded 状态。"
  - "关闭后 focus 回到 trigger。"
do:
  - "移动端目的地保持可预测。"
dont:
  - "搜索或账户是主任务时不要隐藏。"
```

## Dropdown

```yaml
name: "Dropdown"
purpose: "展示紧凑操作、筛选或目的地列表。"
anatomy:
  - "trigger"
  - "menu surface"
  - "menu item"
  - "optional divider"
variants:
  - "action_menu"
  - "select_menu"
  - "filter_menu"
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
  - "shadow.shadow_md"
  - "zIndex.z_dropdown"
behavior:
  - "点击或键盘命令打开。"
  - "方向键在项目间移动。"
  - "Escape 关闭菜单。"
accessibility:
  - "命令菜单才使用 menu 语义。"
  - "值选择使用 listbox 语义。"
do:
  - "将破坏性操作与常用操作分组隔开。"
dont:
  - "不要把关键导航藏入 dropdown。"
```

## Tabs

```yaml
name: "Tabs"
purpose: "在同页切换同级内容组。"
anatomy:
  - "tablist"
  - "tab"
  - "active indicator"
  - "tabpanel"
variants:
  - "underline"
  - "segmented"
  - "icon_label"
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
  - "color.border_subtle"
  - "spacing.space_3"
  - "motion.duration.short"
behavior:
  - "Tabs 切换局部内容并保留页面语境。"
  - "简单 tab 切换不触发整页重新加载。"
accessibility:
  - "使用 tab、tablist 和 tabpanel roles。"
  - "支持方向键导航。"
do:
  - "标签保持短。"
dont:
  - "不要用 tabs 表达顺序步骤。"
```

## Accordion

```yaml
name: "Accordion"
purpose: "压缩可选细节，同时保持可扫描。"
anatomy:
  - "header button"
  - "title"
  - "indicator icon"
  - "content region"
variants:
  - "single_open"
  - "multi_open"
  - "bordered"
  - "flush"
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
  - "color.bg_surface"
  - "radius.radius_md"
  - "motion.duration.short"
behavior:
  - "使用 button 语义切换内容。"
  - "未请求减少动效时可使用高度动画。"
accessibility:
  - "button 通过 aria-controls 连接 panel。"
  - "暴露 expanded 状态。"
do:
  - "用于 FAQ、设置和密集细节。"
dont:
  - "不要隐藏核心转化信息。"
```

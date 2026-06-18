# 按钮与链接

## Button

```yaml
name: "Button"
purpose: "触发明确操作。"
anatomy:
  - "container"
  - "label"
  - "optional leading icon"
  - "optional trailing icon"
variants:
  - "primary"
  - "secondary"
  - "ghost"
  - "danger"
  - "icon"
  - "pill"
  - "full_width"
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
  - "color.action_primary_hover"
  - "color.focus_ring"
  - "spacing.space_2"
  - "spacing.space_4"
  - "radius.radius_md"
  - "radius.radius_full"
  - "shadow.shadow_focus"
behavior:
  - "桌面端高度至少 36px，触控设备至少 44px。"
  - "loading 时保留按钮宽度。"
  - "icon-only 变体只用于熟悉且重复出现的操作。"
accessibility:
  - "操作使用原生 button 元素。"
  - "icon-only 按钮必须提供可访问名称。"
  - "操作等待中使用 aria-busy。"
do:
  - "每个操作组只使用一个 primary button。"
  - "标签使用动词。"
dont:
  - "不要把 primary 色用于破坏性操作。"
  - "不要隐藏 focus 样式。"
```

## Link

```yaml
name: "Link"
purpose: "导航到页面、区块、文件或外部目的地。"
anatomy:
  - "text label"
  - "optional icon"
  - "optional underline or active marker"
variants:
  - "inline"
  - "nav"
  - "standalone"
  - "muted"
  - "external"
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
  - "color.text_primary"
  - "color.text_muted"
  - "color.focus_ring"
  - "motion.duration.short"
behavior:
  - "inline link 在 hover 和 focus 时显示下划线。"
  - "导航 link 在 active 时使用 selected marker 和 aria-current。"
accessibility:
  - "使用带有效 href 的 anchor。"
  - "清楚描述目的地。"
do:
  - "使用简洁目的地标签。"
  - "让 inline link 与周围文本可区分。"
dont:
  - "不要用 link 执行表单提交或 modal 命令。"
```

## Tag

```yaml
name: "Tag"
purpose: "为内容标记类别、主题、筛选或 metadata。"
anatomy:
  - "container"
  - "label"
  - "optional remove icon"
variants:
  - "neutral"
  - "brand"
  - "accent"
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
  - "color.bg_surface"
  - "color.border_subtle"
  - "color.action_secondary"
  - "radius.radius_full"
behavior:
  - "可选择 tag 切换 selected 状态。"
  - "可移除 tag 需要独立 remove 控件。"
accessibility:
  - "toggle tag 使用 aria-pressed。"
  - "remove 控件名称包含 tag label。"
do:
  - "标签保持短。"
dont:
  - "类别有层级时不要用 tag 替代主导航。"
```

## Badge

```yaml
name: "Badge"
purpose: "展示紧凑计数、状态或新鲜度标记。"
anatomy:
  - "container"
  - "short label or number"
variants:
  - "count"
  - "status"
  - "new"
  - "outline"
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
  - "color.text_inverse"
  - "radius.radius_sm"
  - "spacing.space_1"
behavior:
  - "Badge 通常是被动信息。"
  - "交互式 badge 遵循 button 或 tag 语义。"
accessibility:
  - "状态必须有文字，不只靠颜色。"
do:
  - "用于紧凑强调。"
dont:
  - "不要放入长句。"
```

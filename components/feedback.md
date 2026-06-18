# 反馈与浮层

## Alert

```yaml
name: "Alert"
purpose: "传达状态、警告、错误或成功信息。"
anatomy:
  - "icon"
  - "title"
  - "message"
  - "optional action"
  - "optional dismiss"
variants:
  - "info"
  - "success"
  - "warning"
  - "danger"
  - "inline"
  - "toast"
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
  - "color.success"
  - "color.warning"
  - "color.danger"
  - "radius.radius_lg"
behavior:
  - "inline alert 保持在受影响内容附近。"
  - "toast 只对非关键消息自动消失。"
accessibility:
  - "状态使用 aria-live polite，紧急错误使用 assertive。"
  - "除颜色外必须有文本。"
do:
  - "错误提供恢复操作。"
dont:
  - "不要堆叠大量无法管理的 toast。"
```

## Modal

```yaml
name: "Modal"
purpose: "在页面上方请求聚焦操作或确认。"
anatomy:
  - "overlay"
  - "dialog surface"
  - "title"
  - "content"
  - "actions"
  - "dismiss control"
variants:
  - "confirmation"
  - "form"
  - "media"
  - "drawer"
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
  - "color.overlay"
  - "color.bg_surface"
  - "shadow.shadow_lg"
  - "zIndex.z_modal"
behavior:
  - "打开时 trap focus。"
  - "Escape 可关闭，破坏性操作处理中除外。"
  - "关闭后 focus 回到打开控件。"
accessibility:
  - "使用带标题关联的 dialog 语义。"
  - "键盘导航保持在 dialog 内。"
do:
  - "操作标签简洁。"
dont:
  - "不要用 modal 承载日常导航。"
```

## EmptyState

```yaml
name: "EmptyState"
purpose: "说明内容缺失原因并提供下一步。"
anatomy:
  - "small visual or icon"
  - "title"
  - "message"
  - "primary action"
  - "optional secondary action"
variants:
  - "first_use"
  - "no_results"
  - "filtered_out"
  - "permission_limited"
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
  - "color.text_muted"
  - "color.action_secondary"
  - "spacing.space_8"
behavior:
  - "提供创建、清除筛选、重试或学习下一步的路径。"
accessibility:
  - "使用清晰文字，不让装饰承担含义。"
do:
  - "信息与任务具体相关。"
dont:
  - "不要责备用户。"
```

## ActivityFeed

```yaml
name: "ActivityFeed"
purpose: "展示社区、系统或内容的最近更新。"
anatomy:
  - "feed list"
  - "activity item"
  - "actor"
  - "verb"
  - "object"
  - "timestamp"
variants:
  - "compact"
  - "detailed"
  - "grouped"
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
  - "高密度时合并重复事件。"
accessibility:
  - "根据时间顺序重要性选择有序或无序列表。"
do:
  - "时间戳保持可读。"
dont:
  - "不要默认播报所有实时更新。"
```

## ReactionButton

```yaml
name: "ReactionButton"
purpose: "捕捉轻量反馈，如喜欢、收藏、投票或确认。"
anatomy:
  - "icon"
  - "optional count"
  - "selected marker"
variants:
  - "icon"
  - "icon_count"
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
  - "color.action_primary"
  - "radius.radius_full"
  - "shadow.shadow_focus"
behavior:
  - "立即切换 selected 状态，失败时用 alert 回滚或解释。"
accessibility:
  - "在可访问名称中暴露 pressed 状态和计数。"
do:
  - "使用熟悉图标。"
dont:
  - "不要让计数改变按钮宽度。"
```

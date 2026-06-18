# Feedback And Overlays

## Alert

```yaml
name: "Alert"
purpose: "Communicate status, warning, error, or success information."
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
  - "Inline alerts remain near the affected content."
  - "Toast alerts auto-dismiss only for non-critical messages."
accessibility:
  - "Use aria-live polite for status and assertive for urgent errors."
  - "Include text in addition to color."
do:
  - "Provide recovery action for errors."
dont:
  - "Do not stack many toasts without controls."
```

## Modal

```yaml
name: "Modal"
purpose: "Request focused action or confirmation over the page."
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
  - "Trap focus while open."
  - "Close on escape unless a destructive operation is pending."
  - "Return focus to opener."
accessibility:
  - "Use dialog semantics with labelled title."
  - "Keep keyboard navigation inside dialog."
do:
  - "Use concise action labels."
dont:
  - "Do not use modal for routine navigation."
```

## EmptyState

```yaml
name: "EmptyState"
purpose: "Explain why content is absent and offer a next step."
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
  - "Provide a way to create, clear filters, retry, or learn next steps."
accessibility:
  - "Use clear text and avoid decorative-only meaning."
do:
  - "Keep message specific to the task."
dont:
  - "Do not blame the user."
```

## ActivityFeed

```yaml
name: "ActivityFeed"
purpose: "Show recent community, system, or content updates."
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
  - "Group repetitive events when density is high."
accessibility:
  - "Use ordered or unordered lists according to chronology importance."
do:
  - "Keep timestamps readable."
dont:
  - "Do not announce every live update unless requested."
```

## ReactionButton

```yaml
name: "ReactionButton"
purpose: "Capture lightweight feedback such as like, save, vote, or acknowledge."
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
  - "Toggle selected state immediately, then reconcile failures with an alert."
accessibility:
  - "Expose pressed state and count in the accessible name."
do:
  - "Use familiar icons."
dont:
  - "Do not make counts shift button width."
```

# Button And Link

## Button

```yaml
name: "Button"
purpose: "Trigger a clear action."
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
  - "Keep height at 36px minimum on desktop and 44px minimum on touch devices."
  - "Preserve width during loading."
  - "Use icon-only variant only for familiar repeated actions."
accessibility:
  - "Use native button element for actions."
  - "Provide accessible names for icon-only buttons."
  - "Expose loading with aria-busy when action is pending."
do:
  - "Use one primary button per action group."
  - "Use verbs for labels."
dont:
  - "Do not use primary color for destructive actions."
  - "Do not hide focus styles."
```

## Link

```yaml
name: "Link"
purpose: "Navigate to another page, section, file, or external destination."
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
  - "Inline links underline on hover and focus."
  - "Navigation links use selected marker and aria-current when active."
accessibility:
  - "Use anchor element with valid href."
  - "Describe destination clearly."
do:
  - "Use concise destination labels."
  - "Differentiate inline links from surrounding text."
dont:
  - "Do not use links for form submission or modal commands."
```

## Tag

```yaml
name: "Tag"
purpose: "Label content with a category, topic, filter, or metadata term."
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
  - "Selectable tags toggle selected state."
  - "Removable tags expose a separate remove control."
accessibility:
  - "Use aria-pressed for toggle tags."
  - "Name remove controls with the tag label."
do:
  - "Keep labels short."
dont:
  - "Do not use tags as primary navigation when categories need hierarchy."
```

## Badge

```yaml
name: "Badge"
purpose: "Show compact counts, status, or novelty markers."
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
  - "Badges are usually passive."
  - "Interactive badges follow button or tag semantics."
accessibility:
  - "Include text, not color-only status."
do:
  - "Use for compact emphasis."
dont:
  - "Do not overload badges with long phrases."
```

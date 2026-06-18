# Navigation

## NavigationBar

```yaml
name: "NavigationBar"
purpose: "Provide persistent orientation and primary destinations."
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
  - "Use top navigation for broad marketing pages."
  - "Use side rail for repeated app or media actions."
  - "Collapse into mobile menu or bottom navigation below tablet width."
accessibility:
  - "Use nav landmark."
  - "Set aria-current for current destination."
  - "Provide visible labels or accessible names for icons."
do:
  - "Limit primary items to 7 or fewer."
dont:
  - "Do not mix unrelated utilities into the primary link group."
```

## MobileMenu

```yaml
name: "MobileMenu"
purpose: "Expose navigation and utilities on compact screens."
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
  - "Trap focus in modal drawers."
  - "Close on escape and dismiss control."
  - "Keep bottom navigation visible only for top-level destinations."
accessibility:
  - "Announce expanded state on trigger."
  - "Restore focus to trigger after close."
do:
  - "Keep mobile destinations predictable."
dont:
  - "Do not hide account or search when they are primary tasks."
```

## Dropdown

```yaml
name: "Dropdown"
purpose: "Reveal a compact list of actions, filters, or destinations."
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
  - "Open on click or keyboard command."
  - "Arrow keys move through items."
  - "Escape closes menu."
accessibility:
  - "Use menu semantics only for command menus."
  - "Use listbox semantics for value selection."
do:
  - "Group destructive actions away from common actions."
dont:
  - "Do not bury critical navigation in a dropdown."
```

## Tabs

```yaml
name: "Tabs"
purpose: "Switch between peer content groups without leaving the page."
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
  - "Tabs switch local content and preserve page context."
  - "Do not reload full pages for simple tab changes."
accessibility:
  - "Use tab, tablist, and tabpanel roles."
  - "Support arrow key navigation."
do:
  - "Keep labels short."
dont:
  - "Do not use tabs for sequential steps."
```

## Accordion

```yaml
name: "Accordion"
purpose: "Compress optional details while preserving scanability."
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
  - "Toggle content with button semantics."
  - "Animate height only when reduced motion is not requested."
accessibility:
  - "Connect button to panel with aria-controls."
  - "Expose expanded state."
do:
  - "Use for FAQs, settings, and dense details."
dont:
  - "Do not hide core conversion information."
```

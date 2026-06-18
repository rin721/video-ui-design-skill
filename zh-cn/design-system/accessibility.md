# Accessibility

## Compliance Goal

Meet WCAG 2.2 AA or better.

```yaml
accessibility:
  contrast:
    body_text: ">= 4.5:1"
    large_text: ">= 3:1"
    non_text_ui: ">= 3:1 where applicable"
  keyboard:
    - all_interactive_elements_focusable
    - visible_focus_state
    - logical_tab_order
  motion:
    - respects_prefers_reduced_motion
    - no_required_motion_only_feedback
  semantics:
    - landmark_structure
    - heading_order
    - form_labeling
    - button_link_semantics
  responsive:
    - tap_area_minimum
    - mobile_readability
    - no_horizontal_scroll
  content:
    - clear_error_messages
    - meaningful_empty_states
    - accessible_alt_text_rules
```

## Required Practices

- Use one `main` landmark per page.
- Keep headings in logical order.
- Use buttons for actions and links for navigation.
- Give icon-only controls an accessible name.
- Provide visible focus styles using `shadow_focus` or an equivalent outline.
- Set tap areas to at least `44px` square on mobile.
- Use `aria-live="polite"` for asynchronous success, loading, and error updates.
- Provide form labels that remain available when a field is filled.
- Respect `prefers-reduced-motion`.

## Text Alternatives

- Decorative imagery uses empty alt text.
- Informational media describes purpose, not visual trivia.
- Product and content thumbnails describe the item category and meaningful subject.
- Icons inside labeled buttons do not need duplicate labels.

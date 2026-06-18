# Layout System

## Layout Tokens

```yaml
layout_system:
  container:
    max_width_desktop: "80rem"
    max_width_tablet: "56rem"
    max_width_mobile: "100%"
    horizontal_padding:
      desktop: "3rem"
      tablet: "2rem"
      mobile: "1rem"
  grid:
    desktop_columns: "12"
    tablet_columns: "8"
    mobile_columns: "4"
    gutter:
      desktop: "1.5rem"
      tablet: "1.25rem"
      mobile: "1rem"
  section_rhythm:
    hero_to_section: "4rem to 5rem"
    section_to_section: "3rem to 4rem"
    dense_block_gap: "1rem to 1.5rem"
    card_grid_gap: "1rem to 1.5rem"
  visual_flow:
    primary_scan_path: "context header, section marker, content grid, action"
    emphasis_strategy: "single bright action with soft active markers"
    content_reveal_order: "identity, navigation, content clusters, proof, conversion"
  responsive_behavior:
    desktop: "side utility rail or top navigation plus 4 to 5 content columns"
    tablet: "top or side navigation plus 2 to 3 content columns"
    mobile: "top brand row, bottom or drawer navigation, 1 to 2 content columns"
```

## Shell Rules

- Use a fixed utility rail on wide screens only when actions repeat across pages.
- Use a top app bar for identity, search, or account context.
- Use a bottom navigation bar on mobile when primary destinations are frequent.
- Reserve center pages for search, onboarding, login, signup, and empty states.
- Use right-side support panels only when the main content remains at least `60 percent` of available width.

## Grid Rules

- Use `repeat(auto-fit, minmax(14rem, 1fr))` for media and content cards.
- Use fixed aspect ratios for media: `16 / 9`, `4 / 3`, `1 / 1`, or `3 / 4`.
- Keep grid item dimensions stable across hover, loading, and error states.
- Prevent horizontal overflow by using `min-width: 0` on text containers.

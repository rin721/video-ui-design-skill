# Accessibility Checklist

## Contrast

- Body text contrast is at least `4.5:1`.
- Large text contrast is at least `3:1`.
- UI boundaries and focus indicators meet `3:1` where applicable.
- Status colors are paired with icon, text, or structure.

## Keyboard

- All interactive elements are keyboard reachable.
- Focus order follows visual and task order.
- Focus state is visible on every interactive component.
- Menus, modals, tabs, accordions, and command palettes have keyboard behavior.

## Semantics

- Each page has one `main` landmark.
- Navigation uses `nav` with clear labels.
- Footer uses `footer`.
- Headings are ordered.
- Buttons and links use correct elements.
- Tables use table semantics only for tabular data.

## Forms

- Every input has a visible label.
- Helper and error text are connected to controls.
- Errors explain recovery.
- Submission status is announced.

## Motion

- `prefers-reduced-motion` is respected.
- No required feedback is motion-only.
- Auto-advancing content can be paused.

## Responsive

- Tap areas are at least `44px` on mobile.
- Text remains readable without viewport-scaled font sizing.
- No horizontal scroll appears at standard mobile widths.

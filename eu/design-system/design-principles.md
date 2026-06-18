# Design Principles

## Clarity Before Atmosphere

Every section must declare its purpose through hierarchy, grouping, and spacing. Decorative treatments can support mood, but they must never compete with content or controls.

## Soft Emphasis

Use the brand color for active state, primary action, section markers, and focus rings. Keep background accents low opacity so the interface stays readable and replaceable.

## Dense But Breathable

Content-heavy layouts should use compact cards, stable image ratios, and concise metadata. Preserve outer spacing and row rhythm so dense grids remain calm.

## Icon-First Utility

Use icons for repeated navigation and tool actions. Pair icons with accessible labels, tooltips where needed, and clear selected states.

## Token-Driven Implementation

Use semantic tokens for every color, spacing, type, radius, shadow, and motion decision. Primitive tokens can change without rewriting components.

## Safe Responsiveness

Keep fixed navigation dimensions predictable. Constrain grids with minmax rules, stable aspect ratios, and tap areas large enough for mobile.

## Accessible By Default

Meet WCAG 2.2 AA or better through contrast, focus visibility, keyboard reachability, semantic landmarks, text alternatives, reduced motion, and clear error recovery.

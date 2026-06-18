# Quality Review Prompt

```text
Review the generated website or design system for independence, completeness, reusability, implementability, originality, accessibility, responsiveness, and cleanup quality.

Check:
- Semantic tokens exist for color, typography, spacing, radius, shadow, motion, z-index, and breakpoints.
- Components include anatomy, variants, states, behavior, accessibility, do, and dont.
- Page templates can change site type, density, content, brand, and conversion goal.
- Text, imagery, icons, class names, and layout signatures are original and replaceable.
- WCAG 2.2 AA or better is satisfied for contrast, keyboard, motion, semantics, responsive behavior, forms, and status messages.
- Desktop, tablet, and mobile layouts avoid overlap and horizontal scroll.
- Prompt blocks are standalone and do not require external page knowledge.

Return findings first, then required fixes, then a concise readiness verdict.
```

## Verdict Labels

- `ready`: no blocking issues.
- `revise`: fix before shipping.
- `blocked`: missing critical structure, accessibility, or originality safeguards.

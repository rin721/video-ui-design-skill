# Component Generation Prompt

```text
Generate a reusable component using this schema: name, purpose, anatomy, variants, states, tokens_used, behavior, accessibility, do, and dont.

Use semantic tokens for color, typography, spacing, radius, shadow, motion, and z-index. Include default, hover, focus, active, disabled, loading, error, and selected states where the state can occur. Keep dimensions stable across states. Provide keyboard behavior and accessible names for icon-only controls.

The component must be original, replaceable, responsive, and implementable in HTML, CSS, and a component framework. It must not use protected imagery, brand marks, unique class naming, or distinctive visual signatures.
```

## Component Checklist

- Purpose is one sentence.
- Anatomy names structural parts, not visual trivia.
- Variants are useful and mutually understandable.
- States have visual and semantic feedback.
- Token use is semantic.
- Behavior includes keyboard and loading rules where relevant.
- Accessibility includes labels, roles, focus, and reduced motion where relevant.
- Do and dont items prevent common misuse.

# Page Generation Prompt

```text
Generate a complete responsive website page using the Soft Signal Interface design system.

Inputs:
- site_type: [personal_homepage | blog | community | saas | ecommerce | documentation | landing_page]
- content_density: [sparse | balanced | dense]
- conversion_goal: [soft | hard | repeat_engagement | task_completion]
- brand_dimensions: seriousness, warmth, innovation, luxury, playfulness, editorial, technical_depth

Build the page from semantic sections, reusable components, and replaceable assets. Use accessible landmarks, one h1, logical headings, visible focus states, keyboard-safe controls, responsive grids, and 44px mobile tap areas. Keep the first viewport useful. Make the primary action clear without repeating it excessively.

Return implementation-ready structure, token mapping, component list, responsive behavior, and accessibility notes.
```

## Page Rules

- Landing pages require hero, proof, features, conversion, and footer.
- Personal pages require identity, credibility, selected work, writing or projects, contact, and footer.
- Blogs require editorial header, featured article, category navigation, article grid, subscription, and footer.
- Communities require shared purpose, active discussions, member signals, join path, and footer.
- SaaS pages require value, product clarity, proof, pricing or plan path, signup, and footer.
- Ecommerce pages require category browsing, product grid, product details, cart path, and checkout support.
- Documentation requires search, navigation hierarchy, content area, code blocks, callouts, and pagination.

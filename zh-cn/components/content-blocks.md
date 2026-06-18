# Content Blocks

## HeroSection

```yaml
name: "HeroSection"
purpose: "Establish identity, offer, or page context."
anatomy:
  - "headline"
  - "supporting copy"
  - "primary action"
  - "secondary action or trust signal"
  - "optional media or interactive surface"
variants:
  - "centered"
  - "editorial"
  - "product"
  - "search_first"
  - "profile"
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
  - "typography.display_lg"
  - "spacing.space_16"
  - "color.bg_page"
behavior:
  - "Reveal the next section within the first viewport when possible."
  - "Keep actions close to the value statement."
accessibility:
  - "Use a single h1 for the page."
do:
  - "Make the first viewport clearly identify the page purpose."
dont:
  - "Do not place hero text inside a decorative card."
```

## SectionHeader

```yaml
name: "SectionHeader"
purpose: "Mark a content group and explain its role."
anatomy:
  - "label"
  - "heading"
  - "optional count"
  - "optional action"
variants:
  - "compact"
  - "centered"
  - "with_action"
  - "with_counter"
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
  - "typography.h2"
  - "spacing.space_4"
behavior:
  - "Use counters for dynamic lists and content collections."
accessibility:
  - "Use heading level that fits page order."
do:
  - "Keep section labels short."
dont:
  - "Do not repeat the same heading level without hierarchy."
```

## TestimonialBlock

```yaml
name: "TestimonialBlock"
purpose: "Provide social proof with a quoted result or endorsement."
anatomy:
  - "quote"
  - "person or role"
  - "context"
  - "optional avatar"
variants:
  - "single"
  - "grid"
  - "carousel"
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
  - "color.bg_surface"
  - "typography.body_lg"
  - "radius.radius_lg"
behavior:
  - "Use carousel only when all content remains reachable."
accessibility:
  - "Do not auto-advance without pause controls."
do:
  - "Use specific outcomes."
dont:
  - "Do not use anonymous praise for high-trust decisions."
```

## AuthorBlock

```yaml
name: "AuthorBlock"
purpose: "Identify a writer, creator, member, or owner."
anatomy:
  - "avatar"
  - "name"
  - "role or handle"
  - "bio"
  - "optional action"
variants:
  - "inline"
  - "card"
  - "profile_header"
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
  - "radius.radius_full"
  - "typography.body_sm"
  - "color.text_muted"
behavior:
  - "Link name or avatar to profile only when useful."
accessibility:
  - "Avatar alt text should be empty when name is adjacent."
do:
  - "Show role or credibility signal."
dont:
  - "Do not rely on avatar alone for identity."
```

## TableOfContents

```yaml
name: "TableOfContents"
purpose: "Help users navigate long content."
anatomy:
  - "title"
  - "anchor list"
  - "active marker"
variants:
  - "sticky"
  - "inline"
  - "collapsible"
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
  - "color.action_primary"
  - "typography.body_sm"
behavior:
  - "Highlight current section when scroll position changes."
accessibility:
  - "Use nav landmark with descriptive label."
do:
  - "Limit nesting to two levels."
dont:
  - "Do not obscure content on small screens."
```

## CodeBlock

```yaml
name: "CodeBlock"
purpose: "Display commands, snippets, tokens, or configuration."
anatomy:
  - "language label"
  - "code content"
  - "optional action"
  - "line wrap control"
variants:
  - "static"
  - "with_action"
  - "highlighted"
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
  - "font.mono"
  - "color.bg_inverse"
  - "color.text_inverse"
  - "radius.radius_lg"
behavior:
  - "Allow horizontal scroll or wrapping according to content type."
accessibility:
  - "Action buttons must announce result."
do:
  - "Preserve indentation."
dont:
  - "Do not put prose-only content in code styling."
```

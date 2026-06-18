---
name: ui-design-skill
description: Generate original website design systems, semantic tokens, reusable component specifications, page templates, visual asset rules, accessibility guidance, and prompt blocks for personal sites, blogs, communities, SaaS, ecommerce, documentation, portfolios, product pages, brand sites, and marketing experiences.
---

# UI Design Skill

## Purpose

Use this skill to create original website design systems, page templates, component specifications, semantic tokens, responsive rules, visual asset guidance, and front-end generation prompts. The output must be reusable across site types and safe for brand, content, and visual replacement.

## When to Use

Use this skill when generating or refining:

- Personal homepages, portfolios, blogs, and editorial sites.
- Community, media, directory, and content discovery experiences.
- SaaS, product, AI tool, and web app landing pages.
- Ecommerce, pricing, checkout, and product detail pages.
- Documentation, help centers, knowledge bases, and developer portals.
- Multi-page marketing sites and brand systems.

## Inputs

Accept these optional inputs:

- `project_name`: package or skill name.
- `site_type`: `auto`, `personal_homepage`, `blog`, `community`, `saas`, `ecommerce`, `documentation`, or `multi_page`.
- `generation_goal`: intended output such as `design_system`, `page_template`, `component_set`, or `website_prompt`.
- `viewport_modes`: desktop, tablet, mobile.
- `capture_states`: default, hover, focus, active, disabled, loading, empty, error, selected.
- `style_abstraction_level`: low, medium, high.
- `accessibility_level`: compliance goal, default `WCAG_2_2_AA_or_better`.
- `brand_swap_parameters`: seriousness, warmth, innovation, luxury, playfulness, editorial, technical depth.

## Workflow

1. Observe layout, hierarchy, density, controls, states, motion, and responsive behavior.
2. Abstract the visual language into portable rules, not fixed page copies.
3. Normalize values into semantic tokens for color, type, spacing, radius, shadow, motion, z-index, and breakpoints.
4. Define components with anatomy, variants, states, constraints, accessibility, and usage rules.
5. Compose page templates that can change site type, content density, conversion goal, and brand expression.
6. Generate standalone prompt blocks for page, component, style, accessibility, and quality tasks.
7. Clean every artifact so it contains no reused text, images, logos, trademarks, class names, route names, or unique visual signatures.
8. Run quality checks for independence, completeness, implementability, accessibility, responsiveness, and originality.

## Output Contract

Produce a package with:

- `SKILL.md` and `README.md`.
- `design-system/` with overview, principles, tokens, typography, color, spacing, layout, accessibility, and brand expression.
- `components/` with component schemas for navigation, buttons, cards, forms, feedback, content blocks, and conversion blocks.
- `patterns/` with page templates for landing, personal, blog, community, SaaS, ecommerce, and documentation experiences.
- `prompts/` with standalone generation, style swap, component, page, and quality prompts.
- `assets/` with visual asset, icon, and media replacement rules.
- `qa/` with originality, accessibility, responsive, and final cleanup checklists.

## Design Rules

- Use semantic tokens before fixed values.
- Keep the primary palette replaceable and restrict accent color to meaningful emphasis.
- Prefer clear hierarchy, generous breathing room, and dense but scannable content grids.
- Use icon buttons for compact repeated actions and text buttons for clear commands.
- Give every interactive element visible hover, focus, active, disabled, loading, and selected states when applicable.
- Ensure focus states are visible without relying on color alone.
- Keep tap areas at least `44px` on mobile.
- Use responsive grids that collapse from multi-column desktop layouts to readable tablet and mobile layouts.
- Respect `prefers-reduced-motion` and provide non-motion feedback.
- Keep text readable across Chinese, English, numerals, and code-like strings.

## Guardrails

- Do not copy text, images, logos, trademarks, unique icons, route labels, CSS selectors, component names, or visual signatures from any existing product.
- Do not produce pixel-matched layouts or locked measurements that only work for one page.
- Do not require proprietary fonts or assets.
- Do not use color alone for status, validation, or selection.
- Do not make decorative media essential to comprehension.
- Do not include brand identifiers, protected artwork, screenshots, URLs, or artifact traces in final files.

## Usage Examples

Generate a SaaS landing page system:

```yaml
site_type: saas
generation_goal: design_system_and_landing_page
brand_swap_parameters:
  seriousness: medium
  warmth: medium
  innovation: high
  luxury: low
  playfulness: medium
  editorial: low
  technical_depth: medium
```

Generate a blog template set:

```yaml
site_type: blog
generation_goal: page_templates_and_components
content_density: medium_to_dense
accessibility_level: WCAG_2_2_AA_or_better
```

Generate a documentation shell:

```yaml
site_type: documentation
generation_goal: doc_shell_and_prompt_blocks
content_density: dense
brand_swap_parameters:
  seriousness: high
  warmth: low
  technical_depth: high
```

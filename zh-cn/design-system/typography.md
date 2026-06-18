# Typography

## Tokens

```yaml
typography_tokens:
  font_family:
    display: "Inter, ui-sans-serif, system-ui, sans-serif"
    body: "Inter, ui-sans-serif, system-ui, sans-serif"
    mono: "ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
  type_scale:
    display_lg:
      size: "3.75rem"
      line_height: "1.08"
      weight: "700"
      letter_spacing: "0"
    display_md:
      size: "3rem"
      line_height: "1.1"
      weight: "700"
      letter_spacing: "0"
    h1:
      size: "2.25rem"
      line_height: "1.16"
      weight: "700"
      letter_spacing: "0"
    h2:
      size: "1.75rem"
      line_height: "1.22"
      weight: "650"
      letter_spacing: "0"
    h3:
      size: "1.25rem"
      line_height: "1.32"
      weight: "650"
      letter_spacing: "0"
    body_lg:
      size: "1.125rem"
      line_height: "1.65"
      weight: "400"
    body_md:
      size: "1rem"
      line_height: "1.6"
      weight: "400"
    body_sm:
      size: "0.875rem"
      line_height: "1.5"
      weight: "400"
    caption:
      size: "0.75rem"
      line_height: "1.45"
      weight: "500"
    label:
      size: "0.875rem"
      line_height: "1.2"
      weight: "650"
```

## Rules

- Use display styles only for hero identity, major page titles, or high-impact editorial headers.
- Use `h1` through `h3` for page hierarchy and component sections.
- Keep paragraph width between `58ch` and `72ch` for long reading.
- Use `body_sm` and `caption` for metadata; never reduce important labels below `0.75rem`.
- Keep letter spacing at `0` for mixed Chinese, English, numerals, and code-like strings.
- Use mono only for code, commands, tokens, and machine-readable values.

## Modes

```yaml
typography_rules:
  heading_density: "large headings need wide surrounding space; compact panels use h3 or label"
  paragraph_width: "58ch to 72ch for reading; 40ch to 56ch for cards"
  editorial_mode: "slower rhythm, larger h1, wider line height, strong paragraph measure"
  marketing_mode: "display title, short supporting copy, high-contrast action labels"
  dashboard_mode: "compact labels, clear numbers, small captions, no hero-scale type inside panels"
```

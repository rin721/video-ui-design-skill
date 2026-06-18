# Blog Pattern

## Structure

```yaml
blog:
  editorial_header:
    purpose: "define publication theme and reading promise"
  featured_post:
    purpose: "highlight one timely or high-value article"
  category_nav:
    purpose: "support topical discovery"
  post_grid:
    purpose: "show recent and evergreen articles"
  newsletter_cta:
    purpose: "encourage repeat reading"
  footer:
    purpose: "hold archive, policy, social, and contact links"
```

## Layout

- Use editorial rhythm with strong article titles and comfortable line length.
- Use grid cards for discovery and full-width article layout for reading.
- Keep category navigation sticky only when it improves browsing.

## Components

Use `NavigationBar`, `ArticleCard`, `AuthorBlock`, `TableOfContents`, `NewsletterBlock`, `Tag`, and `Footer`.

## Acceptance

- Articles remain readable at `58ch` to `72ch`.
- Metadata supports trust without crowding the card.
- Subscription is available after value has been shown.

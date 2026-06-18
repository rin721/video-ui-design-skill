# Landing Page Pattern

## Structure

```yaml
landing_page:
  global_nav:
    purpose: "orient visitors and expose core destinations"
    density: "compact"
  hero:
    purpose: "state offer, audience, and outcome"
    layout: "centered or full-width with real product, scene, or interactive surface"
  trust_signal:
    purpose: "show concise credibility markers"
  feature_grid:
    purpose: "explain 3 to 6 capabilities or benefits"
  proof_section:
    purpose: "show outcomes, testimonials, metrics, or usage context"
  conversion_cta:
    purpose: "invite trial, demo, signup, purchase, or contact"
  footer:
    purpose: "support secondary navigation and legal closure"
```

## Layout

- Desktop: use 12-column grid, hero centered within `80rem`, feature grid at 3 columns.
- Tablet: use 2-column feature and proof grids.
- Mobile: use single-column hero and stacked content, with primary action near the headline.

## Components

Use `NavigationBar`, `HeroSection`, `SectionHeader`, `FeatureCard`, `TestimonialBlock`, `PricingBlock` when needed, `CTASection`, and `Footer`.

## Acceptance

- One primary action is visually dominant.
- Product or offer is understandable within the first viewport.
- Trust content appears before final conversion.
- Decorative media is replaceable and not required for comprehension.

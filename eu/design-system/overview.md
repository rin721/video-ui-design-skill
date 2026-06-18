# Design System Overview

## Aesthetic Style

```yaml
aesthetic_style:
  style_name: "Soft Signal Interface"
  visual_personality:
    - "lightweight"
    - "friendly"
    - "organized"
    - "content-forward"
    - "quietly expressive"
  mood_keywords:
    - "low noise"
    - "high clarity"
    - "soft energy"
    - "structured warmth"
    - "gentle momentum"
  composition_traits:
    - "fixed utility navigation around a flexible content area"
    - "large first impression area for identity, search, or product context"
    - "dense card grids balanced by generous outer margins"
    - "section labels paired with compact counters or status markers"
    - "primary scan path moves from context to grid to detail"
  surface_traits:
    - "near-white page canvas"
    - "translucent elevated panels when content needs containment"
    - "soft accent wash for active navigation and focus"
    - "thin borders and low shadow depth"
  detail_traits:
    - "rounded media cards"
    - "circle icon controls"
    - "short labels with strong color emphasis"
    - "metadata grouped with small icons or compact text"
  suitable_site_types:
    - personal_homepage
    - blog
    - community
    - saas
    - portfolio
    - ecommerce
    - documentation
  avoid:
    - "heavy chrome"
    - "decorative clutter"
    - "low contrast pastel text"
    - "oversized marketing cards inside operational tools"
    - "single-hue pages without neutral and secondary balance"
```

## System Intent

Build pages that feel approachable, direct, and easy to scan. Use soft color to mark important actions, not to decorate every surface. Keep content cards lightweight so images, titles, and metadata carry the page rhythm.

## Reusable Pattern

Use a persistent navigation layer, a clear content header, a responsive grid or shell, and a visible action path. On compact screens, move primary navigation into a bottom bar or top action row while keeping content in two-column or single-column cards according to available width.

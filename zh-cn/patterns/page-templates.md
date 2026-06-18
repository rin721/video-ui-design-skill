# Page Templates

## Information Architecture

```yaml
information_architecture:
  hierarchy_model:
    level_1: "core value or identity statement"
    level_2: "key features, content, products, or work"
    level_3: "proof, details, examples, trust, or community activity"
    level_4: "action entry or conversion path"
  reading_path:
    - "establish context"
    - "present value"
    - "provide proof"
    - "guide action"
  content_density:
    sparse_mode: "large section spacing, one primary message per viewport, minimal metadata"
    balanced_mode: "clear hero, 2 to 4 content clusters, moderate metadata"
    dense_mode: "compact headings, grids, filters, metadata, and persistent navigation"
  conversion_paths:
    soft_conversion: "follow, subscribe, save, read more, browse, join waitlist"
    hard_conversion: "buy, start trial, book demo, create account, checkout"
    repeat_engagement: "newsletter, feed, saved list, notifications, community participation"
  navigation_rules:
    primary_nav_max_items: "7"
    secondary_nav_usage: "settings, account, filters, support, legal, and deep categories"
    mobile_nav_behavior: "bottom nav for frequent destinations, drawer for broad menus, search visible when discovery is key"
```

## Page Skeletons

```yaml
page_templates:
  landing_page:
    - global_nav
    - hero
    - trust_signal
    - feature_grid
    - proof_section
    - conversion_cta
    - footer
  personal_homepage:
    - intro_hero
    - identity_statement
    - selected_work
    - writing_or_projects
    - contact_cta
    - footer
  blog:
    - editorial_header
    - featured_post
    - category_nav
    - post_grid
    - newsletter_cta
    - footer
  community:
    - community_hero
    - value_statement
    - discussion_highlights
    - member_proof
    - join_cta
    - footer
  documentation:
    - doc_shell
    - sidebar_nav
    - content_area
    - code_or_example_block
    - pagination
  ecommerce:
    - commerce_hero
    - category_grid
    - product_grid
    - product_card
    - cart_cta
```

## Site Type Adapters

```yaml
site_type_adapters:
  personal_homepage:
    priority:
      - identity
      - credibility
      - selected_work
      - contact
    recommended_density: "balanced"
    conversion_goal: "establish_trust_and_invite_contact"
  blog:
    priority:
      - readability
      - content_discovery
      - editorial_rhythm
      - subscription
    recommended_density: "medium_to_dense"
    conversion_goal: "repeat_reading_and_subscription"
  community:
    priority:
      - belonging
      - activity
      - trust
      - participation
    recommended_density: "balanced_to_dense"
    conversion_goal: "join_and_contribute"
  saas:
    priority:
      - value_proposition
      - product_clarity
      - proof
      - signup
    recommended_density: "balanced"
    conversion_goal: "trial_or_demo"
  ecommerce:
    priority:
      - product_discovery
      - comparison
      - confidence
      - purchase
    recommended_density: "dense_but_scannable"
    conversion_goal: "purchase"
  documentation:
    priority:
      - findability
      - readability
      - hierarchy
      - task_completion
    recommended_density: "dense"
    conversion_goal: "successful_task_completion"
```

## Shared Composition Rules

- Begin with a clear purpose statement or task entry.
- Keep primary navigation compact and persistent where repeated actions matter.
- Use grids for discovery and structured shells for reading or task completion.
- Place proof before hard conversion.
- Keep mobile layouts readable with stable card sizes and no horizontal scroll.

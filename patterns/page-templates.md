# 页面模板

## Information Architecture

```yaml
information_architecture:
  hierarchy_model:
    level_1: "核心价值或身份声明"
    level_2: "关键功能、内容、商品或作品"
    level_3: "证明、细节、示例、信任或社区活动"
    level_4: "行动入口或转化路径"
  reading_path:
    - "建立语境"
    - "呈现价值"
    - "提供证明"
    - "引导行动"
  content_density:
    sparse_mode: "宽松区块间距、每屏一个主要信息、最少 metadata"
    balanced_mode: "清晰 hero、2 到 4 个内容簇、适度 metadata"
    dense_mode: "紧凑标题、网格、筛选、metadata 和持久导航"
  conversion_paths:
    soft_conversion: "follow, subscribe, save, read more, browse, join waitlist"
    hard_conversion: "buy, start trial, book demo, create account, checkout"
    repeat_engagement: "newsletter, feed, saved list, notifications, community participation"
  navigation_rules:
    primary_nav_max_items: "7"
    secondary_nav_usage: "settings, account, filters, support, legal, and deep categories"
    mobile_nav_behavior: "高频目的地使用 bottom nav，大菜单使用 drawer，发现任务关键时保持 search 可见"
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

- 以清楚的用途声明或任务入口开始。
- 需要重复操作时，保持主导航紧凑且持久。
- 发现类体验使用网格，阅读或任务完成使用结构化外壳。
- 硬转化前先放置信任内容。
- 移动端保持卡片尺寸稳定，不出现水平滚动。

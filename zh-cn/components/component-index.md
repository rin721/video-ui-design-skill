# Component Index

## Component Schema

Each component entry uses this structure:

```yaml
component_schema:
  name: ""
  purpose: ""
  anatomy:
    - ""
  variants:
    - ""
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
    - ""
  behavior:
    - ""
  accessibility:
    - ""
  do:
    - ""
  dont:
    - ""
```

## Required Components

- Button
- Link
- NavigationBar
- MobileMenu
- HeroSection
- SectionHeader
- Card
- FeatureCard
- ContentCard
- MediaCard
- FormField
- SearchInput
- Tag
- Badge
- Alert
- Modal
- Dropdown
- Tabs
- Accordion
- PricingBlock
- TestimonialBlock
- CTASection
- Footer

## Conditional Components

- Blog: ArticleCard, AuthorBlock, TableOfContents, NewsletterBlock.
- Community: DiscussionCard, MemberAvatar, ActivityFeed, ReactionButton.
- Ecommerce: ProductCard, VariantSelector, CartSummary, CheckoutStep.
- Dashboard: Sidebar, MetricCard, DataTable, EmptyState, CommandPalette.
- Documentation: SidebarTree, CodeBlock, Callout, PaginationNav.

## State Rules

- `default`: stable layout, no content shift.
- `hover`: soft background or shadow increase within token limits.
- `focus`: visible ring or outline with at least 3:1 UI contrast.
- `active`: compressed color or shadow feedback, no layout jump.
- `disabled`: unavailable with clear text or structural cue.
- `loading`: replaces content with spinner, skeleton, or progress text while preserving dimensions.
- `error`: combines color, icon or label, and recovery guidance.
- `selected`: uses active marker plus accessible state.

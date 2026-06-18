# Cards

## Card

```yaml
name: "Card"
purpose: "Group related content into a scannable unit."
anatomy:
  - "surface"
  - "optional media"
  - "title"
  - "body"
  - "metadata"
  - "action area"
variants:
  - "flat"
  - "elevated"
  - "interactive"
  - "compact"
  - "featured"
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
  - "color.border_subtle"
  - "radius.radius_lg"
  - "shadow.shadow_sm"
behavior:
  - "Interactive cards use a single clear click area or explicit inner actions."
  - "Cards preserve dimensions during loading and error states."
accessibility:
  - "Avoid nested interactive conflicts."
  - "Use heading text for card titles when cards start sections."
do:
  - "Use stable media ratios."
dont:
  - "Do not place full page sections inside card shells."
```

## FeatureCard

```yaml
name: "FeatureCard"
purpose: "Explain a capability, benefit, or differentiator."
anatomy:
  - "icon or small media"
  - "headline"
  - "short description"
  - "optional supporting link"
variants:
  - "icon_top"
  - "split"
  - "metric"
  - "proof"
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
  - "color.action_secondary"
  - "color.text_primary"
  - "spacing.space_5"
  - "radius.radius_lg"
behavior:
  - "Keep text concise and benefit-led."
  - "Use hover only when the card navigates or expands."
accessibility:
  - "Icons are decorative unless they add unique meaning."
do:
  - "Use consistent icon scale."
dont:
  - "Do not use vague feature labels."
```

## ContentCard

```yaml
name: "ContentCard"
purpose: "Preview an article, post, project, episode, update, or listing item."
anatomy:
  - "thumbnail or placeholder"
  - "title"
  - "summary"
  - "metadata row"
  - "category or tag"
variants:
  - "grid"
  - "list"
  - "compact"
  - "editorial"
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
  - "color.text_primary"
  - "color.text_muted"
  - "spacing.space_3"
  - "radius.radius_md"
behavior:
  - "Clamp titles to 2 or 3 lines according to density."
  - "Keep metadata grouped and readable."
accessibility:
  - "Use descriptive titles as link text."
  - "Expose meaningful metadata in text."
do:
  - "Use content roles instead of fixed category names."
dont:
  - "Do not make the entire card clickable when inner links conflict."
```

## MediaCard

```yaml
name: "MediaCard"
purpose: "Present visual or playable content with title and compact metadata."
anatomy:
  - "media frame"
  - "duration or status overlay"
  - "title"
  - "creator or owner"
  - "metrics"
variants:
  - "video"
  - "gallery"
  - "audio"
  - "product_media"
  - "placeholder"
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
  - "radius.radius_md"
  - "shadow.shadow_focus"
  - "motion.duration.short"
behavior:
  - "Use fixed aspect ratio for media."
  - "Reveal controls only when available and keyboard reachable."
accessibility:
  - "Provide alt text or media labels."
  - "Do not autoplay sound."
do:
  - "Use placeholders for missing media."
dont:
  - "Do not rely on thumbnail text for essential information."
```

## ArticleCard

```yaml
name: "ArticleCard"
purpose: "Preview readable long-form content."
anatomy:
  - "eyebrow"
  - "title"
  - "excerpt"
  - "author"
  - "date or reading time"
variants:
  - "featured"
  - "standard"
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
  - "typography.h3"
  - "typography.body_sm"
  - "color.text_muted"
behavior:
  - "Use title as the primary link."
accessibility:
  - "Keep card order logical for screen readers."
do:
  - "Use readable excerpts."
dont:
  - "Do not truncate every signal in dense mode."
```

## ProductCard

```yaml
name: "ProductCard"
purpose: "Support product discovery and comparison."
anatomy:
  - "product media"
  - "name"
  - "price"
  - "rating or trust cue"
  - "primary action"
variants:
  - "grid"
  - "list"
  - "sale"
  - "out_of_stock"
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
  - "color.warning"
  - "radius.radius_lg"
behavior:
  - "Keep price and availability visible."
accessibility:
  - "Expose sale and stock status in text."
do:
  - "Use consistent product media ratios."
dont:
  - "Do not hide required purchase details behind hover."
```

## DiscussionCard

```yaml
name: "DiscussionCard"
purpose: "Preview a community thread, question, topic, or update."
anatomy:
  - "topic title"
  - "author summary"
  - "reply or activity count"
  - "latest activity"
  - "tags"
variants:
  - "thread"
  - "question"
  - "announcement"
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
  - "color.text_muted"
  - "color.action_primary"
  - "radius.radius_lg"
behavior:
  - "Sort by activity, recency, or relevance according to page intent."
accessibility:
  - "Use title as the main link and expose counts as text."
do:
  - "Show participation signals."
dont:
  - "Do not hide moderation status."
```

## MemberAvatar

```yaml
name: "MemberAvatar"
purpose: "Represent a person, team, or account in compact spaces."
anatomy:
  - "avatar image or initials"
  - "status ring"
  - "optional tooltip"
variants:
  - "image"
  - "initials"
  - "stack"
  - "status"
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
  - "color.border_subtle"
  - "color.success"
behavior:
  - "Use fallback initials when images are unavailable."
accessibility:
  - "Use empty alt when adjacent name is visible; otherwise provide the name."
do:
  - "Keep status cues text-accessible."
dont:
  - "Do not identify people by color alone."
```

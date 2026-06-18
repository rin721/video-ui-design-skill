# Blog Pattern

## Structure

```yaml
blog:
  editorial_header:
    purpose: "定义刊物主题和阅读承诺"
  featured_post:
    purpose: "突出一篇及时或高价值文章"
  category_nav:
    purpose: "支持主题发现"
  post_grid:
    purpose: "展示近期和常青文章"
  newsletter_cta:
    purpose: "鼓励重复阅读"
  footer:
    purpose: "承载归档、政策、社交和联系链接"
```

## Layout

- 使用编辑型节奏，文章标题强，正文行宽舒适。
- 发现页使用网格卡片，阅读页使用全宽文章布局。
- category navigation 仅在改善浏览时 sticky。

## Components

使用 `NavigationBar`、`ArticleCard`、`AuthorBlock`、`TableOfContents`、`NewsletterBlock`、`Tag` 和 `Footer`。

## Acceptance

- 文章正文保持 `58ch` 到 `72ch`。
- metadata 支持信任但不拥挤。
- 展示价值后再邀请订阅。

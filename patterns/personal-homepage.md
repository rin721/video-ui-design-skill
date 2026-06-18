# Personal Homepage Pattern

## Structure

```yaml
personal_homepage:
  intro_hero:
    purpose: "建立姓名、角色和当前关注点"
  identity_statement:
    purpose: "解释此人做什么以及价值所在"
  selected_work:
    purpose: "展示最强项目或成果"
  writing_or_projects:
    purpose: "通过文章、演讲、实验或笔记提供深度"
  contact_cta:
    purpose: "邀请合作、招聘、演讲或交流"
  footer:
    purpose: "提供社交链接和次级信息"
```

## Layout

- 使用 balanced density，hero 空间宽松，项目卡片紧凑。
- 头像或肖像可选且必须可替换。
- 平板和桌面使用两列作品网格，窄屏使用单列。

## Components

使用 `HeroSection`、`SectionHeader`、`ContentCard`、`MediaCard`、`AuthorBlock`、`CTASection` 和 `Footer`。

## Acceptance

- 不读完细节也能理解身份。
- selected work 包含角色、结果和链接。
- 联系路径在末尾可见，也可放入导航。

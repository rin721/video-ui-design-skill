# Documentation Pattern

## Structure

```yaml
documentation:
  doc_shell:
    purpose: "组合 sidebar、内容区、搜索和工具操作"
  sidebar_nav:
    purpose: "展示内容层级"
  content_area:
    purpose: "支持任务完成和阅读"
  code_or_example_block:
    purpose: "展示命令、配置或实现片段"
  pagination:
    purpose: "在相邻主题间移动"
```

## Layout

- Desktop：持久 sidebar，内容行宽接近 `72ch`，可选右侧目录。
- Tablet：可折叠 sidebar，全宽内容。
- Mobile：顶部搜索、可折叠导航、单列可读内容。

## Components

使用 `NavigationBar`、`SidebarTree`、`SearchInput`、`TableOfContents`、`CodeBlock`、`Callout`、`PaginationNav` 和 `Footer`。

## Acceptance

- 用户可以搜索、浏览层级并完成任务。
- 代码块可读且键盘可访问。
- 当前所在位置在导航中可见。

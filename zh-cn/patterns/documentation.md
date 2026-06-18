# Documentation Pattern

## Structure

```yaml
documentation:
  doc_shell:
    purpose: "combine sidebar, content area, search, and utility actions"
  sidebar_nav:
    purpose: "show content hierarchy"
  content_area:
    purpose: "support task completion and reading"
  code_or_example_block:
    purpose: "show commands, configuration, or implementation snippets"
  pagination:
    purpose: "move between adjacent topics"
```

## Layout

- Desktop: persistent sidebar, content measure near `72ch`, optional right table of contents.
- Tablet: collapsible sidebar, full-width content.
- Mobile: top search, collapsible navigation, readable one-column content.

## Components

Use `NavigationBar`, `SidebarTree`, `SearchInput`, `TableOfContents`, `CodeBlock`, `Callout`, `PaginationNav`, and `Footer`.

## Acceptance

- Users can search, navigate hierarchy, and complete a task.
- Code blocks are readable and keyboard accessible.
- Current location is visible in navigation.

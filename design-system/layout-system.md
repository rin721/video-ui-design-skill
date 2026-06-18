# 布局系统

## Layout Tokens

```yaml
layout_system:
  container:
    max_width_desktop: "80rem"
    max_width_tablet: "56rem"
    max_width_mobile: "100%"
    horizontal_padding:
      desktop: "3rem"
      tablet: "2rem"
      mobile: "1rem"
  grid:
    desktop_columns: "12"
    tablet_columns: "8"
    mobile_columns: "4"
    gutter:
      desktop: "1.5rem"
      tablet: "1.25rem"
      mobile: "1rem"
  section_rhythm:
    hero_to_section: "4rem to 5rem"
    section_to_section: "3rem to 4rem"
    dense_block_gap: "1rem to 1.5rem"
    card_grid_gap: "1rem to 1.5rem"
  visual_flow:
    primary_scan_path: "context header, section marker, content grid, action"
    emphasis_strategy: "single bright action with soft active markers"
    content_reveal_order: "identity, navigation, content clusters, proof, conversion"
  responsive_behavior:
    desktop: "side utility rail or top navigation plus 4 to 5 content columns"
    tablet: "top or side navigation plus 2 to 3 content columns"
    mobile: "top brand row, bottom or drawer navigation, 1 to 2 content columns"
```

## Shell Rules

- 宽屏中仅在跨页面重复操作较多时使用固定工具栏。
- 顶部 app bar 用于身份、搜索或账户语境。
- 移动端底部导航只用于高频一级目的地。
- 搜索、onboarding、登录、注册和空状态适合居中页面。
- 右侧辅助面板出现时，主内容至少保留可用宽度的 `60 percent`。

## Grid Rules

- 媒体和内容卡片使用 `repeat(auto-fit, minmax(14rem, 1fr))`。
- 媒体使用固定比例：`16 / 9`、`4 / 3`、`1 / 1` 或 `3 / 4`。
- 网格项在 hover、loading 和 error 状态中保持尺寸稳定。
- 文本容器使用 `min-width: 0`，避免水平溢出。

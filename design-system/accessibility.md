# 可访问性

## Compliance Goal

达到 WCAG 2.2 AA 或更高标准。

```yaml
accessibility:
  contrast:
    body_text: ">= 4.5:1"
    large_text: ">= 3:1"
    non_text_ui: ">= 3:1 where applicable"
  keyboard:
    - all_interactive_elements_focusable
    - visible_focus_state
    - logical_tab_order
  motion:
    - respects_prefers_reduced_motion
    - no_required_motion_only_feedback
  semantics:
    - landmark_structure
    - heading_order
    - form_labeling
    - button_link_semantics
  responsive:
    - tap_area_minimum
    - mobile_readability
    - no_horizontal_scroll
  content:
    - clear_error_messages
    - meaningful_empty_states
    - accessible_alt_text_rules
```

## Required Practices

- 每页使用一个 `main` landmark。
- 标题顺序保持逻辑一致。
- 操作用 button，导航用 link。
- 图标按钮必须有可访问名称。
- 使用 `shadow_focus` 或等价 outline 提供可见 focus 样式。
- 移动端点击区域至少 `44px`。
- 异步 success、loading 和 error 更新使用 `aria-live="polite"`。
- 表单 label 在字段填写后仍保持可用。
- 尊重 `prefers-reduced-motion`。

## Text Alternatives

- 装饰图片使用空 alt。
- 信息性媒体描述用途，而不是无关视觉细节。
- 商品和内容缩略图描述项目类别与有意义主体。
- 带文字标签的按钮内图标不需要重复标签。

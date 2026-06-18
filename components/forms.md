# 表单

## FormField

```yaml
name: "FormField"
purpose: "收集单个用户输入，并提供清楚标签和反馈。"
anatomy:
  - "label"
  - "input control"
  - "helper text"
  - "error text"
  - "optional leading or trailing icon"
variants:
  - "text"
  - "textarea"
  - "select"
  - "checkbox"
  - "radio"
  - "switch"
  - "file"
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
  - "color.border_default"
  - "color.focus_ring"
  - "color.danger"
  - "radius.radius_md"
behavior:
  - "简单字段 blur 后校验，依赖字段 submit 时校验。"
  - "helper 与 error 文本保持同一位置。"
accessibility:
  - "使用可见 label 并连接 input。"
  - "错误文本通过 aria-describedby 连接。"
  - "placeholder 不能作为唯一 label。"
do:
  - "错误文本说明恢复方法。"
dont:
  - "校验失败后不要清空输入。"
```

## SearchInput

```yaml
name: "SearchInput"
purpose: "帮助用户查找内容、商品、文档或命令。"
anatomy:
  - "label or accessible name"
  - "input"
  - "search icon"
  - "submit or clear button"
  - "optional suggestions"
variants:
  - "global"
  - "section"
  - "command"
  - "filter"
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
  - "color.focus_ring"
  - "shadow.shadow_focus"
  - "radius.radius_lg"
behavior:
  - "有查询内容时 Enter 提交。"
  - "获取建议时展示 loading。"
  - "输入后提供 clear button。"
accessibility:
  - "全局搜索使用 search landmark。"
  - "建议更新时播报建议数量。"
do:
  - "只有能改善结果时才提供范围筛选。"
dont:
  - "不要让基础搜索必须依赖高级选项。"
```

## VariantSelector

```yaml
name: "VariantSelector"
purpose: "让用户选择商品、套餐、格式或配置变体。"
anatomy:
  - "label"
  - "option group"
  - "option"
  - "selected marker"
  - "availability text"
variants:
  - "swatch"
  - "size"
  - "plan"
  - "segmented"
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
  - "color.border_default"
  - "color.action_primary"
  - "radius.radius_md"
behavior:
  - "禁用不可用变体并说明原因。"
  - "立即更新关联价格或媒体。"
accessibility:
  - "单选使用 radio group 语义。"
do:
  - "selected 状态保持可见。"
dont:
  - "不要只用颜色表达选择。"
```

## CheckoutStep

```yaml
name: "CheckoutStep"
purpose: "表达购买、注册或设置流程中的步骤。"
anatomy:
  - "step indicator"
  - "title"
  - "status"
  - "content"
  - "actions"
variants:
  - "linear"
  - "editable_summary"
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
  - "color.info"
  - "color.success"
  - "color.danger"
  - "radius.radius_lg"
behavior:
  - "允许返回编辑已完成步骤。"
  - "步骤切换时保留已输入数据。"
accessibility:
  - "用文本暴露当前步骤和完成状态。"
do:
  - "显示清晰下一步操作。"
dont:
  - "不要把阻塞错误藏在长表单底部。"
```

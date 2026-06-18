# 可访问性清单

## Contrast

- 正文对比度至少 `4.5:1`。
- 大文字对比度至少 `3:1`。
- UI 边界和 focus indicator 在适用时达到 `3:1`。
- 状态颜色搭配图标、文字或结构。

## Keyboard

- 所有交互元素都可通过键盘到达。
- focus 顺序符合视觉和任务顺序。
- 每个交互组件都有可见 focus 状态。
- menu、modal、tabs、accordion 和 command palette 都有键盘行为。

## Semantics

- 每页有一个 `main` landmark。
- 导航使用带清晰标签的 `nav`。
- 页脚使用 `footer`。
- 标题顺序正确。
- 按钮和链接使用正确元素。
- 表格只用于表格数据。

## Forms

- 每个输入都有可见 label。
- helper 和 error 文本与控件关联。
- 错误说明恢复方法。
- 提交状态会被播报。

## Motion

- 尊重 `prefers-reduced-motion`。
- 不存在只靠动效表达的必要反馈。
- 自动播放内容可暂停。

## Responsive

- 移动端点击区域至少 `44px`。
- 文本不依赖视口缩放字体也可读。
- 标准移动宽度下无水平滚动。

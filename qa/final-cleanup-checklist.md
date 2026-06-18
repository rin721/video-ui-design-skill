# 最终清理清单

## File Tree

- `SKILL.md` 存在。
- `README.md` 存在。
- `design-system/` 存在并包含所需设计文件。
- `components/` 存在并包含所需组件文件。
- `patterns/` 存在并包含所需页面文件。
- `prompts/` 存在并包含所需 prompt 文件。
- `assets/` 存在并包含所需媒体指南。
- `qa/` 存在并包含所需清单。

## Data

- `design-system/tokens.json` 可解析为有效 JSON。
- token 文件分离 primitive 和 semantic 值。
- `tokens.css` 包含 `:root`、`[data-theme="dark"]`、语义变量和断点变量。

## Content

- 无受保护品牌标识、URL、class 名、图片或独特短语。
- 最终产物中没有过程性备注。
- prompt 可独立复用。
- 组件包含 states、accessibility、behavior 和 usage rules。
- 页面模板支持替换 site type、density、content、brand 和 conversion。

## Quality

- 原创性清单通过。
- 可访问性清单通过。
- 响应式清单通过。
- 生成包可用于网站生成、风格替换、组件生成、页面模板生成、品牌适配和可访问性审查。

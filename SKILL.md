---
name: ui-design-skill-zh-cn
description: 生成原创网站设计系统、语义化 token、可复用组件规范、页面模板、视觉资产规则、可访问性指南和提示词模块，适用于个人主页、博客、社区、SaaS、电商、文档站、作品集、产品页、品牌站和营销网站。
---

# UI Design Skill

## Purpose

使用该 skill 创建原创网站设计系统、页面模板、组件规范、语义化 token、响应式规则、视觉资产指南和前端生成提示词。输出必须能跨网站类型复用，并支持品牌、内容和视觉资产替换。

## When to Use

在生成或优化以下网站时使用：

- 个人主页、作品集、博客和编辑型内容站。
- 社区、媒体、目录和内容发现体验。
- SaaS、产品、AI 工具和 Web App 落地页。
- 电商、定价、结账和商品详情页。
- 文档站、帮助中心、知识库和开发者门户。
- 多页面营销站和品牌系统。

## Inputs

可接受以下输入：

- `project_name`：包或 skill 名称。
- `site_type`：`auto`、`personal_homepage`、`blog`、`community`、`saas`、`ecommerce`、`documentation` 或 `multi_page`。
- `generation_goal`：输出目标，如 `design_system`、`page_template`、`component_set` 或 `website_prompt`。
- `viewport_modes`：desktop、tablet、mobile。
- `capture_states`：default、hover、focus、active、disabled、loading、empty、error、selected。
- `style_abstraction_level`：low、medium、high。
- `accessibility_level`：合规目标，默认 `WCAG_2_2_AA_or_better`。
- `brand_swap_parameters`：seriousness、warmth、innovation、luxury、playfulness、editorial、technical depth。

## Workflow

1. 观察布局、层级、密度、控件、状态、动效和响应式行为。
2. 将视觉语言抽象为可迁移规则，而不是固定页面拷贝。
3. 将颜色、字体、间距、圆角、阴影、动效、层级和断点归一化为语义化 token。
4. 定义包含结构、变体、状态、约束、可访问性和使用规则的组件。
5. 组合可切换网站类型、内容密度、转化目标和品牌表达的页面模板。
6. 生成页面、组件、风格、可访问性和质量任务可单独使用的 prompt block。
7. 清理所有产物，确保不包含复用文案、图片、标志、商标、class 名、路由名或独特视觉符号。
8. 检查独立性、完整性、可实现性、可访问性、响应式和原创性。

## Output Contract

生成以下内容：

- `SKILL.md` 和 `README.md`。
- `design-system/`：总览、原则、token、字体、色彩、间距、布局、可访问性和品牌表达。
- `components/`：导航、按钮、卡片、表单、反馈、内容区块和转化区块组件 schema。
- `patterns/`：落地页、个人主页、博客、社区、SaaS、电商和文档站页面模板。
- `prompts/`：网站生成、风格替换、组件生成、页面生成和质量审查 prompt。
- `assets/`：视觉资产、图标和媒体替换规则。
- `qa/`：原创性、可访问性、响应式和最终清理清单。

## Design Rules

- 优先使用语义化 token，不直接写固定值。
- 保持主色可替换，只在有意义的强调位置使用强调色。
- 优先清晰层级、充足留白、密集但可快速扫描的内容网格。
- 重复操作使用图标按钮，明确命令使用文本按钮。
- 适用时为每个交互元素提供 hover、focus、active、disabled、loading 和 selected 状态。
- focus 状态必须可见，不能只依赖颜色。
- 移动端点击区域至少 `44px`。
- 使用响应式网格，让多列桌面布局折叠为平板和移动端可读布局。
- 尊重 `prefers-reduced-motion`，并提供非动效反馈。
- 确保中文、英文、数字和代码样式文本都可读。

## Guardrails

- 不使用任何现有产品的文字、图片、标志、商标、专属图标、路由标签、CSS 选择器、组件名或视觉签名。
- 不生成像素级锁定布局或只适合单一页面的固定尺寸。
- 不依赖专有字体或资产。
- 状态、校验和选择不能只靠颜色表达。
- 装饰性媒体不能成为理解内容的必要条件。
- 最终文件不得包含品牌标识、受保护 artwork、截图、URL 或过程痕迹。

## Usage Examples

生成 SaaS 落地页系统：

```yaml
site_type: saas
generation_goal: design_system_and_landing_page
brand_swap_parameters:
  seriousness: medium
  warmth: medium
  innovation: high
  luxury: low
  playfulness: medium
  editorial: low
  technical_depth: medium
```

生成博客模板集：

```yaml
site_type: blog
generation_goal: page_templates_and_components
content_density: medium_to_dense
accessibility_level: WCAG_2_2_AA_or_better
```

生成文档站外壳：

```yaml
site_type: documentation
generation_goal: doc_shell_and_prompt_blocks
content_density: dense
brand_swap_parameters:
  seriousness: high
  warmth: low
  technical_depth: high
```

# Soft Modular Product UI Skill
### 把模糊的界面需求变成可运行的产品 UI 语言。

> 「不要再说清爽一点。让界面自己知道该怎么呼吸。」

`Agent Skill` · `Design Tokens` · `Component Recipes` · `Responsive UI` · `WCAG AA`

SMUI 帮你把官网首页、落地页、产品介绍页、内容型页面、企业展示页和移动端页面，蒸馏成一套可以被 AI agent 执行的设计规则。

输入页面类型、目标用户、内容轮廓和少量品牌偏好，它会读取 token、布局语法、组件配方、交互状态、响应式规则和质量检查清单，输出结构化 design spec，或进一步生成 HTML/CSS、React、Vue、Tailwind、Figma prompt。

今天你可以用它生成一个柔和、明亮、轻量、模块化的产品界面。未来它可以成为多项目 UI 生成、组件库起稿、设计系统迁移和前端原型生成的视觉行为层。

看效果 · 为什么不是模板库 · SMUI 蒸馏什么 · 产品哲学 · 使用场景 · 安装 · 工作原理 · 仓库结构

---

## 效果示例

你不需要先画完整 wireframe，也不需要写一长串审美形容词。

只要说：

```text
> 使用 Soft Modular Product UI Skill，为一个协作工具生成 landing page。
> 输出 React + CSS variables。
> 需要 hero、功能卡片、价格区、FAQ、CTA 和移动端布局。
> 主色使用柔和蓝绿色，整体保持轻盈、亲和、模块化。
```

生成时，Skill 不会只给你一段“好看的页面描述”。它会把页面拆成可执行的判断：

```text
页面      ❯ 协作工具 landing page

视觉      ❯ 浅灰底 + 白色表面，主色只进入 CTA、当前状态、重点图标和少量标签。
            卡片使用轻量边界，不靠厚阴影制造层级。

布局      ❯ hero 露出下一段内容；功能区使用 3 列到 1 列响应式重排；
            价格区保持同高卡片，移动端改为单列纵向比较。

组件      ❯ Button / Navigation / Card / Form / FAQ / CTA 全部包含
            hover、active、focus-visible、disabled、loading、empty、error 状态。

响应式    ❯ Desktop 1040-1120px 容器；Tablet 2 列卡片；
            Mobile 16px gutter、44x44px 触控目标、底部导航不遮挡内容。

验证      ❯ 检查 WCAG AA、语义 token、标题长度、CTA 密度、reduced motion。
```

这不是把圆角、浅色、卡片和渐变拼起来。真正被蒸馏出来的是：一个产品界面在信息压力、品牌替换、组件状态、断点变化和可访问性约束下，应该怎样保持一致。

---

## 为什么不是 UI 模板

普通模板常常这样写：

```text
风格：清爽、柔和、卡片化。
布局：Hero + Feature + Pricing + FAQ + CTA。
颜色：粉色或蓝绿色。
```

这对 AI 来说太模糊。它知道形容词，却不知道怎么行动。

SMUI 要写的是：

```text
当页面需要表达轻量产品感时，主色只能承担动作和状态，不承担整页背景。
当内容密度上升时，先压缩卡片内部元信息，再重排网格，不牺牲正文行距。
当品牌主色替换后，必须同步生成 hover、focus、pressed、disabled、ripple 和 shadow 变体。
```

区别就在这里：

| 模板库 | SMUI |
| --- | --- |
| 写固定页面顺序 | 写可组合的布局语法 |
| 复述审美标签 | 蒸馏视觉决策机制 |
| 靠卡片和圆角装像 | 用 token、密度、状态和层级塑形 |
| 很少处理边界 | 明确响应式、可访问性和替换规则 |
| 改主色容易散 | 用语义 token 保持全局一致 |

模板告诉你页面怎么摆。SMUI 让界面知道自己为什么这样摆。

---

## SMUI 蒸馏什么

SMUI 提取七层信息：

| 层次 | SMUI 关心的问题 |
| --- | --- |
| 视觉 token | 颜色、字号、间距、圆角、阴影、断点和动效如何语义化？ |
| 布局语法 | 页面如何分区、露出下一段、重排网格、控制阅读节奏？ |
| 组件配方 | Button、Navigation、Hero、Card、Form、Modal、Footer、CTA 如何成套出现？ |
| 状态机制 | hover、active、focus、disabled、loading、error、success、empty 如何被补齐？ |
| 响应式策略 | Desktop、Tablet、Mobile 如何改变容器、列数、导航和触控区域？ |
| 内容节奏 | 标题、正文、CTA、空状态、错误提示如何短、准、可替换？ |
| 质量边界 | 什么时候必须拒绝专有素材、真实标识、逐像素复刻和不可访问实现？ |

SMUI 不追求更像一个模板。它追求更像一套能运行的界面判断。

---

## 产品哲学

SMUI 的底层判断很简单：界面不是漂亮截图，而是一套可执行的信息系统。

参考图告诉你一个页面长什么样；模板告诉你一个页面通常有哪些区块；SMUI 要进一步回答：当用户的需求还不完整、品牌色要替换、文案长度会变化、断点会压缩、组件会进入错误状态时，界面应该先保什么、让什么、改什么。

这也是 SMUI 坚持规则化输出的原因。一个页面如果只有“柔和”“高级”“模块化”这些词，生成几轮就会变成同质化拼贴；但如果它有语义 token、布局语法、组件 recipes、状态边界和验证清单，它就能在不同产品里保持同一种秩序，而不是每次靠审美词救场。

| SMUI 要写进去的 | 意味着什么 | 没写进去会怎样 |
| --- | --- | --- |
| 语义 token | 颜色和尺寸有角色，而不是散落的数值 | 改主色后全局失控 |
| 布局语法 | 页面区块可组合、可替换、可响应式重排 | 只剩固定顺序复刻 |
| 组件 recipes | 每个组件知道用途、结构、状态和边界 | 组件只有静态样子 |
| 交互状态 | 用户操作、等待、错误和空状态都有归处 | 页面一到真实场景就塌 |
| 内容规则 | 标题、段落、CTA 有长度和语气约束 | 文案撑爆容器或变成广告腔 |
| 验证清单 | 交付前能检查可访问性、响应式和清洁度 | 看起来完成，实际不可复用 |

写得进去的是生成规则，写不进去的要变成边界。这不是降低自由度，反而是让界面更可信：真正稳定的设计系统，不会靠一次灵感维持一致。

---

## 使用场景

SMUI 不只是“生成一个好看的页面”的工具。它更像是把产品 UI 从静态参考中解放出来，变成可以被设计、前端和 AI agent 调用的视觉行为层。

现在，它可以用于：

| 场景 | 怎么用 | SMUI 提供什么 |
| --- | --- | --- |
| 产品官网 | 从一句产品定位起稿首页 | Hero、卖点、证明区、CTA 和响应式结构 |
| Landing page | 快速生成转化页面 | 信息节奏、CTA 密度、FAQ 和价格区 |
| 内容门户 | 组织文章、资源、活动或课程入口 | 低噪声信息层级、卡片网格、筛选与空状态 |
| 移动端首页 | 生成手机端产品界面 | 顶部工具栏、底部导航、触控目标和单列/双列内容流 |
| 组件规范 | 建立轻量组件库 | variants、states、tokens、可访问性和实现提示 |
| 前端原型 | 输出 HTML/CSS、React、Vue 或 Tailwind | 语义结构、CSS variables、状态选择器和断点策略 |

未来，它可以继续走向：

| 方向 | 可能形态 |
| --- | --- |
| 多品牌设计系统迁移 | 用 brand overrides 快速替换主色、圆角、字体、密度和动效强度 |
| AI 原型工作台 | 把产品需求直接转成可验证的页面 spec 和前端骨架 |
| 组件库扩写 | 按统一 recipe 增加新组件，保持状态、响应式和可访问性完整 |
| 设计质量守门 | 用 validation checklist 检查生成结果是否只是好看、却不可落地 |

SMUI 面向的是更稳定的 UI 生成基础设施。今天它服务单页设计和前端原型；未来它可以成为产品团队反复调用、替换、验证和扩展的界面规则层。

---

## 安装

SMUI 是一个 Codex / Agent Skills 风格的 design skill。若你的运行环境支持从 GitHub 安装 skill，可以直接使用：

```bash
skills add rin721/video-ui-design-skill
```

也可以手动安装：

```bash
git clone https://github.com/rin721/video-ui-design-skill.git
cp -r video-ui-design-skill ~/.codex/skills/soft-modular-product-ui
```

复制后，入口文件是 `SKILL.md`。规则文件、示例和质量检查清单都在同一目录内，不依赖私有素材或专有服务。

### 依赖

- Markdown：用于读取 skill 规则、recipes、示例和检查清单。
- JSON：`design-tokens.json` 必须保持合法 JSON。
- 前端运行环境：仅当你要求输出 React、Vue、Tailwind 或静态页面实现时需要。

---

## 使用

安装后，对 Codex 或支持 Agent Skills 的运行环境说：

```text
> 使用 Soft Modular Product UI Skill，生成一个产品官网首页。
> 输出 UI design spec。
> 受众是中小团队，页面需要轻量、清晰、可信。
```

也可以直接指定技术栈：

```text
> 使用 Soft Modular Product UI Skill，输出移动端产品首页。
> 需要 React + CSS variables。
> 包含顶部工具栏、底部导航、信息提示条、产品卡片、空状态和错误状态。
```

模糊需求也可以：

```text
> 想要一个柔和一点的 SaaS 首页。
> 帮我把这个功能介绍区做得更像产品页面。
> 给一个清爽的内容门户首页结构。
```

SMUI 会先判断 `page_type`、`output_mode`、内容完整度和品牌覆盖项。用户没有提供文案时，它会使用中性、可替换、非专有的占位内容；用户提供主色时，它会同步更新相关状态 token，而不是只替换一个按钮颜色。

---

## 工作原理

SMUI 默认生成可执行 design spec；当用户指定技术栈时，再映射为对应代码结构。一次完整运行会做六件事：

1. 读取任务入口
从 `SKILL.md` 判断页面类型、输出模式、技术栈、可访问性要求和需要加载的规则文件。

2. 建立视觉变量
读取 `design-tokens.json`，建立颜色、字体、间距、圆角、阴影、边框、断点和动效变量。

3. 选择布局语法
读取 `layout-patterns.md`，根据页面目标选择 2-4 个可组合模块，而不是套用固定页面顺序。

4. 生成组件 recipes
读取 `component-recipes.md`，补齐组件用途、视觉结构、token 依赖、状态规则、响应式规则、可访问性和技术实现提示。

5. 校正交互、响应式和内容
读取 `interaction-rules.md`、`responsive-rules.md` 和 `content-rules.md`，处理 hover、focus、loading、empty、error、键盘、触控、标题长度和 CTA 密度。

6. 运行质量检查
使用 `validation-checklist.md` 检查视觉语言、token 使用、布局、组件状态、响应式、可访问性、内容规则和发布清洁度。

完整方法论见：

- `style-profile.md`
- `layout-patterns.md`
- `component-recipes.md`
- `runtime-decision-tree.md`
- `validation-checklist.md`

---

## 输出长什么样

SMUI 可以输出多种形态：

| 输出模式 | 适合什么 |
| --- | --- |
| UI design spec | 设计方案、规则、结构和组件说明 |
| HTML / CSS | 可直接放入静态页面的语义结构和样式变量 |
| React | 数据驱动组件、props、状态枚举和 CSS variables |
| Vue | props、slots、computed class 和 scoped CSS variables |
| Tailwind | token 到 config 的映射、组件 class 和 responsive variants |
| Figma prompt | frame、auto layout、token、component variants 和 constraints |
| Wireframe outline | 低保真模块顺序、内容密度和响应式 sketch |
| Component library spec | variants、states、tokens、键盘行为和实现提示 |

每种输出都应该能被独立读取、复用和继续扩展。

---

## 更新与扩展

### 更新 design tokens

1. 修改 `design-tokens.json` 中的 `value`、`usage`、`modifiable` 或 `fallback`。
2. 保持 token 名称语义化，例如 `color.brand.primary`。
3. 不删除已被组件依赖的 token；需要废弃时新增替代 token。
4. 更新后检查 JSON 合法性，并按全文清洁度规则确认没有专有痕迹。

### 更新 component recipes

1. 在 `component-recipes.md` 中新增组件时，保持相同结构：使用场景、视觉结构、token 依赖、状态规则、响应式规则、可访问性规则、技术实现提示、禁止事项和生成示例。
2. 新组件必须使用已有 token；新增视觉变量时同步更新 `design-tokens.json`。
3. 示例文案保持中性、可替换、非专有。

### 替换视觉风格

风格替换时，读取 `adaptation-rules.md`，同步调整主色、辅助色、字体、圆角、卡片密度和动效强度。替换完成后，必须重新检查 hover、focus、pressed、disabled、ripple、shadow 和文本对比度。

---

## 质量边界

SMUI 生成的结果必须保持：

- 使用语义 token，而不是散落硬编码颜色、圆角、阴影和断点。
- 覆盖 hover、active、focus-visible、disabled、loading、error、success、empty 状态。
- 覆盖 desktop、tablet、mobile，并保证移动端触控目标不小于 44x44px。
- 满足文本对比度、键盘操作、表单 label、alt、标题层级和 reduced motion。
- 避免具名商业标识、真实网址、专有图片、专有图标、不可授权文案和真实业务数据。
- 避免逐像素复刻和固定页面顺序。

不会假装审美词已经等于设计系统。能写成规则的就写成规则，暂时不能确定的就变成可检查的边界。

---

## 仓库结构

```text
video-ui-design-skill/
├── SKILL.md                         # Skill 入口、触发方式、运行流程
├── design-tokens.json               # 语义 token：颜色、字体、间距、圆角、阴影、断点、动效
├── style-profile.md                 # 视觉气质、密度、情绪和一致性边界
├── layout-patterns.md               # 页面布局语法与可组合模块
├── component-recipes.md             # 组件配方、状态、响应式和可访问性
├── interaction-rules.md             # hover、active、focus、loading、empty、error 等交互规则
├── responsive-rules.md              # desktop、tablet、mobile 的断点和重排策略
├── content-rules.md                 # 标题、正文、CTA、空状态和错误文案规则
├── adaptation-rules.md              # 主色、字体、圆角、密度和动效替换规则
├── output-modes.md                  # design spec、代码、Figma prompt 等输出形态
├── runtime-decision-tree.md         # 运行时选择文件和输出路径
├── validation-checklist.md          # 质量检查与发布清洁度
├── prompt-templates.md              # 常用调用模板
└── examples/
    ├── landing-page.md
    ├── mobile-page.md
    ├── product-section.md
    └── corporate-homepage.md
```

---

参考图告诉你页面长什么样。

SMUI 让界面知道自己为什么这样摆。

不要再说清爽一点。

让界面自己知道该怎么呼吸。

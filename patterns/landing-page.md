# Landing Page Pattern

## Structure

```yaml
landing_page:
  global_nav:
    purpose: "定位访客并展示核心目的地"
    density: "compact"
  hero:
    purpose: "说明 offer、受众和结果"
    layout: "居中或全宽，并使用真实产品、场景或交互表面"
  trust_signal:
    purpose: "展示简洁可信信号"
  feature_grid:
    purpose: "解释 3 到 6 个能力或收益"
  proof_section:
    purpose: "展示结果、评价、指标或使用语境"
  conversion_cta:
    purpose: "邀请试用、演示、注册、购买或联系"
  footer:
    purpose: "支持次级导航和法律收束"
```

## Layout

- Desktop：使用 12 列网格，hero 放在 `80rem` 容器内，feature grid 为 3 列。
- Tablet：feature 和 proof grid 使用 2 列。
- Mobile：hero 单列堆叠，主操作靠近标题。

## Components

使用 `NavigationBar`、`HeroSection`、`SectionHeader`、`FeatureCard`、`TestimonialBlock`、必要时使用 `PricingBlock`、`CTASection` 和 `Footer`。

## Acceptance

- 一个主操作在视觉上最突出。
- 首屏即可理解产品或 offer。
- 最终转化前出现信任内容。
- 装饰媒体可替换，且不承担理解必要信息。

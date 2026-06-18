# Ecommerce Pattern

## Structure

```yaml
ecommerce:
  commerce_hero:
    purpose: "介绍类别、系列或促销"
  category_grid:
    purpose: "帮助购物者缩小意图"
  product_grid:
    purpose: "支持比较和发现"
  product_card:
    purpose: "展示图片、名称、价格、状态和操作"
  cart_cta:
    purpose: "推动已选商品进入购买流程"
```

## Layout

- 使用密集但可扫描的商品网格。
- 筛选在移动端可访问且可折叠。
- 价格、可用状态和主购买操作保持可见。

## Components

使用 `NavigationBar`、`ProductCard`、`VariantSelector`、`CartSummary`、`CheckoutStep`、`Badge`、`Alert` 和 `Footer`。

## Acceptance

- 不打开每个详情页也能比较商品。
- 折扣、库存和配送信息包含文字。
- 结账步骤保留输入并提供恢复路径。

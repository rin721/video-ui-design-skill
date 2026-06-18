# Ecommerce Pattern

## Structure

```yaml
ecommerce:
  commerce_hero:
    purpose: "introduce category, collection, or promotion"
  category_grid:
    purpose: "help shoppers narrow intent"
  product_grid:
    purpose: "enable comparison and discovery"
  product_card:
    purpose: "show image, name, price, status, and action"
  cart_cta:
    purpose: "move selected items toward purchase"
```

## Layout

- Use dense but scannable product grids.
- Keep filters accessible and collapsible on mobile.
- Keep price, availability, and primary purchase action visible.

## Components

Use `NavigationBar`, `ProductCard`, `VariantSelector`, `CartSummary`, `CheckoutStep`, `Badge`, `Alert`, and `Footer`.

## Acceptance

- Product comparison is possible without opening every detail page.
- Sale, stock, and shipping messages include text.
- Checkout steps preserve user input and expose recovery paths.

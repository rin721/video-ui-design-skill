# 间距、形态与层级

## Spacing Tokens

```yaml
spacing_tokens:
  space_0: "0"
  space_1: "0.25rem"
  space_2: "0.5rem"
  space_3: "0.75rem"
  space_4: "1rem"
  space_5: "1.25rem"
  space_6: "1.5rem"
  space_8: "2rem"
  space_10: "2.5rem"
  space_12: "3rem"
  space_16: "4rem"
  space_20: "5rem"
```

`space_1` 到 `space_3` 用于紧凑控件内部，`space_4` 到 `space_6` 用于卡片和表单内部，`space_10` 到 `space_20` 用于页面区块之间。

## Radius Tokens

```yaml
radius_tokens:
  radius_none: "0"
  radius_sm: "0.25rem"
  radius_md: "0.375rem"
  radius_lg: "0.5rem"
  radius_xl: "0.75rem"
  radius_2xl: "1rem"
  radius_full: "9999px"
```

- `radius_full` 用于圆形图标控件和 pill badge。
- `radius_md` 或 `radius_lg` 用于媒体卡片、输入框和小面板。
- `radius_xl` 只用于较大的分组表面。

## Shadow Tokens

```yaml
shadow_tokens:
  shadow_none: "none"
  shadow_sm: "0 1px 2px rgba(17, 24, 39, 0.08)"
  shadow_md: "0 4px 10px rgba(17, 24, 39, 0.12), 0 0 0 1px rgba(207, 216, 227, 0.5)"
  shadow_lg: "0 14px 32px rgba(17, 24, 39, 0.16)"
  shadow_focus: "0 0 0 3px rgba(15, 118, 110, 0.35), 0 2px 8px rgba(17, 24, 39, 0.12)"
```

## Layer Tokens

```yaml
layer_tokens:
  z_base: 0
  z_dropdown: 100
  z_sticky: 200
  z_overlay: 300
  z_modal: 400
  z_toast: 500
```

只在需要解释堆叠、focus 和模态优先级时使用 elevation。避免每张卡片都堆叠装饰性阴影。

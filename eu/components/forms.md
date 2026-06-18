# Forms

## FormField

```yaml
name: "FormField"
purpose: "Collect a single user input with clear labeling and feedback."
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
  - "Validate on blur for simple fields and on submit for dependent fields."
  - "Keep helper and error text in the same location."
accessibility:
  - "Use visible label connected to input."
  - "Connect errors with aria-describedby."
  - "Do not use placeholder as the only label."
do:
  - "Write recovery-focused error text."
dont:
  - "Do not remove typed input after validation errors."
```

## SearchInput

```yaml
name: "SearchInput"
purpose: "Help users find content, products, documents, or commands."
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
  - "Submit on enter when a query exists."
  - "Show loading state while fetching suggestions."
  - "Provide clear button after text entry."
accessibility:
  - "Use search landmark for global search."
  - "Announce suggestion counts when suggestions update."
do:
  - "Offer scoped filters only when they improve results."
dont:
  - "Do not require advanced options for basic search."
```

## VariantSelector

```yaml
name: "VariantSelector"
purpose: "Let users choose product, plan, format, or configuration variants."
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
  - "Disable unavailable variants while explaining why."
  - "Update dependent price or media immediately."
accessibility:
  - "Use radio group semantics for single selection."
do:
  - "Keep selected state visible."
dont:
  - "Do not encode selection by color alone."
```

## CheckoutStep

```yaml
name: "CheckoutStep"
purpose: "Represent a step in a purchase, signup, or setup flow."
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
  - "Allow users to return to editable completed steps."
  - "Preserve entered data when navigation changes."
accessibility:
  - "Expose current step and completed status in text."
do:
  - "Show clear next action."
dont:
  - "Do not hide blocking errors at the bottom of long forms."
```

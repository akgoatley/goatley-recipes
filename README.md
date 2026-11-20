# Goatley Recipes

A family recipe collection stored as XML files, styled for viewing in a browser.

## Layout

- `Meals/`, `Slow cooker/`, `Sweet/`, `Other/`: recipes grouped by category. Most are `.xml`; a few are still `.rtf`.
- `zz-TEMPLATE.xml`: blank recipe template.
- `zz-recipe-style.css`: stylesheet the XML files use (each folder has its own copy so the relative `href` works).
- `00-BUILD-RECIPE.html`: open in a browser to fill in a form and generate a recipe's XML.

## Recipe format

```xml
<recipe>
  <title>…</title>
  <notes>…</notes>      <!-- optional -->
  <serves>…</serves>    <!-- optional -->
  <prep>…</prep>        <!-- optional -->
  <ingredients>
    <i><q>quantity</q><n>ingredient</n></i>
  </ingredients>
  <method>
    <s>step</s>
  </method>
</recipe>
```

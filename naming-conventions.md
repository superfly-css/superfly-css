# Naming Conventions

## Component Class Names

### Syntax

`.[namespace-]ComponentName[_descendant|--modifier][.onState]`

### Examples

``` css
.fs-Button {} /* Component */
.fs-Button_price {} /* Descendant */
.fs-Button--default {} /* Modifier */
.fs-Button--default.onHover {} /* Hover state */
```
## Component Variable Names

### Syntax

`--[namespace-]ComponentName[_descendant|--modifier][.onState]-(cssProperty|variableName)`

### Examples

``` css
--fs-Button-font: inherit; /* Inherit button font family */
--fs-Button-border-color: current-color; /* Use the text color for the border */
--fs-Button_price-text-color: light-gray; /* Text color for the price descendant */
--fs-Button--default-background-color: red; /* Modifier */
--fs-Button--default.onDisabled-opacity /* Disabled button opacity setting */
```
## Utility Names

### Syntax

`u-[xs-|sm-|md-|lg-|xl-]utilityName`

### Examples

``` css
.u-flex {
  display: flex !important;
}

.u-flexInline {
  display: inline-flex !important;
}
```

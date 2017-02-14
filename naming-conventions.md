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

### Example

``` css
.fs-Button {} /* Component */
.fs-Button_price {} /* Descendant */
.fs-Button--default {} /* Modifier */
.fs-Button--default.onHover {} /* Hover state */
```

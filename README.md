# superfly-css

Modularized and responsive CSS components, utilities, typography, their foundation, and corresponding structural, build, and test methodology.

## Objectives

The aim of [superfly-css](https://github.com/superfly-css/superfly-css) is to maximize designer and developer productivity by providing:
- A robust CSS foundation / base
- Small focused CSS modules that are easily customizable, adhere to a [Module philosophy](https://github.com/substack/browserify-handbook#module-philosophy), and are free of [side effects](https://philipwalton.com/articles/side-effects-in-css/)
- Dependency management for CSS modules and build tools
- Test cases clearly illustrating how to utilize the css module features and how to got about customization
- The ability to incorporate future CSS specification features, such as variables, now using [PostCSS](https://github.com/postcss/postcss).
- Naming and structural conventions for CSS elements, components, utilities, and repositories
- End to end Gulp based build pipeline examples
- Well documented and tested code that incorporates design rationale
- A standardized [project layout](https://github.com/superfly-css/superfly-css-pli) for all project repositories
- [Gulp](http://gulpjs.com) tasks providing workflow automation

## Installation

### CSS Modules

The **superfly-css** css modules can be installed via NPM.  For example install the color module as a `dev` dependency by running:

```console
npm install --save-dev superfly-css-variables-colors
```  

### Gulp Build Tasks

The **superfly-css** [Gulp](http://gulpjs.com) tasks can be installed via NPM.  To install the [`superfly-css-task-test`](https://github.com/superfly-css/superfly-css-task-test) gulp task as a development dependency run:
```console
npm install --save-dev superfly-css-task-test
```

## Usage

### CSS Modules

Import the module using `@import <module_name>`.  For example:
```css
@import superfly-css-variables-colors;
```

Then customize by overriding CSS variables and/or extending the CSS.  Once your CSS file is complete, build by setting up your `gulpfile.js` and running:

```console
gulp build:css
```  

### Build Tasks

Once the task is NPM installed require it in the `gulpfile.js` file like this:
`require(<name_of_task>)`

For example:
```js
require('superfly-css-task-build');
```

Your css can now be built by running:
```console
gulp build:css
```

### Foundation

All superfly-css modules assume the utilization of the [superfly-css-foundation](https://github.com/superfly-css/superfly-css-foundation) module in order to keep code [DRY](https://en.wikipedia.org/wiki/Don't_repeat_yourself).  Thus in order to guarantee consistent results always include the [superfly-css-foundation](https://github.com/superfly-css/superfly-css-foundation) module import first.


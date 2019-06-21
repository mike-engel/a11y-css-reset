# a11y-css-reset

> Global CSS rules to improve accessibility in your site and make your life easier

Included are three stylesheets you can include in your sites. One is strictly best practice CSS rules for accessibility, and another is what I consider to be best practices for starting development. The third combines them into a single stylesheet. These are meant to be used with the CSS [`@import` at-rule](https://developer.mozilla.org/en-US/docs/Web/CSS/@import).

This project is available on npm and [unpkg](https://unpkg.com/) so things should be fast as well as versioned! For more info about versioning, read the [examples](https://unpkg.com/#examples) section of unpkg's website.

## Usage

### accessibility only

If you just want some CSS rules focused on accessibility, include the `a11y` stylesheet _before_ any other CSS rules you write. You can see the current ruleset deployed by opening the url for [a11y.css](https://unpkg.com/a11y-css-reset/a11y.css);

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hey y'all</title>
    <link rel="stylesheet" href="https://unpkg.com/a11y-css-reset/a11y.css" />
    <link rel="stylesheet" href="main.css" />
  </head>
  <body>
    <h1>Hi 👋</h1>
  </body>
</html>
```

```css
@import url("https://unpkg.com/a11y-css-reset/a11y.css");

/* more rules here! */
ul {
  list-style-type: disc;
}
```

### reset only

If you just want some CSS rules focused on providing a better out-of-the-box dev experience, include the `reset` stylesheet _before_ any other CSS rules you write. You can see the current ruleset deployed by opening the url for [reset.css](https://unpkg.com/a11y-css-reset/reset.css);

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hey y'all</title>
    <link rel="stylesheet" href="https://unpkg.com/a11y-css-reset/reset.css" />
    <link rel="stylesheet" href="main.css" />
  </head>
  <body>
    <h1>Hi 👋</h1>
  </body>
</html>
```

```css
@import url("https://unpkg.com/a11y-css-reset/reset.css");

/* more rules here! */
ul {
  list-style-type: disc;
}
```

### the combo

If you just both the `reset` and `a11y` stylesheets, include the `combo` stylesheet _before_ any other CSS rules you write. You can see the current ruleset deployed by opening the url for [combo.css](https://unpkg.com/a11y-css-reset/combo.css);

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Hey y'all</title>
    <link rel="stylesheet" href="https://unpkg.com/a11y-css-reset/combo.css" />
    <link rel="stylesheet" href="main.css" />
  </head>
  <body>
    <h1>Hi 👋</h1>
  </body>
</html>
```

```css
@import url("https://unpkg.com/a11y-css-reset/combo.css");

/* more rules here! */
ul {
  list-style-type: disc;
}
```

### Via JS

If you are able to include CSS from within your javascript files through something like webpack, this project is also available from npm. Unlike the CSS at-rule, this does _not_ need to come before any other rules. It should be near the top due to the cascading nature of CSS, however.

```js
import "~a11y-css-reset/a11y.css";
import "~a11y-css-reset/reset.css";
import "~a11y-css-reset/combo.css";
```

## Contibuting

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

Issues and pull requests are welcome, but because this is an interview test project, I may not respond and/or merge PRs.

This project is pure CSS—no preprocessing, no development environment to setup, nada! Just plain ol' CSS.

## [License](LICENSE.md)

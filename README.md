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

## Contributing

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

Issues and pull requests are welcome!.

This project is pure CSS—no preprocessing, no development environment to setup, nada! Just plain ol' CSS.

## [License](LICENSE.md)

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="https://www.mike-engel.com"><img src="https://avatars0.githubusercontent.com/u/464447?v=4" width="100px;" alt="Mike Engel"/><br /><sub><b>Mike Engel</b></sub></a><br /><a href="#question-mike-engel" title="Answering Questions">💬</a> <a href="https://github.com/mike-engel/a11y-css-reset/issues?q=author%3Amike-engel" title="Bug reports">🐛</a> <a href="https://github.com/mike-engel/a11y-css-reset/commits?author=mike-engel" title="Code">💻</a> <a href="#review-mike-engel" title="Reviewed Pull Requests">👀</a> <a href="#maintenance-mike-engel" title="Maintenance">🚧</a> <a href="#infra-mike-engel" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#example-mike-engel" title="Examples">💡</a> <a href="https://github.com/mike-engel/a11y-css-reset/commits?author=mike-engel" title="Documentation">📖</a> <a href="#ideas-mike-engel" title="Ideas, Planning, & Feedback">🤔</a></td>
    <td align="center"><a href="https://github.com/lukehler"><img src="https://avatars0.githubusercontent.com/u/25492369?v=4" width="100px;" alt="Luke Ehler"/><br /><sub><b>Luke Ehler</b></sub></a><br /><a href="https://github.com/mike-engel/a11y-css-reset/commits?author=lukehler" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/qpowell"><img src="https://avatars2.githubusercontent.com/u/1351050?v=4" width="100px;" alt="Quinten Powell"/><br /><sub><b>Quinten Powell</b></sub></a><br /><a href="https://github.com/mike-engel/a11y-css-reset/commits?author=qpowell" title="Documentation">📖</a></td>
    <td align="center"><a href="https://gitlab.com/toastal"><img src="https://avatars2.githubusercontent.com/u/561087?v=4" width="100px;" alt="toastal"/><br /><sub><b>toastal</b></sub></a><br /><a href="https://github.com/mike-engel/a11y-css-reset/commits?author=toastal" title="Code">💻</a></td>
    <td align="center"><a href="http://notiv.org/"><img src="https://avatars0.githubusercontent.com/u/10743009?v=4" width="100px;" alt="Mikhail Novikov"/><br /><sub><b>Mikhail Novikov</b></sub></a><br /><a href="https://github.com/mike-engel/a11y-css-reset/commits?author=notiv-nt" title="Code">💻</a></td>
    <td align="center"><a href="http://www.offirmo.net/"><img src="https://avatars0.githubusercontent.com/u/603503?v=4" width="100px;" alt="offirmo"/><br /><sub><b>offirmo</b></sub></a><br /><a href="#ideas-Offirmo" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/mike-engel/a11y-css-reset/commits?author=Offirmo" title="Code">💻</a></td>
  </tr>
</table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

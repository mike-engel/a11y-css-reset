# Changelog

## Unreleased

## 1.2.0

### New features

- `border-box` is now easier to override [#10](https://github.com/mike-engel/a11y-css-reset/issues/10), [#12](https://github.com/mike-engel/a11y-css-reset/issues/12)

## 1.1.1

### Fixes

- Increase browser support by using `::` over `:` for pseudo-selectors [#6](https://github.com/mike-engel/a11y-css-reset/pull/6)
- Change the body height to be a `min-height` instead of `height` for better flexibility [#7](https://github.com/mike-engel/a11y-css-reset/pull/7)

## 1.1.0

### New features

- Adds `scroll-behavior` for reduced motion users [#2](https://github.com/mike-engel/a11y-css-reset/pull/2)

### Fixes

- Removes extraneous `width: 100%` for `body` elements [#2](https://github.com/mike-engel/a11y-css-reset/pull/2)
- Fixes a typo in the README [#1](https://github.com/mike-engel/a11y-css-reset/pull/1)

## 1.0.1

Publish all files instead of ones that weren't git-ignored.

## 1.0.0

Nothing new here, just a 1.0 release. Enjoy!

## 1.0.0-rc3

### Fixes

- Limit the amount that `.plain-list` resets

## 1.0.0-rc2

### New features

- Add a11y helper classes
- Add minified versions of each css file

### Fixes

- Remove hand-made combo.css and add code to automatically generate it

## 1.0.0-rc1

Initial release! Includes the `a11y`, `reset`, and `combo` stylesheets.

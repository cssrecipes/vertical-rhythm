# Vertical Rhythm

> Flexible CSS vertical rhythm

## Install

```console
$ npm install cssrecipes-vertical-rhythm
```

## Usage

Import `index.css` (or just files you want) & don't forget import a ratio as well.  
(**Right now, the only ratio available is _minor third_**, feel free to add more with a PR).

```css
@import "./node_modules/cssrecipes-vertical-rhythm/index.css";
@import "./node_modules/cssrecipes-vertical-rhythm/lib/ratio/minor-third.css";
```

Then use `.cssr-VerticalRhythm` on your `<html>` (or anywhere you want)

```html
<!doctype html>
<html class="cssr-VerticalRhythm">
/* ... */
</html>
```

### Defined custom properties

You can obviously override of the lib, but here is only what you should consider

```css
:root {
  --cssr-fontSizeRatio: 1;
  --cssr-fontSizeUnit: 1rem;
  /* fontSizeRatio x fontSizeUnit = fontSize) */

  --cssr-lineHeight: calc(var(--cssr-fontSize) * 1.5625); /* your line height */
  --cssr-capHeight: calc(var(--cssr-fontSize) * 0.75); /* adjust according to your font */
}
```

#### All availables custom props

- `--cssr-fontSizeRatio`
- `--cssr-fontSizeUnit`
- `--cssr-fontSize`
- `--cssr-lineHeight`
- `--cssr-capHeight`
- `--cssr-gutter-y`
- `--cssr-gutter-x`
- `--cssr-gutter`
- `--cssr-VerticalRhythm-ratio`
- `--cssr-h1-fontSize`
- `--cssr-h1-lines`
- `--cssr-h1-lineHeight`
- `--cssr-h1-baseLineDistance`
- `--cssr-h1-paddingTop`
- `--cssr-h1-marginBottom`
- `--cssr-h2-fontSize`
- `--cssr-h2-lines`
- `--cssr-h2-lineHeight`
- `--cssr-h2-baseLineDistance`
- `--cssr-h2-paddingTop`
- `--cssr-h2-marginBottom`
- `--cssr-h3-fontSize`
- `--cssr-h3-lines`
- `--cssr-h3-lineHeight`
- `--cssr-h3-baseLineDistance`
- `--cssr-h3-paddingTop`
- `--cssr-h3-marginBottom`
- `--cssr-h4-fontSize`
- `--cssr-h4-lines`
- `--cssr-h4-lineHeight`
- `--cssr-h4-baseLineDistance`
- `--cssr-h4-paddingTop`
- `--cssr-h4-marginBottom`
- `--cssr-h5-fontSize`
- `--cssr-h5-lines`
- `--cssr-h5-lineHeight`
- `--cssr-h5-baseLineDistance`
- `--cssr-h5-paddingTop`
- `--cssr-h5-marginBottom`
- `--cssr-h6-fontSize`
- `--cssr-h6-lines`
- `--cssr-h6-lineHeight`
- `--cssr-h6-baseLineDistance`
- `--cssr-h6-paddingTop`
- `--cssr-h6-marginBottom`
- `--cssr-small-fontSize`

**Please look the source to see what rules are defined before using this lib ;)**

### Helper

Attach the class `.cssr-VerticalRhythm-helper` to `<html>` to get a visual helper (horizontal lines) to make adjustements for existing content.

You can override the following defaults values to change the appearance of the lines

```css
:root {
  --cssr-VerticalRhythm-helper-color: rgba(0, 0, 0, .25);
  --cssr-VerticalRhythm-helper-color--light: color(var(--cssr-VerticalRhythm-helper-color) alpha(- 33%));
  --cssr-VerticalRhythm-helper-color--lighter: color(var(--cssr-VerticalRhythm-helper-color) alpha(- 66%));
}
```

---

## Testing

To generate a build:

```console
$ npm run build
```

To generate the testing build.

```console
$ npm run build-test
```

Basic visual tests are in `test/index.html`.

## Contributing

Work on a branch, install dev-dependencies, respect coding style & run tests before submitting a bug fix or a feature.

```console
$ git clone https://github.com/cssrecipes/vertical-rhythm.git
$ git checkout -b patch-1
$ npm install
$ npm test
```

## [Changelog](CHANGELOG.md)

## [License](LICENSE)

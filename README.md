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

Then use `.r-VerticalRhythm` on your `<html>` (or anywhere you want)

```html
<!doctype html>
<html class="r-VerticalRhythm">
/* ... */
</html>
```

### Defined custom properties

You can obviously override of the lib, but here is only what you should consider

```css
:root {
  --r-fontSizeRatio: 1;
  --r-fontSizeUnit: 1rem;
  /* fontSizeRatio x fontSizeUnit = fontSize) */

  --r-lineHeight: calc(var(--r-fontSize) * 1.5625); /* your line height */
  --r-capHeight: calc(var(--r-fontSize) * 0.75); /* adjust according to your font */
}
```

#### All availables custom props

- `--r-fontSizeRatio`
- `--r-fontSizeUnit`
- `--r-fontSize`
- `--r-lineHeight`
- `--r-capHeight`
- `--r-gutter-y`
- `--r-gutter-x`
- `--r-gutter`
- `--r-VerticalRhythm-ratio`
- `--r-h1-fontSize`
- `--r-h1-lines`
- `--r-h1-lineHeight`
- `--r-h1-baseLineDistance`
- `--r-h1-paddingTop`
- `--r-h1-marginBottom`
- `--r-h2-fontSize`
- `--r-h2-lines`
- `--r-h2-lineHeight`
- `--r-h2-baseLineDistance`
- `--r-h2-paddingTop`
- `--r-h2-marginBottom`
- `--r-h3-fontSize`
- `--r-h3-lines`
- `--r-h3-lineHeight`
- `--r-h3-baseLineDistance`
- `--r-h3-paddingTop`
- `--r-h3-marginBottom`
- `--r-h4-fontSize`
- `--r-h4-lines`
- `--r-h4-lineHeight`
- `--r-h4-baseLineDistance`
- `--r-h4-paddingTop`
- `--r-h4-marginBottom`
- `--r-h5-fontSize`
- `--r-h5-lines`
- `--r-h5-lineHeight`
- `--r-h5-baseLineDistance`
- `--r-h5-paddingTop`
- `--r-h5-marginBottom`
- `--r-h6-fontSize`
- `--r-h6-lines`
- `--r-h6-lineHeight`
- `--r-h6-baseLineDistance`
- `--r-h6-paddingTop`
- `--r-h6-marginBottom`
- `--r-small-fontSize`

**Please look the source to see what rules are defined before using this lib ;)**

### Helper

Attach the class `.r-VerticalRhythm-helper` to `<html>` to get a visual helper (horizontal lines) to make adjustements for existing content.

You can override the following defaults values to change the appearance of the lines

```css
:root {
  --r-VerticalRhythm-helper-color: rgba(0, 0, 0, .25);
  --r-VerticalRhythm-helper-color--light: color(var(--r-VerticalRhythm-helper-color) alpha(- 33%));
  --r-VerticalRhythm-helper-color--lighter: color(var(--r-VerticalRhythm-helper-color) alpha(- 66%));
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

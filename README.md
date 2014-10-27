# Vertical Rhythm

> Flexible CSS vertical rhythm

## Install

```sh
$ npm install cssrecipes-vertical-rhythm
```

## Usage

Import `index.css` (or just files you want) & don't forget import a ratio as well.  
(**Right now, the only ratio available is _minor third_**, feel free to add more with a PR).

```css
@import "./path/to/cssrecipes-vertical-rhythm/index.css";
@import "./path/to/cssrecipes-vertical-rhythm/lib/ratio/minor-third.css";
```

### Helper

Attach the class `cssr-VerticalRhythm-helper` to `<html>` to get a visual helper (horizontal lines) to make adjustements for existing content.

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

```sh
$ npm run build
```

To generate the testing build.

```sh
$ npm run build-test
```

Basic visual tests are in `test/index.html`.

## Contributing

Work on a branch, install dev-dependencies, respect coding style & run tests before submitting a bug fix or a feature.

```sh
$ git clone https://github.com/cssrecipes/vertical-rhythm.git
$ git checkout -b patch-1
$ npm install
$ npm test
```

## [Changelog](CHANGELOG.md)

## [License](LICENSE)

# Vertical Rhythm

> Flexible CSS vertical rhythm

## Install

    npm install cssrecipes-vertical-rhythm

## Usage

Import `index.css` (or just files you want) & don't forget import a ratio as well.  
(**Right now, the only ratio available is _minor third_**, feel free to add more with a PR).

```css
@import "./path/to/cssrecipes-vertical-rhythm/index.css";
@import "./path/to/cssrecipes-vertical-rhythm/ratio/minor-third.css";
```

### Helper

Attach the class `rcp-VerticalRhythm-helper` to `<html>` to get a visual helper (horizontal lines) to make adjustements for existing content.

You can override the following defaults values to change the appearance of the lines

```css
:root {
  --rcp-VerticalRhythm-helper-color: rgba(0, 0, 0, .25);
  --rcp-VerticalRhythm-helper-color--light: color(var(--rcp-VerticalRhythm-helper-color) alpha(- 33%));
  --rcp-VerticalRhythm-helper-color--lighter: color(var(--rcp-VerticalRhythm-helper-color) alpha(- 66%));
}
```

## [Changelog](CHANGELOG.md)

## [License](LICENSE)

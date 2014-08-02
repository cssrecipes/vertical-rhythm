# Vertical Rhythm

> Flexible CSS vertical rhythm

## Install

    npm install cssrecipes-vertical-rhythm

## Usage

First import a chosen ratio, then the `index.css` (or just files you want).
(Right now, the only ratio available is _minor third_).

```css
@import "./path/to/vertical-rhythm/ratio/minor-third.css";
@import "./path/to/vertical-rhythm/index.css";
```

### Helper

Attach the class `VerticalRhythmHelper` to `<html>` to get a visual helper (horizontal lines) to make adjustements for existing content.

You can override the following defaults values to change the appearance of the lines

```css
:root {
  --VerticalRhythm-helper-color: rgba(0, 0, 0, .25);
  --VerticalRhythm-helper-color--light: color(var(--VerticalRhythm-helper-color) alpha(- 33%));
  --VerticalRhythm-helper-color--lighter: color(var(--VerticalRhythm-helper-color) alpha(- 66%));
  --VerticalRhythm-helper-backgroundColor: #fff;
  --VerticalRhythm-helper-lineHeight: var(--lineHeight);
}
```

## [Changelog](CHANGELOG.md)

## [License](LICENSE-MIT)

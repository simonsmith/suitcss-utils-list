# SUIT CSS utilities: list

[![Build Status](https://travis-ci.org/simonsmith/suitcss-utils-list.svg?branch=master)](https://travis-ci.org/simonsmith/suitcss-utils-list)

SUIT CSS list utilities

* Read more about [SUIT CSS's design principles](https://github.com/suitcss/suit/).

## Installation

* [npm](http://npmjs.org/): `npm install suitcss-utils-list`
* Download: [zip](https://github.com/simonsmith/suitcss-utils-list/releases/latest)

## Available classes

* `u-listReset` - Remove default margin and padding
* `u-listIndent` - Set the left indent. Default is `40px` as found in browser
  defaults
* `u-listNone` - Remove list style
* `u-listBullet` - Bulleted list using `disc` style type
* `u-listBulletNested` - Bulleted list using `circle` style type
* `u-listSquare` - Square list style
* `u-listNumber` - Numbered list using `decimal` style type

### Configuration

The indent size can be changed:

```css
:root {
  --list-indentSize: 25px;
}
```

## Usage

```html
<ul class="u-listIndent u-listBullet">
  <li>An item</li>
  <li>
    <ul class="u-listBulletNested">
      <li>Nested item</li>
    </ul>
  </li>
</ul>
```

Please refer to the README for [SUIT CSS utils](https://github.com/suitcss/utils/)

## Testing

Install [Node](http://nodejs.org) (comes with npm).

```
npm install
```

To generate a build:

```
npm run build
```

To lint code with [postcss-bem-linter](https://github.com/postcss/postcss-bem-linter) and [stylelint](http://stylelint.io/)

```
npm run lint
```

To generate the testing build.

```
npm run build-test
```

To watch the files for making changes to test:

```
npm run watch
```

Basic visual tests are in `test/index.html`.

## Browser support

* Google Chrome
* Opera
* Firefox
* Safari
* Internet Explorer 8+
* Android 4.1+
* iOS 6+
* Windows phone 8.1+

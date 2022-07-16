# twotip

`twotip` is a minimal CSS tooltip library.

## Installation

**With npm**

```sh
npm install twotip
```

**With yarn**

```sh
yarn add twotip
```

**With pnpm**

```sh
pnpm add twotip
```

**With CDN**

```sh
<link rel="stylesheet" href="https://unpkg.com/twotip/twotip.min.css">
```

## Setup

**With PostCSS**

```scss
@import "twotip";
```

**With Vite/Webpack**

```js
import "tooltip";
```

## Usage

Simply add a `data-tt="tooltip message"` attribute to the element on which the
tooltip should appear. For example:

```html
<button data-tt="This is a tooltip">Click me!</button>
```

### Positioning Tooltip

You can change the position of the tooltip by adding a `data-tt-pos` attribite
with one of the following values: `top`, `bottom`, `left` or `right`. For
example:

```html
<button data-tt="This is a tooltip" data-tt-pos="right">Click me!</button>
```

### Static Tooltip

If you want your tooltip to be always visible add a `data-tt-open` attribute:

```html
<button data-tt="Always open" data-tt-open>Click me!</button>
```

### Customizing Tooltip

You can use CSS variables to customize your tooltip:

| CSS Variable    | Description                      | Default |
| --------------- | -------------------------------- | ------- |
| `--tt-bg`       | Background color of the tooltip  | `#333`  |
| `--tt-fg`       | Text color of the tooltip        | `#fff`  |
| `--tt-padding`  | Padding of the tooltip           | `0.3em` |
| `--tt-radius`   | Border radius of the tooltip     | `0.2em` |
| `--tt-delay`    | Delay before tooltip appears     | `0.1s`  |
| `--tt-duration` | Duration of the appear animation | `0.15s` |

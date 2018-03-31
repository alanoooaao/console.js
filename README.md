# [console.js](https://github.com/yanhaijing/console.js) [![](https://img.shields.io/badge/Powered%20by-jslib%20base-brightgreen.svg)](https://github.com/yanhaijing/jslib-base) [![npm](https://img.shields.io/badge/npm-0.5.0-orange.svg)](https://www.npmjs.com/package/@yanhaijing/console_js) [![Build Status](https://travis-ci.org/yanhaijing/console.js.svg?branch=master)](https://travis-ci.org/yanhaijing/console.js) [![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/yanhaijing/console.js/blob/master/LICENSE)

console.js is a small javascript library. Fix console is undefined, similar to HTML5 Shim and reset.css.

In IE6 and IE7, console is undefined. In IE8 and IE9, first open the developer tools before, console is undefined.

## How to Use
Download and install using npm:

```bash
$ npm install --save @yanhaijing/console_js
```

If you use webpack:

```js
import { polyfill } from '@yanhaijing/console_js';

polyfill(); // polyfill console undefined
```

If you use requirejs:

```js
requirejs(['node_modules/@yanhaijing/console_js/dist/index.aio.js'], function (console_js) {
    var polyfill = console_js.polyfill;

    polyfill(); // polyfill console undefined
})
```

If you use a browser:

```html
<script src="node_modules/@yanhaijing/console_js/dist/index.aio.js"></script>

<script>
    var polyfill = console_js.polyfill;
    
    polyfill(); // polyfill console undefined
</script>
```

## Document
[API](https://github.com/yanhaijing/console.js/blob/master/doc/api.md)

## Principle & Blog
[use console.js](http://yanhaijing.com/js/2014/11/03/use-console.js/)

## Contribution Guide
For first time contributors, you need to install the dependencies first.

```bash
$ npm install
```

To build the project:

```bash
$ npm run build
```

To run unit tests：

```bash
$ npm test
```
* Note: The browser environment needs to be tested manually under ```test/browser```

Modify the version number in package.json, modify the version number in README.md, modify the CHANGELOG.md, and then release the new version.

```bash
$ npm run release
```

Publish the new version to NPM:

```bash
$ npm publish --access=public
```
You may need to modify the following files in your project：

- README.md
- package.json
- config/rollup.js
- test/browser/index.html

## CHANGELOG
[CHANGELOG.md](https://github.com/yanhaijing/console.js/blob/master/CHANGELOG.md)

## TODO
[TODO.md](https://github.com/yanhaijing/console.js/blob/master/TODO.md)

## Who use

## Reference
- [MSDN](http://msdn.microsoft.com/en-us/library/ie/gg589530.aspx)
- [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Console)
- [Firebug](http://getfirebug.com/wiki/index.php/Console_API)

## Related Projects
- [browser-shim](https://github.com/ishmaelthedestroyer/browser-shim)
- [console-shim(liamnewmarch)](https://github.com/liamnewmarch/console-shim)
- [console-shim(kayahr)](https://github.com/kayahr/console-shim)
- [console-polyfill](https://github.com/paulmillr/console-polyfill)
- [consolex.js](https://github.com/deadlyicon/consolex.js/blob/master/src/consolex.js)

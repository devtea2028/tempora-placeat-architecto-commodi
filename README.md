# @devtea2028/tempora-placeat-architecto-commodi <sup>[![Version Badge][2]][1]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][5]][6]
[![dev dependency status][7]][8]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][11]][1]

Gets the description of a Symbol. Handles `Symbol()` vs `Symbol('')` properly when possible.

## Example

```js
var getSymbolDescription = require('@devtea2028/tempora-placeat-architecto-commodi');
var assert = require('assert');

assert(getSymbolDescription(Symbol()) === undefined);
assert(getSymbolDescription(Symbol('')) === ''); // or `undefined`, if in an engine that lacks name inference from concise method
assert(getSymbolDescription(Symbol('foo')) === 'foo');
assert(getSymbolDescription(Symbol.iterator) === 'Symbol.iterator');
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[1]: https://npmjs.org/package/@devtea2028/tempora-placeat-architecto-commodi
[2]: https://versionbadg.es/inspect-js/@devtea2028/tempora-placeat-architecto-commodi.svg
[5]: https://david-dm.org/inspect-js/@devtea2028/tempora-placeat-architecto-commodi.svg
[6]: https://david-dm.org/inspect-js/@devtea2028/tempora-placeat-architecto-commodi
[7]: https://david-dm.org/inspect-js/@devtea2028/tempora-placeat-architecto-commodi/dev-status.svg
[8]: https://david-dm.org/inspect-js/@devtea2028/tempora-placeat-architecto-commodi#info=devDependencies
[11]: https://nodei.co/npm/@devtea2028/tempora-placeat-architecto-commodi.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2028/tempora-placeat-architecto-commodi.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2028/tempora-placeat-architecto-commodi.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2028/tempora-placeat-architecto-commodi
[codecov-image]: https://codecov.io/gh/inspect-js/@devtea2028/tempora-placeat-architecto-commodi/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@devtea2028/tempora-placeat-architecto-commodi/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@devtea2028/tempora-placeat-architecto-commodi
[actions-url]: https://github.com/devtea2028/tempora-placeat-architecto-commodi/actions

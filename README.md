# WIF

[![TRAVIS](https://secure.travis-ci.org/dcousens/WIF.png)](http://travis-ci.org/dcousens/WIF)
[![NPM](http://img.shields.io/npm/v/WIF.svg)](https://www.npmjs.org/package/WIF)

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

Bitcoin Wallet Import Format encoding/decoding module.


## Example

``` javascript
var wif = require('wif')

var d = new Buffer('0000000000000000000000000000000000000000000000000000000000000001')

wif.encode(128, d, true)
// => KwDiBf89QgGbjEhKnhXJuH7LrciVrZi3qYjgd9M7rFU73sVHnoWn

wif.decode(128, 'KwDiBf89QgGbjEhKnhXJuH7LrciVrZi3qYjgd9M7rFU73sVHnoWn')
// => {
//	version: 128,
//	d: <Buffer 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 01>,
//	compressed: true
//}
```

## LICENSE [MIT](LICENSE)

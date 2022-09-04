# word2number_turkish

[![npm version](https://badge.fury.io/js/word2number_turkish.svg)](//npmjs.com/package/word2number_turkish)

It is a Javascript library that converts numbers written with words to digits.

## Installation

```
npm install --save word2number_turkish
```

## Usage

```js
const word2Number = require("word2number_turkish");
console.log(word2Number.convert("yüzaltmışyedi"));
```

You can extract numbers' indexes from sentences.
```js
const word2Number = require("word2number_turkish");
let words = word2Number.splitSentenceToWords("sekizyüz on iki milyar üç yüz kırk dört milyon beşyüz yetmişikibin dörtyüz bir lira otuz iki kuruş");
console.log(word2Number.findNumbersIndexes(words));
// Output: [ { startIndex: 0, endIndex: 17 }, { startIndex: 19, endIndex: 20 } ]
```


## To Do

- [x] Handling all written numbers.
- [x] Handling phone numbers.
- [x] Handling zero number.
- [x] Handling numbers that next to each other.
- [x] Handling both numeric and written numbers.
- [x] Handling Dates.
- [x] Handling Decimal numbers.
- [x] Fuzzy matching.
- [ ] Handling half numbers.


#### Unit Test Status

**Total**: 41

39 success, 2 fail

![95%](https://progress-bar.dev/95)

## Author

**Ender CAN**

- <https://github.com/endrcn>
- <https://twitter.com/endrcn>

## License

Open sourced under the [MIT license](LICENSE).

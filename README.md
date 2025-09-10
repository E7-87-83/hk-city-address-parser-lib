# 香港城市地址解析器 Hong Kong City Address Parser Lib

This is a fork and continued development of [香港地址解析器 Hong Kong Address Parser Lib](https://github.com/g0vhk-io/hk-address-parser-lib).

The original Hong Kong Address Parser Lib has been paused development for more than 5 years.

Hong Kong Address Parser Lib was the JavaScript Address Resolver library for [Hong Kong Address Parser](https://g0vhk-io.github.io/HKAddressParser).

For their details, see [https://g0vhk-io.github.io/hk-address-parser-lib](https://g0vhk-io.github.io/hk-address-parser-lib)

## Installation

```bash
npm i hk-city-address-parser-lib 
```

## Usage
```bash
node test.mjs
```

Content of test.mjs:

```javascript

// import AddressResolver from 'hk-city-address-parser-lib';
import AddressResolver from './dist/hk-address-parser.cjs.js';
...

const records = await AddressResolver.parse("address to search");
records.forEach(address => {
  //
})
```

## License

MIT

## Python Fork of "Hong Kong Address Parser"

https://github.com/wingkwong/hk-address-parser


## About the Hong Kong Address Parser

### Contributers of "Hong Kong Address Parser"

* Brian Leung (@cswbrian)
* Nandi Wong (@nandiheath)
* Wong Wing Kam (@wingkwong)
* Kan Omar (@oktak)
* Law Wai Chun (@chunlaw)
* Chai (@ylchan87)
* UnKnoWn-Consortium (@UnKnoWn)

### Special Thanks of "Hong Kong Address Parser"

* HoLok Chen
* Ho Wa Wong (@howawong)
* Ng Benny
* Lam Wai
* Himphen Hui Hau Him (@himphen)
* Ha Chi Yeung
* Samson Lau
* Carrie Lau
* Gemini Cheng
* Sze Ching Wee
* Yat Tin Sunny Chan
* Eric Yuen. Lun

## About the Hong Kong City Address Parser

### Maintainer

* Cheok Yin Fung (@E7-87-83)

### TODO

* OGCIO no longer exists; modify related codes
* Finish Documentation (including History)

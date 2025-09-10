## Example

with ES6 import syntax:

```javascript

import AddressResolver from 'hk-city-address-parser-lib';

const records = await AddressResolver.parse("麥花臣球場");
for (const record of records) {
  console.log(record.coordinate());
  console.log(record.fullAddress(AddressResolver.Address.LANG_ZH));
}

/*
  { lat: 22.3501, lng: 114.1274 }
  新界葵涌荔景足球場    #錯誤地址
  { lat: 22.3187, lng: 114.1729 }
  奶路臣街   38號       #正確地址
  { lat: 22.3182, lng: 114.1728 }
  九龍旺角洗衣街59號    #正確地址
  ...
*/

const myRecords = await AddressResolver.parse("綠在佐敦");
const [firstRecord] = myRecords;
console.log(firstRecord.coordinate());
// { lat: 22.4681, lng: 114.2094 }
console.log(firstRecord.fullAddress(AddressResolver.Address.LANG_ZH));
// 佐敦偉晴街14-18號偉晴閣地下1-3號舖
console.log(firstRecord.fullAddress(AddressResolver.Address.LANG_EN));
// Shop 1-3, G/F, Wai Ching Court, 14-18 Wai Ching Street, Jordan
```

# jsonaky - update and extend json file

## Installation
` $ npm install jsonaky`

## API
**jsonaky(filepath, data[, options], callback)**
+ filepath String
+ data String | Buffer
+ options Object
  + encoding String | Null default = 'utf8'
  + replacer Function | Null default = null
  +	space: Number | Null default = null
+ callback Function
```js
var jsonaky = require('jsonaky');

jsonaky('metadata.json', {
  compile_css: {
    run: false,
    time: 1405213450
  }
}, function(err, data) {
  console.log('json saved: ', data);
});
```

## Authors

**xmhscratch**

+ http://github.com/xmhscratch

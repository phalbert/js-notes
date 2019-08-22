# `typeof()`

Return type of a variable

```javascript
typeof(1); // 'number'

typeof(true) // 'boolean'

typeof('hello') // 'string'

typeof(function(){}) // 'function'

typeof({}) // 'object'

//this is controversial..some expect typeof(null) to return 'null'
typeof(null) //  'object'

typeof(undefined) // 'undefined'

// its a number because its assumes some type of numerical operation went wrong but still a number was expected
typeof(NaN) // 'number'
```

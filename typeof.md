# `typeof()` and conversions btn types

## Return type of a variable

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

## Common conversion types

```javascript
//convert to string
let foo = 9
foo.toString(); // '9'

//convert string to integer
Number.parseInt('8') // 8

//this still works; as soon as a non-number is encountered, parsing stops
Number.parseInt('859pod') // 859
Number.parseInt('85u9pod') // 85
Number.parseInt('799.90') // 799

//however if you begin with a non-number, an error is thrown
Number.parseInt('ha4') // NaN - Not a Number

//convert string to float
Number.parseFloat('799.90') // 799.9
```

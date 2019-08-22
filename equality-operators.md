# Equality Operators

Below js tries to convert the types to be the same before the comparison i.e. '4' is converted to an int and so the comparison will be true

```javascript
4 == '4' // true

4 != '4' // false
```

However in when using identity comparison, js will do a strict equality check for identity by comparing both the value and type

```javascript
4 === '4' // false

4 !== '4' // true
```

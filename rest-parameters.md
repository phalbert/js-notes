# Rest parameters

Store multiple arguments in an array. Useful when one is not sure beforehand how many arguments are needed.

```javascript
function sendCars(...allCars){
    allCars.forEach(id => console.log(id))
}

sendCars(['monday',2,3,4,4])
```

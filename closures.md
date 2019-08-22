# Closures

```javascript
let app = (function(){
  let car = 123
  let getId = function(){
    return car;
  }
  return {
    getId: getId,
    car: car
  }
})();

console.log(app.getId()) // 123
console.log(app.car) // 123
```

# Destructuring Arrays

Destructuring is a quick way of assigning array elements to variables. 

```javascript
function sendCars(...allCars){
let carIds = [100,200,400];

//destructure 
let [car1, car2, car3] = carIds;

console.log(car1, car2, car3); // 100 200 400

//destructure with rest parameters
let [car4, ...rest] = carIds;
console.log(car4, ...rest); // 100 200 400

//skip first parameter when destructuring
//first element skipped
let [, ...others] = carIds;
console.log(...others); // 200 400
console.log(others); // [ 200, 400 ]
```

Always use `[]` when destructuring arrays

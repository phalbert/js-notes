# Destructuring

## Arrays

Destructuring can be used as a quick way of assigning array elements to variables.

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

## Objects

### Method 1

```javascript
//create object
let car = {id: 1, make: "toyota" };

//destructure
let {id, make} = car;
console.log(id, make); // 1 'toyota'
```

### Method 2

```javascript
//destructure with definition, then init
let car = {id: 1, make: "toyota" };

let id, make;

//initialise
{id, make} = car; // SyntaxError: Unexpected token (11:11)

// curly braces are also used for code blocks so interpreter is confused: are u destructuring or starting a code block.

//solution: put destructuring statement in parenthesis
({id, make} = car);
console.log(id, make)
```

Always use `{}` when destructuring objects

> NB: Destructured variable names ought to be similar to object attribute names, otherwise `undefined` is returned

```javascript
let car = {id: 1, make: "toyota" };

//destructure
let {car_id, car_make} = car;
console.log(car_id, car_make); // undefined undefined
```

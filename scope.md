# Scope

## Function Scope

```javascript
function startCar(card){
  let message = 'Starting...'
  let startFn = function turnKey(){
    let message = 'Override';
    console.log(message)
  }
  startFn();
  console.log(message)
}

startCar(12)

console.log(message) //out of scope
```

## Block Scope

Lifetime of variables as they exist within curly braces

```javascript
if(5 == 5){
  var message = 'Equal' // var hoists values, so no scope when using var
  let value = 'Value' //use let keyword for block scope
}

console.log(message) // 'Equal'
console.log(value) // ReferenceError: value is not defined
```

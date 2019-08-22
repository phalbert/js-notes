# Spread syntax

Take an array and spread out its elements so that they are assigned to parameters. This is the opposite of the rest parameters

```javascript
function sendCars(a, b, c){
    console.log(a, b, c)
}

let array = ['monday',2,3,4,4]
sendCars(...array) // 'monday' 2 3

let array2 = [2,3,4,5]
sendCars(...array2) // 2 3 4

let array3 = 'abc'
sendCars(...array3) // 'a' 'b' 'c'
```

Combining spread syntax and rest parameters

```javascript
//add a rest parameter
//you can use spread and rest at the same time

function printOut(a, b, c, ...others){
    console.log(a, b, c, others)
}

let list = ['tue','wed','thur','fri','sat']
printOut(...list) // 'tue' 'wed' 'thur' [ 'fri', 'sat' ]
```

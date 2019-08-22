# Prototypes


```javascript
function Car(id){
  this.carId = id
  this.start = _ => `start ${this.carId}`
}

let car = new Car(5)
car.start()
```

If you were to instantiate a 1000 copies of `Car`, 100 copies of the function `start` would be created. This is inefficient and affects performance. Using prototypes, we ensure that only one copy `start` is created no matter how many objects of `Car`

```javascript
function Car(id){
  this.carId = id
}

Car.prototype.start = function() {
  console.log('start ' + this.carId)
}

let car = new Car(5)
car.start()
```

## Expand objects using prototypes

Expand object functionality by adding functions to object prototypes

```javascript
String.prototype.hello = function(){
  return this.toString() + ' hello'
}

'foo'.hello()
```

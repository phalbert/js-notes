# Constructors

Way of defining objects before classes were introduced in ES16

```javascript
function Car(id){
  this.carId = id
  this.start = _ => `start ${this.carId}`
}

let car = new Car(5)
car.start()
```

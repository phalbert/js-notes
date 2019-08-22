# Classes

Alternative to constructors

```javascript
class Car {
  
}

let car = new Car()
console.log(car) // Car {}
```

## Constructors

Instantiate class with attribute values

```javascript
class Car {
   constructor(id, color='black'){
       this.id = id
       this.color = color
   }
}

let car = new Car(4)
console.log(car)
```

## Methods

```javascript
class Car {
   constructor(id, color='black'){
       this.id = id
       this.color = color
   }
  
  //no need for function keyword for class methods
  identify(){
    return `Car ${this.id}`
  }
}

let car = new Car(4)
console.log(car.identify())
```

## Inheritance

```javascript
class Vehicle{
  constructor(){
    this.type = 'car'
  }
  
  start(){
    return `Starting ${this.type}`
  }
}

class Car extends Vehicle{
  start(){
    return 'in car start ' + super.start()
  }
}

let car = new Car()
car.start() // 'in car start Starting car'
```

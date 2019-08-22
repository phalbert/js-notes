# Array iteration

```javascript
let cars = [  { car: 'sedan', mileage: 344},
  { car: 'audi', mileage: 433},
  { car: 'chevrolet', mileage: 792}
]

cars.forEach(car => console.log(car))

cars.forEach((car, index) => console.log(car, index))
```
```bash
{ car: 'sedan', mileage: 344 }
{ car: 'audi', mileage: 433 }
{ car: 'chevrolet', mileage: 792 }
```

```javascript
//filtering
let beasts = cars.filter(
  car => car.mileage > 600
)
console.log(beasts) // [ { car: 'chevrolet', mileage: 792 } ]
```

```bash
{ car: 'sedan', mileage: 344 } 0
{ car: 'audi', mileage: 433 } 1
{ car: 'chevrolet', mileage: 792 } 2
```

```javascript
//testing
// does every object have a mileage greater than 600
let check = cars.every(
  car => car.mileage > 600
)
console.log(check) // false

//locate first match
let car = cars.find(
  car => car.mileage > 400
)
console.log(car) // { car: 'audi', mileage: 433 }
```
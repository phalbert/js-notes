# JSON

## Moving Javascript objects over the network

```javascript
let car = {
  id: 123,
  style: 'blue'
}

let json = JSON.stringify(car)
console.log(json) // '{"id":123,"style":"blue"}'
```

## Arrays

```javascript
let carIds = [
  { car: 'sedan', mileage: 344},
  { car: 'audi', mileage: 433},
  { car: 'chevrolet', mileage: 792}
]

let json = JSON.stringify(carIds)

console.log(json) // '[{"car":"sedan","mileage":344},{"car":"audi","mileage":433},{"car":"chevrolet","mileage":792}]'
```

## Parsing JSON

```javascript
let json = '[{"car":"sedan","mileage":344, "color": "blue"},{"car":"audi","mileage":433},{"car":"chevrolet","mileage":792,"service":{"name":"washing","cost": 345000}}]'

let cars = JSON.parse(json)
console.log(cars)
```

# Immediately Invokable Function Expression

```javascript
//IIFE
(function(){
  console.log('in func')
})() //'in func'

let app = function(){
  let car = 123
  console.log('in func')
  return {}
}

console.log(app) // [Function: app]
```

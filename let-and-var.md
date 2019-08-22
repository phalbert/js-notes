# `let` and `var`

1. `let` has block scope while `var` doesnt

```javascript
const card = 42;
...
card = 45; //TypeError: Assignment to constant variable.
```

2. `let` helps you catch errors earlier. Doesnt allow one to use undefined variables 

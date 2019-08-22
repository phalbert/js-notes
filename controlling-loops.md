# Controlling Loops

```javascript
let i = 0
for(;i<4;i++){
  console.log(i)
}

for(let k=0;k<4;k++){
  console.log(k)
}
```

## `continue`

```javascript
//continue helps you stop executing the body but go ahead and continue as though the body had completed
for(let i = 0;i<4;i++){
  console.log(i)
  continue
  console.log("skipped")
}
```

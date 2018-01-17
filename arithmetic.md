## Arithmetic

#### Max values
Find the max value in an array of values
```javascript
// a basic function
function findMax(input){
    var max = input[0];
    for(i=0;i<input.length;i++){
        if(input[i] >= max){
            max = input[i];
        }
    }
    return max;
}

var numbers = [-1,-5,-17,-9];

// using custom function
console.log(findMax(numbers));

// using Math
console.log(Math.max.apply(null,numbers));

// using Math ES2015
console.log(Math.max(...numbers));
```

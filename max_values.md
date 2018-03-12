## Arithmetic

#### Max values
Find the max value in a list of values with python:
```py
# python
numbers = [-1,-5,-17,-9]

# the easiest method is to use max()
print(max(numbers))

# a custom function
def findMax(input):
    max = input[0]
    for item in input:
        if item > max:
            max = item
    return max
print(findMax(numbers))
```

Find the max value in a list of values with javascript:
```javascript
// a basic javascript function
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

# Challenges

## 1. Easy mathematical callback

Write the processArray function, which takes an array and a callback function as parameters. The callback function can be, for example, a mathematical function that will be applied on each element of this array. Optionally, also write tests similar to the examples below.

### Examples

1. Array `[4, 8, 2, 7, 5]` after processing with function

```javascript
var myArray = [4, 8, 2, 7, 5];
myArray = processArray(myArray, function (a) {
  return a * 2;
});
```

will be `[ 8, 16, 4, 14, 10 ].`

2. Array `[7, 8, 9, 1, 2]` after processing with function

```javascript
var myArray = [7, 8, 9, 1, 2];
myArray = processArray(myArray, function (a) {
  return a + 5;
});
```

will be `[ 12, 13, 14, 6, 7 ].`

## 2. Moving Zeros To The End

Write an algorithm that takes an array and moves all of the zeros to the end, preserving the order of the other elements.

```javascript
moveZeros([false, 1, 0, 1, 2, 0, 1, 3, "a"]); // returns[false,1,1,2,1,3,"a",0,0]
```

## 3. Valid Parentheses

Write a function that takes a string of parentheses, and determines if the order of the parentheses is valid. The function should return true if the string is valid, and false if it's invalid.

### Examples

```
"()"              =>  true
")(()))"          =>  false
"("               =>  false
"(())((()())())"  =>  true
```

### Constraints

`0 <= input.length <= 100`

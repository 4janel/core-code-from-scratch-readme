# Moving Zeros To The End

## Description

Write an algorithm that takes an array and moves all of the zeros to the end, preserving the order of the other elements.

```javascript
moveZeros([false, 1, 0, 1, 2, 0, 1, 3, "a"]); // returns[false,1,1,2,1,3,"a",0,0]
```

## Solution

```javascript
function moveZeros(nums) {
  let nonZero = nums.filter((val) => val !== 0);
  let zeros = nums.filter((val) => val === 0);
  return nonZero.concat(zeros);
}
```

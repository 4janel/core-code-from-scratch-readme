# Bit counting

## Description

Write a function that takes an integer as input, and returns the number of bits that are equal to one in the binary representation of that number. You can guarantee that input is non-negative.

### Example

The binary representation of `1234` is `10011010010`, so the function should return `5` in this case.

## Solution

```javascript
var countBits = function (n) {
  let binaryNumber = n.toString(2);
  let oneBitCount = 0;
  for (let i = 0; i < binaryNumber.length; i++) {
    if (binaryNumber[i] === "1") oneBitCount++;
  }
  return oneBitCount;
};
```

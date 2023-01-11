# String: indexOf()

## Description

Write a function `indexOfIgnoreCase` taking two strings and determining the first occurrence of the second string in the first string. The function should be case insensitive.

Example: `indexOfIgnoreCase('bit','it')` and `indexOfIgnoreCase('bit','IT')` should return `1`.

## Solution

```javascript
function indexOfIgnoreCase(str1, str2) {
  let str1Lower = str1.toLowerCase();
  let str2Lower = str2.toLowerCase();
  return str1Lower.indexOf(str2Lower);
}
```
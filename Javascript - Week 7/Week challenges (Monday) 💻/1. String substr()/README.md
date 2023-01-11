# String: substr()

## Description

Write a function `firstWord`, taking a string and returning the first word in that string. The first word are all characters up to the first space.

Example: `firstWord('see and stop'`) should return `'see'`.

## Solution

```javascript
function firstWord(str) {
  return str.substring(0, str.indexOf(" "));
}
```
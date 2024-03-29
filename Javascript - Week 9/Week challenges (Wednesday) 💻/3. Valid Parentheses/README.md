# Valid Parentheses

## Description

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

## Solution

```javascript
function validParentheses(str) {
  return (
    str.split("").reduce((acc, val) => {
      if (val === "(") {
        acc++;
      } else if (val === ")") {
        acc--;
        if (acc < 0) {
          acc = NaN;
        }
      }
      return acc;
    }, 0) === 0
  );
}
```

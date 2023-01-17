# 1. Even or odd

## Description

Create a function that takes an integer as an argument and returns `"Even"` for even numbers or `"Odd"` for odd numbers.
and return a string like this:

`"This white dog has 4 legs."`

## Solution

```javascript
function evenOrOdd(number) {
  return number % 2 === 0 ? "Even" : "Odd";
}
```
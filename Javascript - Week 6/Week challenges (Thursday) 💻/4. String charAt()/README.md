# String: charAt()

## Description

Write a function `shortcut` that takes two strings and returns the initial letters of theses strings.

Example: `shortcut('Amnesty', 'International')` should return `'AI'`.

## Solution

```javascript
function shortcut(str1, str2) {
  return str1.charAt(0) + str2.charAt(0);
}
```
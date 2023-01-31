# Convert string to camel case

## Description

Complete the method/function so that it converts dash/underscore delimited words into [camel casing](https://en.wikipedia.org/wiki/Camel_case). The first word within the output should be capitalized only if the original word was capitalized (known as Upper Camel Case, also often referred to as Pascal case). The next words should be always capitalized.

### Examples

`"the-stealth-warrior"` gets converted to `"theStealthWarrior"`
`"The_Stealth_Warrior"` gets converted to `"TheStealthWarrior"`

## Solution

```javascript
function toCamelCase(str) {
  if (str === "") return "";
  let words = str.split("");
  return words.reduce((acc, val, i) => {
    if (val === "-" || val === "_") {
      return acc + words[i + 1].toUpperCase();
    } else {
      return acc + val;
    }
  }, words[0]);
}
```

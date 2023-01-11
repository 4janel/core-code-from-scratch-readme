# Return to sanity

## Description

This function should return an object, but it's not doing what's intended. What's wrong?

```javascript
function mystery() {
  var results = { sanity: "Hello" };
  return;
  results;
}
```

## Solution

```javascript
function mystery() {
  var results = { sanity: "Hello" };
  return results;
}
```
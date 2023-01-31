# The Hashtag Generator

## Description

The marketing team is spending way too much time typing in hashtags.
Let's help them with our own Hashtag Generator!

Here's the deal:

- It must start with a hashtag (`#`).
- All words must have their first letter capitalized.
- If the final result is longer than 140 chars it must return `false`.
- If the input or the result is an empty string it must return `false`.

### Examples

```
" Hello there thanks for trying my Kata"  =>  "#HelloThereThanksForTryingMyKata"
"    Hello     World   "                  =>  "#HelloWorld"
""                                        =>  false
```

## Solution

```javascript
function generateHashtag(str) {
  if (str.length === 0) return false;
  let hashtag = str
    .split(" ")
    .reduce(
      (acc, val) => (acc += val.charAt(0).toUpperCase() + val.slice(1)),
      "#"
    );
  if (hashtag.length > 140) return false;
  return hashtag;
}
```

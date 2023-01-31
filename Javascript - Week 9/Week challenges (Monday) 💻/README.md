# Challenges

## 1. "this" is a problem

We want to create a constructor function 'NameMe', which takes first name and last name as parameters. The function combines the first and last names and saves the value in "name" property.

We already implemented that function, but when we actually run the code, the "name" property is accessible, but the "firstName" and "lastName" is not accessible. All the properties should be accessible. Can you find what's wrong with it? A test fixture is also available

```javascript
function NameMe(first, last) {
  this.firstName = first;
  this.lastName = last;
  return { name: this.firstName + " " + this.lastName };
}

var n = new NameMe("John", "Doe");
n.firstName; //Expected: John
n.lastName; //Expected: Doe
n.name; //Expected: John Doe
```

## 2. Thinkful - List and Loop Drills: Lists of lists

You have a two-dimensional list in the following format:

```javascript
data = [
  [2, 5],
  [3, 4],
  [8, 7],
];
```

Each sub-list contains two items, and each item in the sub-lists is an integer.

Write a function `process_data()`/`processData()` that processes each sub-list like so:

- `[2, 5]` --> `2 - 5` --> `-3`
- `[3, 4]` --> `3 - 4` --> `-1`
- `[8, 7]` --> `8 - 7` --> `1`

and then returns the product of all the processed sub-lists:
`-3 * -1 * 1` --> `3`.

For input, you can trust that neither the main list nor the sublists will be empty.

## 3. Stop gninnipS My sdroW!

Write a function that takes in a string of one or more words, and returns the same string, but with all five or more letter words reversed (Just like the name of this Kata). Strings passed in will consist of only letters and spaces. Spaces will be included only when more than one word is present.

### Examples:

```javascript
spinWords( "Hey fellow warriors" ) => returns "Hey wollef sroirraw"
spinWords( "This is a test") => returns "This is a test"
spinWords( "This is another test" )=> returns "This is rehtona test"
```

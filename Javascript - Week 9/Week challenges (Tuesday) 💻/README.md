# Challenges

## 1. "this" is an other problem

Having created a function `NamedOne` which takes `first` & `last` names as parameters and returns an object with `firstName`, `lastName` and `fullName` ( = `firstName` + a space + `lastName` ) properties which should be all **accessibles**, we discovered that "accessible" also means "mutable".

If, for example, we've got a "NamedOne" like this:

```javascript
var namedOne = new NamedOne("Naomi", "Wang");
namedOne.firstName; // -> "Naomi"
namedOne.lastName; // -> "Wang"
namedOne.fullName; // -> "Naomi Wang"
```

...properties may be **changed**:

```javascript
namedOne.firstName = "John";
namedOne.firstName; // -> "John"
namedOne.lastName = "Doe";
namedOne.lastName; // -> "Doe"
```

...but **all** properties are not **updated**!

```javascript
namedOne.fullName; // -> "Naomi Wang"
//-- Oh no ! we want fullName == "John Doe" now !
```

### Your mission

So the purpose of this kata is to create an object with accessible **and** **"updatable"** (can i say that?) properties.

- If `.firstName` or `.lastName` are changed, then `.fullName` should also be changed
- If `.fullName` is changed, then `.firstName` and .lastName should also be changed.

**Note:** "input format" to `.fullName` will be `firstName + space + lastName.` If given fullName isn't valid then no property is changed.

### Examples

```javascript
var namedOne = new NamedOne("Naomi", "Wang");

namedOne.firstName = "John";
namedOne.lastName = "Doe";
// ...then...
namedOne.fullName; // -> "John Doe"

// -- And :
namedOne.fullName = "Bill Smith";
// ...then...
namedOne.firstName; // -> "Bill"
namedOne.lastName; // -> "Smith"

// -- But :
namedOne.fullName = "Tom"; // -> no : lastName missing
namedOne.fullName = "TomDonnovan"; // -> no : no space between first & last names
namedOne.fullName; // -> "Bill Smith" (unchanged)
```

Can you change our function to create such a `NamedOne` object ?

## 2. "Who likes it?"

You probably know the "like" system from Facebook and other pages. People can "like" blog posts, pictures or other items. We want to create the text that should be displayed next to such an item.

Implement the function which takes an array containing the names of people that like an item. It must return the display text as shown in the examples:

```
[]                                -->  "no one likes this"
["Peter"]                         -->  "Peter likes this"
["Jacob", "Alex"]                 -->  "Jacob and Alex like this"
["Max", "John", "Mark"]           -->  "Max, John and Mark like this"
["Alex", "Jacob", "Mark", "Max"]  -->  "Alex, Jacob and 2 others like this"
```

**Note:** For 4 or more names, the number in `"and 2 others"` simply increases.

## 3. Convert string to camel case

Complete the method/function so that it converts dash/underscore delimited words into [camel casing](https://en.wikipedia.org/wiki/Camel_case). The first word within the output should be capitalized only if the original word was capitalized (known as Upper Camel Case, also often referred to as Pascal case). The next words should be always capitalized.

### Examples

`"the-stealth-warrior"` gets converted to `"theStealthWarrior"`
`"The_Stealth_Warrior"` gets converted to `"TheStealthWarrior"`

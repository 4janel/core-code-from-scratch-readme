# Challenges

## 1. Count strings in objects

Create a function strCount (takes an object as argument) that will count all string values inside an object. For example:

```javascript
strCount({
  first: "1",
  second: "2",
  third: false,
  fourth: ["anytime", 2, 3, 4],
  fifth: null,
});
//returns 3
```

## 2. Extending JavaScript Objects: Get First & Last Array Element

Your task is to extend JavaScript Array object, with methods `.first()` and `.last()`, so you can get respectively first or last element of the array.

```javascript
var a = [2, 5, 7, 3, 4];

a.first(); // 2
a.last(); // 4
```

**Note:** in case of empty array, methods should return `undefined`.

## 3. Object Oriented Piracy

You have access to the ship `draft` and `crew`. `Draft` is the total ship weight and `crew` is the number of humans on the ship.

Each crew member adds `1.5` units to the ship draft. If after removing the weight of the crew, the draft is still more than `20`, then the ship is worth looting. Any ship weighing that much must have a lot of booty!

Add the method

```
isWorthIt
```

to decide if the ship is worthy to loot. For example:

```
titanic.isWorthIt() // return false
This Kata teaches you the very basics of method creation.
```

Good luck!
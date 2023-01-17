# Challenges

## 1. Even or odd

Create a function that takes an integer as an argument and returns `"Even"` for even numbers or `"Odd"` for odd numbers.

## 2. A wolf in sheep's clothing

Wolves have been reintroduced to Great Britain. You are a sheep farmer, and are now plagued by wolves which pretend to be sheep. Fortunately, you are good at spotting them.

Warn the sheep in front of the wolf that it is about to be eaten. Remember that you are standing **at the front of the queue** which is at the end of the array:

```
[sheep, sheep, sheep, sheep, sheep, wolf, sheep, sheep]      (YOU ARE HERE AT THE FRONT OF THE QUEUE)
   7      6      5      4      3            2      1
```

If the wolf is the closest animal to you, return `"Pls go away and stop eating my sheep"`. Otherwise, return `"Oi! Sheep number N! You are about to be eaten by a wolf!"` where `N` is the sheep's position in the queue.

**Note:** there will always be exactly one wolf in the array.

### Examples

Input: `["sheep", "sheep", "sheep", "wolf", "sheep"]`
Output: `"Oi! Sheep number 1! You are about to be eaten by a wolf!"`

Input: `["sheep", "sheep", "wolf"]`
Output: `"Pls go away and stop eating my sheep"`

## 3. Decode the morse code

In this kata you have to write a simple [Morse code](https://en.wikipedia.org/wiki/Morse_code) decoder. While the Morse code is now mostly superseded by voice and digital data communication channels, it still has its use in some applications around the world.
The Morse code encodes every character as a sequence of "dots" and "dashes". For example, the letter `A` is coded as `·−`, letter `Q` is coded as `−−·−`, and digit `1` is coded as `·−−−−`. The Morse code is case-insensitive, traditionally capital letters are used. When the message is written in Morse code, a single space is used to separate the character codes and 3 spaces are used to separate words. For example, the message `HEY JUDE` in Morse code is `···· · −·−−   ·−−− ··− −·· ·`.

**NOTE:** Extra spaces before or after the code have no meaning and should be ignored.

In addition to letters, digits and some punctuation, there are some special service codes, the most notorious of those is the international distress signal [SOS](https://en.wikipedia.org/wiki/SOS) (that was first issued by [Titanic](https://en.wikipedia.org/wiki/Titanic)), that is coded as `···−−−···`. These special codes are treated as single special characters, and usually are transmitted as separate words.

Your task is to implement a function that would take the morse code as input and return a decoded human-readable string.

For example:

```javascript
decodeMorse(".... . -.--   .--- ..- -.. .");
//should return "HEY JUDE"
```

**NOTE:** For coding purposes you have to use ASCII characters `.` and `-`, not Unicode characters.

The Morse code table is preloaded for you as a dictionary, feel free to use it:

* Coffeescript/C++/Go/JavaScript/Julia/PHP/Python/Ruby/TypeScript: `MORSE_CODE['.--']`
* C#: `MorseCode.Get(".--")` (returns `string`)
* F#: `MorseCode.get ".--"` (returns `string`)
* Elixir: `@morse_codes` variable (from `use MorseCode.Constants`). Ignore the unused variable warning for `morse_codes` because it's no longer used and kept only for old solutions.
* Elm: `MorseCodes.get : Dict String String`
* Haskell: `morseCodes ! ".--"` (Codes are in a `Map String String`)
* Java: `MorseCode.get(".--")`
* Kotlin: `MorseCode[".--"] ?: ""` or `MorseCode.getOrDefault(".--", "")`
* Racket: `morse-code` (a hash table)
* Rust: `MORSE_CODE`
* Scala: `morseCodes(".--")`
* Swift: `MorseCode[".--"] ?? ""` or `MorseCode[".--", default: ""]`
* C: provides parallel arrays, i.e. `morse[2] == "-.-"` for `ascii[2] == "C"`
* NASM: a table of pointers to the morsecodes, and a corresponding list of ascii symbols
  
All the test strings would contain valid Morse code, so you may skip checking for errors and exceptions. In C#, tests will fail if the solution code throws an exception, please keep that in mind. This is mostly because otherwise the engine would simply ignore the tests, resulting in a "valid" solution.

Good luck!
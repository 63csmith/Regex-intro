# REGEX INTRO

"Regular expression is not a library nor is it a programming language. Instead, regular expression is a sequence of characters that specifies a search pattern in any given text (string). A text can consist of pretty much anything from letters to numbers, space characters to special characters.
Introductory paragraph."
-First search result of google

## Summary

We will be going over the basic components of Regex an what they are used for. Regex or regular expression is used as a search tool to find and even edit returned information. Something that is great about Regex is it available in almost every programing language. For the purpose of this example I will be showing you code snippets in Vanilla Javascript.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

- Regex has basic syntax that starts with everything between two forward slashes /

- In the image below it shows more quick symbols and what they will target.
  ![alt text](/assets/images/regex-cheatsheet.jpg)

### Anchors

- Anchors match a position rather than a single character.

- The ^ and $ characters are anchors that fix a match to the beginning or end of a line of text.
- Example
  ```
  /^$/
  ```

### Quantifiers

- Quantifiers tell how many instances of a character must be present for there to be a positive match.

- Example

```
/x*/ matches x 0 or more times
/x+/ matches x 1 or more times
```

### Grouping Constructs

- This will help us put a set group of characters into a search
- Example

```
(the) is now saved together and will be pulled from any word containing the
```

### Bracket Expressions

- Bracket expressions help with returning a wide range of results
- The best Example is [a-z]

```
[a-z] will return any letter in the alphabet
[3-9] will return any number between 3 and 9
```

### Character Classes

- Character classes or character sets help match a few characters at a time
- Example

```
[ae] can be used to select a or e out of a word
gr[ae]y to return gray or grey depending on the different spelling
```

### The OR Operator

- The OR operator is used to provide options between two or more stings
- Example

```
/(cats|dogs)/ this will return either cats or dogs if it is in the given information

I like cats and I also like dogs
Returned = cats & dogs

```

### Flags

- Flags are used outside of the slashes to determine the scale at which you want to parse your information.
- Example

```
//g will provide a global search
//i will provide a Case insensitive search
//m will provide a multi line search
these flags can be stacked
//ig will be a combo of global an case insensitive search


```

-Flags

![alt text](/assets/images/slide-7.jpg)

### Character Escapes

- The back slash is used \ to turn off the default function of a variable that you would be able to use.
- Example

```
(/$) would escape the normal /$/ function (end of line +) and searches for the dollar sign($)
```

## Author

Please contact me with any questions.

-GitHub:https://github.com/63csmith

-Email: 63csmith@gmail.com

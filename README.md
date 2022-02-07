# Regular Expressions (RegExp)

Regular expressions, otherwise known as 'regex', is a method used in various languages including JavaScript which find patterns in a text. It's used mostly to validate a user input and to search through a body of text.

## Summary

There are two ways of creating a new RegExp object, by using the literal syntax, or by using the `RegExp()` constructor.

The literal syntax `(/pattern/)` uses forward slashes to wrap the regular expression pattern and does not use quotation marks, whereas the constructor syntax `("pattern")` uses quotation marks and is not enclosed between slashes.

One way Regex could be used is to validate user input.

I'll be using this line of code throughout my tutorial:

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
```

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

### Anchors

An Anchor in regex shows the position of the beginning of the string and its ending .

The caret `^` is positioned before the first character in the string. For example in our line of code:

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
```

the caret could be found after the forward slash used in the literal syntax indicating that the string starts from the opening parenthesis and not at the beginning of the line of code.

Similarly, the dollar sign `$` shows the ending of the string and is to be found at the end of the code line.

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

Character classes are what we call the square brackets that surround a string/ pattern of characters. The character class always matches at least one of the characters found inside the square brackets.
For example in our code, there are 3 character class instances `([\da-z\.-]+)`, `([a-z\.]{2,6})`, `([\/\w \.-]*)`. For each of these character class contents at least one of its letters or numbers matches the original url string.

We could further break down the code inside the square brackets:

- `[abc]` -> Matches any one of these characters a, b or c.
- `[^abc]` -> Matches any other character apart from a, b or c.
- `[a-z]` -> Matches any character from lowercase a to lowercase z.
- `[A-Z]` -> Matches any character from uppercase A to uppercase Z.
- `[a-Z]` -> Matches any character from lowercase a to uppercase Z.
- `[0-9]` -> Matches any single digit from 0-9.
- `[a-z 0-9]` -> Matches a single character from a-z or 0-9.

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

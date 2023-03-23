# Regular Expression 

A Regular Expression is a special sequence of characters that help a user match or find strings (or sets of strings), using a special syntax. It is one of the most powerful concept used for pattern matching within strings. Hence, it is very important to know various Special Characters, Quantifiers, and Anchors that form part of regular expressions. 

## Summary

This series of characters might look like nonsense, but it’s actually a search pattern meant for basic username validation. That is, it checks to see if a string fulfills the requirements for a basic username. In a nutshell, here’s how it breaks down (we’ll explore it in more detail later):

* The string can contain any lowercase letter between a–z

* The string can contain any number between 0–9

* The string can contain an underscore or hyphen

* The string is between 3–16 characters long


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)


## Regex Components

A regex is considered a literal, so the pattern must be wrapped in slash characters (/).

* /^[a-z0-9_-]{3,16}$/

### Anchors

The characters ^ and $ are both considered to be anchors. The ^ anchor signifies a string that begins with the characters that follow it

The $ anchor signifies a string that ends with the characters that precede it. Just as with the ^ character, it can be preceded by an exact string or a range of possible matches.

 * [a-z0-9_-]
 * {3,16}
 * $


### Quantifiers

All right, so now we know what we're looking for inside the brackets. Quantifiers set the limits of the string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that your regex is looking for.

* *—Matches the pattern zero or more times

* +—Matches the pattern one or more times

* ?—Matches the pattern zero or one time

* {}—Curly brackets can provide three different ways to set limits for a match:

### OR Operator

Using the OR operator (|), the expression [abc] could be written as (a|b|c). Using our example in the grouping constructs section, we can take the original expression:

* (abc):(xyz)

### Character Classes

A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match

* .—Matches any character except the newline character (\n)

* \d—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

### Flags

Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex.

* g—Global search: the regex should be tested against all possible matches in a string.

* i—Case-insensitive search: case should be ignored while attempting a match in a string

* m—Multi-line search: a multi-line input string should be treated as multiple lines

### Grouping 

The primary way you group a section of a regex is by using parentheses (()). 
 
 * (abc):(xyz)

### Bracket Expressions

Anything inside a set of square brackets ([]) represents a range of characters that we want to match. These patterns are known as bracket expressions, but they are also known as a positive character group, because they outline the characters we want to include.

* [a-z]—The string can contain any lowercase letter between a–z. Keep in mind that this looks for lowercase characters only. If we wanted to include uppercase characters, we would need to change the expression to [a-zA-Z].

* [0-9]—The string can contain any number between 0–9

### Resources 

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions

## Author

A short section about the author with a link to the author's https://github.com/Haillander

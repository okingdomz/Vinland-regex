# **Regex Tutorial** 



## Summary
---
Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
---

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

## Regex Example Below :

## *Password Parameters*
/^[a-z0-9_-&%$@!()]{8,16}$/

**Qualified passwords**
- "jonsnowww"
- "jon34snow"
- "jon34snow_"

**Not Qualified passwords**
- "Jonsnow"
- "jon sno"
- "jonsnow^istheking

### Anchors
**components of a regex**
- `$` is a common anchor that signifies a string that ends with the charcters that precede it. typically put at the end of a line.
- `^` anchor signifies a string that begins with the character that follows it. It is also case sensitive and usually put at the beginning of a line.

### Quantifiers
- Quantifiers set limits of the string that your regex matches. They typically hold the min/max number of characters that your regex is looking for.
### Grouping Constructs
- using multple parts of a string to determine how to use different constructs to break the sections up. You can use parentheses to group a section of a regex, and connecting them with a colon. Their 2 primary functions is to:
    - capturing
    - non-capturing

### Bracket Expressions
 anything inside of ([]) represents a range of charcaters that we want to match. Known as **positive character groups** because they they outline the characters we want to include.
 - [a-z] string will contain any lowercase between a-z
 - [0-9] string will include numbers between 0-9
### Character Classes
 - regex defines a set of charcaters, any one of which can occur in an input string to fulfill a match. common character classes are:
    - . = macthes any charcater except the newline character (\n)
    - \d = any number between (0-9)
    - \w = including the _ it's (a-z)
    - \s = single whitespace, including tabs and line breaks
### The OR Operator
Using the OR operator (|), the expression [abc] could be written as (a|b|c). Using our example in the grouping constructs section, we can take the original expression:
### Flags
- Placed at the end of of a regex, after the second slash. They are defined additional functionality or limites for the regex
    
    **Examples**
    - g = global search: the regex should be tested against all possible matches in a string.
    - i = Case-insensitive search: case should be ignored while attempting a match in a string
    - s = Multi-line search: a multi-line input string should be treated as multiple lines
### Character Escapes
The backslash (\) in a regex escapes a character that otherwise would be interpreted literally. For example, the open curly brace ({) is used to begin a quantifier, but adding a backslash before the open curly brace (\{) means that the regex should look for the open curly brace character instead of beginning to define a quantifier
## Author
### Robert Barnes
Full-Stack Web Developer: 
[Github](https://github.com/okingdomz/Vinland-regex).



# Regex Tutorial - Matching an Email

This tutorial is to explain how you can match an email through Regular Expression. This can be a handy tool for verifying an email has been entered correctly by checking that it fits the format of an email. The code that will be covered in this tutorial can be seen below.

Code for Matching an Email: "/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/"
Example Email: michaelengstrand1@gmail.com

## Summary

A Regular Expression, often referred to as a Regex, is a combination of characters that can be used to to create a pattern that can then be used to search, match or replace text. Regex can be used in scripting languages and some programming languages. One useful Regex is the code that was mentioned above for matching an email. This code may look like someone just smashed a bunch of random keys on their keyboard, but that is not the case. This tutorial will walk you through the different aspects of this Regex and help you understand what it is doing and how to implement it.

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
As the name would imply; Anchors are used to "anchor" the regex at a certain point. So these are not used to match a character, they are used to match a position. The anchors used in this Regex are "^" and "$".  The "^" matches the beginning of the text while the "$" matches the ending of the text.

### Quantifiers
Quantifiers allow the Regex to quantify how many times a part of you expression should be repeated. The quantifiers used in this Regex are "+" and "{2,6}".  the "+" operator allows us to connect groups. Using our example email, this would be something like group 1: michaelengstrand1  +  group 2: gmail  +  group 3:  com. The quantifier "{2,6}" tells the expression to match from at least 2 times but not more than 6 times

### Grouping Constructs
Grouping allows us to create a sequence or a sub expression. This is done using "( )". As seen in the quantifiers explanation, our groups in this sub expression are group 1: michaelengstrand1  +  group 2: gmail  +  group 3:  com.

### Bracket Expressions
Brackets "[ ]" are used to indicate a set of characters that we want to match. For this expression, we can see them wrapped around group 1, 2 and 3.  In group 1 we see "[a-z0-9_\.-]" which tells us :
- a-z: matches a single character in the range of a to z.
- 09: matches a single character in the range of 1 to 9
- _: matches the character  "_"
- .\: matches the character "."
- -: matches the character "-"

### Character Classes
Character classes allow us to distinguish and match certain kinds of characters. The character class used in this expression is "/d" and this will match any digit.

### Flags
Flags are optional parameters that can be used in a Regular Expression to modify the searching behavior. This expression does not include a flag.

### Character Escapes
Character escapes are used when you need to match a character that is hard to represent in its literal form.

## Author - Michael Engstrand
Here is a link to my Github: https://github.com/mikeengstrand

## Gist
Attached is a link to the gist I have created: https://gist.github.com/mikeengstrand/45ccee34f5d0983addc6a58bef82d3ad

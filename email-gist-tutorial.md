# Regex-email-gist

The purpose for the Regex-email-gist, is to break down what an email gist's specific section of code actually does. This way I can increase my knowledge and better understand what my code is doing behind the scenes.

## Summary

I will be breaking down an email-regex to better understand its functionality. This is what an email-regex looks like: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. It is extremely confusing, so that's why I'm here to break it down.

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

All of the regex components are wrapped inside of slash characters (/). As you can tell by examining the regex, the email-regex is split into three different sections. One section is before the '@,' another is right after it, then the last section is at the end. They are all wrapped inside of '()'.

### Anchors

The characters, '^' and '$' are both considered anchors. In this case the '$' is our anchor. The '$' anchor signifies a string that ends with the characters before it.

### Quantifiers

Quantifiers set the limits of the string. They set the parameters, in this case, they set the minimum and maximum number of characters that the regex is looking for. This is represented in the expression by the {2,6}.

### Grouping Constructs

To group constructs, simply wrap them inside of parentheses. The email-regex is split into 3 different grouping constructs, all easily told apart by the '()'. Each section wrapped by the parentheses are called subexpressions.

### Bracket Expressions

Characters inside of '[]' are known as bracket expressions. Anything inside of there represents a range of characters that we want to match.

### Character Classes

Character classes define a set of characters, which can occur in an input string. For example, the bracket expressions are a form of character class.

### The OR Operator

The OR operator can be used like this: '|'. The OR operator can be used inside of character classes to provide more mobility. For example, instead of (abc):(xyz), you can write (a|b|c):(x|y|z).

### Flags

Flags can be found at the end of a regex, after the second slash. They define functionality or set limits. There are six optional flags that can be used seperately or together. They can also be used in any order. A few of the most common flags are 'g', known for global search, 'i' known for case-sensitive search, and 'm' known for multi-line search.

### Character Escapes

The '\' character is the escape. This is useful if you want to search for a specific character that you are already using inside of the regex. For example, '\{', would search for the open curly brace character instead of beginning the quantifier.

## Author

My name is Zach Barnes. I am a student with the KU bootcamp for full-stack development. This is my first time writting a Regex-tutorial. 

My Github Repository - https://github.com/TooSparky/Regex-email-gist

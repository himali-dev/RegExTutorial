# Regex Tutorial

A regex, or regular expression, is a method used in JavaScript to check if a string fullfills the requirements of validation, by using a series of special characters to define a search pattern.

## Summary

This tutorial explains how to use a regex to match emails, using the expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, as an example.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#author)

## Regex Components

### Anchors

(`^`) - The caret symbol denotes the start of the string. This ensures that the email begins with the pattern specified next.

(`$`) - The dollar sign represents the end of the string. It ensures that the email address ends after the TLD.

### Quantifiers

(`+`) (plus sign): Matches one or more occurrences of the preceding element. In this regex, it applies to [a-zA-Z0-9._-], [a-zA-Z0-9.-], and [a-zA-Z]{2,}. It allows for one or more alphanumeric characters, periods, underscores, or hyphens in the local part of the email, one or more alphanumeric characters, periods, or hyphens in the domain name, and at least two alphabetic characters in the TLD.

### OR Operator
(`|`) (pipe symbol): Matches either the expression on the left or the expression on the right. It is not used in this regex.

### Character Classes
The character class in this expression, (`\d`), means that a single character matches a digit between 0-9. (`\.`) (escaped period): Matches a literal period. It is used to match the dot in the domain name.

### Flags
Flags modify the behavior of the regex pattern, such as case-insensitive matching (i flag), global matching (g flag), or multiline matching (m flag). Like the OR Operator, no flags are specified in this regex.

### Grouping and Capturing
Referring to the example: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, capturing group #1, `([a-z0-9_\.-]+)`, matches the user email name. Capturing group #2, `([\da-z\.-]+)`,matches the email service.  And capturing group #3 is `([a-z\.]{2,6})` which matches the .com.

### Bracket Expressions
Bracket expressions for email validation include the character sets of (`[a-z0-9_\.-]`), which matches any case sensitive letter between (a-z), as well as a digit between 0-9  and matches the characters "_" , "-" , and ".". (`[\da-z\.-]`), which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; (`[a-z\.]`) matches any character case senstive to (`a-z`) and the character ".".

### Greedy and Lazy Match
Because the expression includes the (`+`) and (`{}`) Quantifiers, it will match as many times as possible.

## Author
Here is the link to my github!
[https://github.com/himali-dev](https://github.com/himali-dev)

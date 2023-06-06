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
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

(`^`) - The caret symbol denotes the start of the string. This ensures that the email begins with the pattern specified next.

(`$`) - The dollar sign represents the end of the string. It ensures that the email address ends after the TLD.

### Quantifiers

(`+`) (plus sign): Matches one or more occurrences of the preceding element. In this regex, it applies to [a-zA-Z0-9._-], [a-zA-Z0-9.-], and [a-zA-Z]{2,}. It allows for one or more alphanumeric characters, periods, underscores, or hyphens in the local part of the email, one or more alphanumeric characters, periods, or hyphens in the domain name, and at least two alphabetic characters in the TLD.

### OR Operator

(`()`) (parentheses): Groups multiple elements together. In this regex, parentheses are not used for capturing groups; instead, they are used to group parts of the regex for applying quantifiers and operators.

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

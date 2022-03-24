Used for user validation (most often), but can be used to capture bad info (doesn't match format, spam/fraud)

# Title: Email Validation - Regex Expression

Introductory paragraph (replace this with your text)

## Summary

The regex expression that I will be explaining is /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, which is used to ensure that the email address a user enters is valid. I will explain how each aspect of this expression works to check the validity of the email address.

## Table of Contents

- [Title: Email Validation - Regex Expression](#title-email-validation---regex-expression)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
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
  - [Author](#author)

## Regex Components

### Anchors
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

At the beginning and end, you will notice two anchors, '^' and '$'. The '^' is always at the start of the expression, while '$' is always at the end of the expression.
### Quantifiers
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The quantifiers in this expression are '{}'. In this expression, the quantifiers are housing the "rule" that the domain of the email address (this being .com, .net, etc.) is at least 2 characters long and up to 6 characters.
### OR Operator
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

CHECK ON \.
### Character Classes
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

UNKNOWN - may not have
### Flags
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

UNKNOWN - may not have
### Grouping and Capturing

### Bracket Expressions
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The bracket expressions within this expression are encompassed in the multiple '[]' brackets. The content within the brackets state what is to be contained in the user input. If you type in an email address, based off of this expression, it can be lowercase (any letter a to z), it can have digits between zero and nine, may contain an underscore, period, or hyphen. 

REVISE
### Greedy and Lazy Match
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Boundaries
Reference: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

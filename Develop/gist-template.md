Used for user validation (most often), but can be used to capture bad info (doesn't match format, spam/fraud)

# Title: Email Validation - Regex Expression

This regex tutorial on email validation will describe how to use a regex expression to match emails. The reason that this is useful is because there may be applications that require a login or user data that requires an email address. How can we tell if someone entered an email address? We can use this regex expression: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

At the beginning and end of the expression, you will notice two anchors, '^' and '$'. The '^' is always at the start of the expression, while '$' is always at the end of the expression. They signify the beginning and end of the expression, respectively.
### Quantifiers

The quantifiers in this expression are '{}' and '+'. In this expression, the bracket quantifiers are housing the "rule" that the domain of the email address (this being .com, .net, etc.) is at least 2 characters long and up to 6 characters. The '+' quantifier is combining the email name, email service (gmail, outlook, etc.), and the .com (or .net).
### OR Operator

There are no OR operators in this expression. This would be notated by either a '|' or '[]'.
### Character Classes

The character class in this regex expression is '\d'. This class matches a single digit between zero and nine. For example, it could match '1' or '3', but if there was more than one of the same digit in a row, it would not match. So, '11' or '33' would not match. This is important because of all of the different combinations of digits that email addresses can have. 
### Flags

There are no flags in this expression. A flag is notated by a 'g', 'm', or 'i' at the end of the last '/'.
### Grouping and Capturing

This regex expression has a few different capturing groups, these being ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]{2,6}). These are identified by the parentheses surrounding them. In this expression, each capturing group handles its own task. Going in order of how they are listed above, the first group is tasked with housing the criteria that matches the user email name. Based on this group, the email name must only contain what the constraints listed in the group. The second group houses the criteria that matches the email service and has its own criteria. The third group houses the criteria that matches the .com (or others). These capture groups house the constraints of how the email address must be entered.
### Bracket Expressions

The bracket expressions within this regex expression are encompassed in the multiple '[]' brackets. The content within the brackets state what is to be contained in the user input as mentioned in the Grouping and Capturing section. If you type in an email address, based off of this expression, it can be lowercase (any letter a to z), it can have digits between zero and nine, may contain an underscore, period, or hyphen. It then must have a valid email service match and .com (or others). It is easy to think of bracket expressions as the actual criteria that must be met, while the grouping and capturing component houses these different criteria.
### Greedy and Lazy Match

The greedy match in this expression are the '+' and '{}'. These will match as many times as possible in the given input. A greedy match is repeated as many times as possible.
### Boundaries

There are no boundaries in this expression. A boundary is signified by a \b and \B.
### Back-references

There are no back-references in this expression. This would be shown as a '\1' up to '\n' or by a letter such as '\k'.
### Look-ahead and Look-behind

This expression does not have any look-ahead and look-behind contents. This would be labeled as '(?=)' or '(?<=)'.
## Author

My name is Nate Huerd and I am working my way towards becoming a full stack developer. You can see my other projects at https://github.com/Nate-Huerd.

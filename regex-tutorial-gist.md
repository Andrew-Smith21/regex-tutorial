# Regex Tutorial

Regex is an abbreviation for "regular expressions." They make it easier to search for specific 
sections of a text by describing a pattern of characters to look for. Regex can be applied to many
different programming languages, and are useful for input validation, finding and replacing characters, etc.

## Summary

A regex will be examined below that can be used to validate an email address. Each component of the regex will be explain in its corresponding section. 

Regex: Matching an Email
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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

^

`^([a-z0-9_\.-])` Matches any string that begins with the characters specified between the brackets

Example:

`^andrew-smith` This will match any string that begins with "andrew-smith"  
$

`([a-z\.]{2,6})$` Matches any string that ends with the characters specified between the brackets

Example:

`97$` This will match any string that ends with "97"

^ $

`^andrew45$` This will match only a string that is exactly "andrew45"  


### Quantifiers

\+

`([a-z0-9_\.-]+)` Matches any string that has the characters between the brackets followed by one or more characters

Example:

`charlie+` This will match any string that has "charlie" followed by at least one character  

{}

`([a-z\.]{2,6})` This will match any string that has the characters between the brackets follow by at least two and up to six characters

### Character Classes

\d

`\.` Matches a literal "." character  

Example:

`[a-z]\.[a-z]` This will match any pair of strings with a "." between them

### Grouping and Capturing

()

`([a-z0-9_\.-]+)` Groups together everything that comes before the @ symbol in our email. This allows us to manipulate this part of our data using the respective 
coding language we are using

### Bracket Expressions

[]

`[a-z0-9_\.-]` Matches a string that contains any of the specified characters between the brackets

Example:

`[a-z]` This will match a string that contains any lowercase letter from a to z

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

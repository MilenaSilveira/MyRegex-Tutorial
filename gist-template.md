# My Regex Tutorial

A Regular Expression (Regex) is a string of text that allows you to create patterns to match, find, and manage text.

## Summary

Regex can be used to match data format like Name, Email, Phone Number, Hex Value, HTML Tag, URL etc...
This document will describe the components of an Email validator:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

```
^  Will match beginning of line or text.
$  Will match end of line.
```
### Quantifiers

Quantifiers determin the amount of classes, groups or characters an input should have to match the desired search information.
There are two types of quantifiers, Greedy and Lazy.
```
*  match zero or more times
+  match one or more times
? match zero or one time
{ n }  match exactly n times
{ n, }  match at least n times
{ n, m }  match from n to m times

{?} Is added in a Lazy Quantifier.
```

### Grouping Constructs

Grouping constructs determin the subexpressions of a regular expression and capture the substrings of an input string. 
We add the expression to the open and close parentheses that identify groups.

```
() Read the information that matches what is inside the parentheses.
(?:) Disables a group inside the parentheses.
(?<>) Give a name to group inside the parentheses.
```


### Bracket Expressions

Bracket Expressions are used to determin values to be searched. 
```
[a-z]  A single character between a and z.
[cde]  Searches for c, d or e.
[0-9]  A single character between 0 and 9.
[[:alpha:]] Alphabetic order.

```
### Character Classes

Character classes are used to sort and filter.

```
\d It matches a digit.
\s It matches new lines, spaces and tabs
\w It matches a word.
. It matches any character.
```

### The OR Operator

The OR is used to find a specified expression within a variety of regular expressions.

```
| It is used to match a string.
```

### Flags

Modifies search parameters.

```
i It makes the search case sensitive.
g It makes the search find all matches, not only one result.
m It is used for multiline mode search.
u Enables unicode support.
y Enables sticky mode.

```



### Character Escapes

## Author

Milena Silveira
https://github.com/MilenaSilveira/MyRegex-Tutorial
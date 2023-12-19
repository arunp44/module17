# REGEX (an intro)

Introduction to regex. A brief explination.

## Summary

A regular expression, commonly referred to as regex or regexp, is a sequence of characters that define a search pattern. It is mainly used for text-based searching and string manipulation.
Regular expressions are often used in web development to validate user input or find specific strings of characters within larger blocks of text. They are also widely used in data science, natural language processing, and text analytics.

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
Anchors match the starting and ending points of a string or line. For example, you can use ^ to match the beginning of a string, and $ to match the end of a string.
### Quantifiers
Quantifiers allow you to specify how many of a character or character class should be matched. For example, you can use * to match zero or more occurrences of the preceding character or character class, or + to match one or more occurrences of the preceding character or character class.
### OR Operator
The or operator allows you to specify a list of values that can match a field. If any of the values matches, the entire clause is a match. Or operators can also be nested.
### Character Classes
With a “character class”, also called “character set”, you can tell the regex engine to match only one out of several characters. Simply place the characters you want to match between square brackets. If you want to match an a or an e, use [ae]. You could use this in gr[ae]y to match either gray or grey. Very useful if you do not know whether the document you are searching through is written in American or British English.
### Flags

### Grouping and Capturing
Groups allow you to match a pattern multiple times within a string, and backreferences allow you to refer back to previously matched groups.
By placing part of a regular expression inside round brackets or parentheses, you can group that part of the regular expression together. This allows you to apply a quantifier to the entire group or to restrict alternation to part of the regex.
### Bracket Expressions

### Greedy and Lazy Match

### Boundaries
he metacharacter \b is an anchor like the caret and the dollar sign. It matches at a position that is called a “word boundary”. This match is zero-length.

There are three different positions that qualify as word boundaries:

Before the first character in the string, if the first character is a word character.
After the last character in the string, if the last character is a word character.
Between two characters in the string, where one is a word character and the other is not a word character.
### Back-references
Backreferences match the same text as previously matched by a capturing group. The backreference \1 (backslash one) references the first capturing group. \1 matches the exact same text that was matched by the first capturing group. The / before it is a literal character. It is simply the forward slash in the closing HTML tag that we are trying to match.
### Look-ahead and Look-behind
Lookaheads and lookbehinds are another powerful tool available in regex. They allow you to check for a certain pattern before or after the main expression without actually including it in the match.
Lookahead and lookbehind, collectively called “lookaround”, are zero-length assertions just like the start and end of line, and start and end of word anchors explained earlier in this tutorial. The difference is that lookaround actually matches characters, but then gives up the match, returning only the result: match or no match. That is why they are called “assertions”. They do not consume characters in the string, but only assert whether a match is possible or not. Lookaround allows you to create regular expressions that are impossible to create without them, or that would get very longwinded without them.
## Author

Arun Prasad - https://www.linkedin.com/in/arun-prasad-9071274/

https://github.com/arunp44 - My github profile
JavaScript Regex Tutorial: Matching a Hex Value

Regular expressions (regex) are invaluable tools for pattern matching and text manipulation in JavaScript. They allow developers to define specific search patterns within strings, making tasks like validation and data extraction much more manageable. In this tutorial, we will explore a particular regex used for matching hexadecimal color values and dissect each part of the expression to understand its functionality.

Summary

In this tutorial, we will focus on understanding the regex /^#?([a-f0-9]{6}|[a-f0-9]{3})$/, which is commonly used to validate hexadecimal color codes in HTML, CSS, and JavaScript. This regex ensures that the input string represents either a 3-digit or 6-digit hexadecimal color value, optionally preceded by a # symbol.

Table of Contents
Anchors
Quantifiers
Grouping Constructs
Bracket Expressions
Character Classes
Regex Components
Anchors

Anchors are regex elements used to asert positions within the text. In our regex, ^ and $ are anchors.

^ asserts the start of the line/string.
$ asserts the end of the line/string.
javascript

const pattern = /^#?([a-f0-9]{6}|[a-f0-9]{3})$/;


Quantifiers

Quantifiers specify the number of occurrences of a character or group in the regex. In our regex, {6} and {3} are quantifiers.

{6} specifies exactly 6 occurrences.
{3} specifies exactly 3 occurrences.

javascript

const pattern = /^#?([a-f0-9]{6}|[a-f0-9]{3})$/;
Grouping Constructs
Grouping constructs alloow parts of a regex to be treated as a single unit. In our regex, () are grouping constructs.

([a-f0-9]{6}|[a-f0-9]{3}) is a group that matches either a 6-digit or 3-digit hexadecimal value.
javascript

const pattern = /^#?([a-f0-9]{6}|[a-f0-9]{3})$/;
Bracket Expressions
Bracket expressions match any single character within the brackets. In our regex, [a-f0-9] is a bracket expression.

[a-f0-9] matches any lowercase letter from 'a' to 'f' or any digit from '0' to '9'.
javascript


const pattern = /^#?([a-f0-9]{6}|[a-f0-9]{3})$/;

Character Classes

Character classes match specific characters. In our regex, \# and \d are character classes.

/# matches the '#' character.
\d matches any digit from '0' to '9'.
javascript

const pattern = /^#?([a-f0-9]{6}|[a-f0-9]{3})$/;


Author
Written by Jacob Ferraro.







# Regex Tutorial: Matching a Hex Value

A regular expression, or regex, is a sequence of specific characters used to match specific patterns within text. Using a regex is a very efficient way of finding commonly needed information such as an HTML tag, URL, email address, or hex value.

## Summary

This regex tutorial will be going over the regex for matching a hex value. Hex values are most commonly used for hex color codes, with each combination of 6 characters connecting to a specific hue. The system that hex values use to create a unique code is known as the hexadecimal system, which utilizes 16 different possible characters: 0-9, and a-f. A couple examples of hex color codes look like this: "#872727", "68FF83", "#FF3322". If the hex color code uses repeating characters, such as the last example, you can instead write the code with just 3 characters: "#F32". The regex for matching a hex value looks like this: "/^#?([a-f0-9]{6}|[a-f0-9]{3})$/". This regex allows you to match any combination of hex value, whether it is 6 or 3 characters in length.

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

Anchors are used to specify the position of a pattern in the text. A couple of the most common anchors are the caret: "^", which matches the start of a line, and the dollar sign: "$", which matches the end.

### Quantifiers

Quantifiers determine how many times a character should be matched. One common quantifiers that this regex uses is the question mark: "?", which matches zero or on occurence of the preceding character.

### OR Operator

The OR operator: "|" is used to match one pattern or a different pattern. In this regex for hex values, it allows you to match either a 6-character value, or a 3-character value.

### Character Classes

Character classes are used to match any one character in a particular set. With the hex value regex, the character class [a-f0-9] matches any letter from "a" through "f", or any number from "0" through "9".

### Flags

Flags will modify the behavior of the regex. A common flag that you may think fits this regex is the case-insensitive flag: "i", which allows matching for both uppercase and lowercase characters. However, that flag is not needed for hex values.

### Grouping and Capturing

Grouping and capturing allow you to match patterns as a group, and then capture them to use later. The parentheses in the hex value regex group the possible hex value lengths together.

### Bracket Expressions

Bracket expressions can be used to specify a range of characters, which is displayed in this regex with the hyphen: "-". This allows matching of any character from "0" to "9", or "a" to "f".

### Greedy and Lazy Match

Greedy matching matches as much of a pattern as possible, and lazy matching matches as little as possible. The hex value regex utilizes greedy matching, in order to match the entire 3 or 6 character value.

### Boundaries

Boundaries are used to match a specific position in the text. Contrary to anchors, they match between characters, as opposed to the beginning or end of text. The hex value regex does not use boundaries.

### Back-references

Back-references allow you to match a previously matched group. It is helpful when matching patterns that have repeating elements. The hex value regex does not use back-references.

### Look-ahead and Look-behind

Look-ahead and look-behind can be used to match a pattern depending on what comes before or after it. The hex value regex does not utilize either of these.

## Author

This tutorial was written by Jackson Maltby, a UW coding bootcamp student. [GitHub](https://github.com/jacksonmaltby)

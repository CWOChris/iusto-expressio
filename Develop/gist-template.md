# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Tutorial for the regular expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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
/ = is the start and end of the regex
^ = the beginning of a string

### Anchors
<!-- $ = is an anchor that matches the end of the string. --> Commented out for reading clarity.

### Quantifiers
#? = matches a single character zero or one time(s). ? is a quantifier that means zero or one of the preceding character/elements allowing for the # at the start of a color code as needed.
{ and } = are used to specify a number of times a character/element must appear.  You can also use ranges and negation to create more complex sets. (In my chosen regex, the quantity of hex digits is specified by the {6} and {3} quantifiers.)

### OR Operator
| = is the OR operator.  It allows a match before or after it.  It is used in my chosen regex to match either a hex digit or a # and either 6 or 3 hex digits.

### Character Classes
[ and ] = are used to match a single character from a set of characters (classes).  You can use ranges and negation to create more complex sets. The caret ^ is used (placed first in the chosen regex) to negate a character class, in the example, it would match any character that is not a hexadecimal digit.

### Flags
No flags are present in my example but are defined here:

g = global search, doesn't return after the first match is identified.
i = case insensitive search meaning upper or lowercase characters are treated the same according to the regex.
m = multi-line search meaning ^ and $ match the beginning and end of each line, instead of the beginning and end of the entire string.
u = unicode search meaning the regex will match unicode characters or treat the pattern as unicode code points.
y = is used to execute multiple searches in a single pass.  This is useful when you need to find multiple matches in a string from the lastindex indicated by the placement of the flag. The next search string will begin at the lastindex + 1 when this flag is used.  This is called a sticky.

### Grouping and Capturing
( and ) = are used to group elements together in a 'capture group'. This is used to apply a quantifier to the group of characters. This is also useful for later referencing the captured text. In my chosen regex, the grouping idicates there will be either 6 or 3 hex digits that match.

### Bracket Expressions
[ and ] = are used to define a bracket expression, which matches any one character enclosed in the brackets. In the chosen regex, `[a-f0-9]` is a bracket expression that matches any single character that is a hexadecimal digit.

### Greedy and Lazy Match
Refers to quantifiers behavior when matching characters.  Greedy means it will match the longest possible string.  Lazy means it will match the shortest possible string.  In my chosen regex, there are no greedy or lazy quantifiers.

### Boundaries
^ = is the beginning of a string boundary. It means that the following pattern will start at the beginning of the string.
<!-- $ = is the end of a string boundary. All characters preceding it must be at the end of the string. --> Commented out for reading clarity.
### Back-references
\ = are used to refer to a previous capture group in the same pattern. The backslash, followed by a digit representing the number of the group to be referenced. There are no back-references in my chosen regex.

### Look-ahead and Look-behind
Look-ahead = is denoted by (?=...) for a positive look ahead, or that the pattern must be present. (?<!...>) for a negative look ahead where the pattern must not be there.
Look-behind = is denoted by (?<=...) for a positive look behind, or that the pattern must be present. (?<!...>) for a negative look behind where the pattern must not be there.

## Author

A short section about the author with a link to the author's GitHub profile https://github.com/CWOChris

I am a Full Stack Web Developer BootCamp student with EdX at the University of Minnesota.  I am an independent, self starter, motivated leader, who is passionate about learning new skills and applying them in the web development realm. I am a team player who is able to work well in either, team leadership, or, as an integral team member.  I have a wealth of knowledge and experience across many sectors including the military (combat and non-combat roles), aviation, logistics, medicine, mentorship, retail, purchasing, contract negotiations, legal and business areas.
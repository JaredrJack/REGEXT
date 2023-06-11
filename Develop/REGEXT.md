# REGEX

- This regular expression (regex) pattern is designed to match and validate email addresses. Email addresses are used for communication and data exchange.It's important to ensure that the email provided by a user is in the correct format. This regex pattern can be used to validate email addresses in various applications, such as form validation, user registration, or data filtering.



## Summary

- This regular expression (regex)  checks for the correct structure of an email address, including the presence of a username, the "@" symbol, a domain name, and a top-level domain. The regex pattern incorporates various rules and restrictions to ensure that the email address follows the commonly accepted format. By using this regex pattern, you can verify if a given string is a valid email address and handle it accordingly in your application.

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)



## Regex Components

### Anchors
- The ^ anchor indicates the beginning of a string, and the $ anchor indicates the end of a string. Both of these are found in our snippet above showing where the string starts and stops.

### Quantifiers
- Quantifiers set the limits of the string that the regex matches, they frequently include a minimum and maximum number of characters the regex is looking for.

- (+) Matches the character before the + one or more times, connects the user email name + email service + .com. {2,6} is saying that the requirement of the regex is between 2-6 charcaters long. for the set [a-z.].

### Character Classes
- A character class matches any one of the enclosed characters enclosed in the square brackets.

- The \d Matches any digit (Arabic numeral), from 0-9

### Grouping and Capturing
- The primary way to group a section of a regex is by using parentheses. In our snippet there are three groupings. The first grouping ([a-z0-9_\.-]+) will capture the email name, everything prior to the @ sign found in email addresses. The second grouping ([\da-z\.-]+) will capture the email domain name like gmail or yahoo. The third grouping ([a-z\.]{2,6}) will capture the last part of an email address, for example ".com" or ".net".

### Bracket Expressions
- Brackets indicate a set of characters to match, and any individual character between the brackets will match. Hypens are also used to define a set.

The [a-z0-9_.-] matches any letters form a-z and is case sensitive to lower case. It matches any number values between 0 and 9. It matches also matches the characters "_", ".", and "-" The [\da-z.-] matches a single digit from 0-9. Any letter from a-z and is case sensitive to lower case. It also matches the characters "." and "-". The [a-z.] matches any letters form a-z and is case sensitive to lower case. It also matches the characters ".".
### Greedy and Lazy Match
- This regrex include greedy matches. A greedy match means that By default, a quantifier tells the engine to match as much text as possible

The + will match as many times as possible and giving back as needed. The {} is used when matching the character or subexpression at least 2 times but no more than 6 times (as close to 6 as possible).
## Author

https://github.com/JaredrJack

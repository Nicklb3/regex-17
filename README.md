<h1 align="center"> REGEX 17</h1>

## Tutorial: Regex Matching a URL

Regular expressions, commonly referred to as "regex" is a special string used to describe search patterns. it allow us to match, search, and manipulate text more efficiently and effectively than traditional string methods. In this tutorial, you will learn the basics of regex syntax and how to use it in various programming languages and tools, including Python, JavaScript, and Perl. Whether you are a beginner or have some experience with regex, this tutorial will provide a comprehensive introduction to this powerful tool.

---

## Summary

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
As a regular expression, I check for a valid URL format. I look for the optional presence of "http://" or "https://" at the start of the string, followed by characters representing the domain name. The domain extension must be two to six letters, followed by an optional series of characters representing the path and file name. The string must end with a forward slash or have nothing after the domain extension.

---

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Boundaries](#boundaries)

---

## Regex Components

### Anchors

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
The anchors in this regular expression code are "^" and "$". The "^" anchor specifies the start of the string and the "$" anchor specifies the end of the string. These anchors ensure that the entire string matches the pattern specified in the regular expression and nothing more. In this case, the pattern specifies the format of a URL, and the "^" and "$" anchors ensure that the entire string is a valid URL and nothing else is included. This helps to validate that the input is a complete and well-formed URL, rather than just a partial match.

---

### Quantifiers

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
Quantifiers in this regular expression code are used to specify the number of times a particular character or group of characters should appear in the string. In this code, the quantifier "?" is used after the "s" in "https" to indicate that the "s" is optional and may or may not appear in the string. The quantifier "{2,6}" is used after the dot in the domain extension to specify that the extension must be between two and six letters long. The quantifier "*" is used after the group of characters representing the path and file name to indicate that this group may appear zero or more times in the string. These quantifiers help to define the pattern of a valid URL, ensuring that the string contains the appropriate number of characters in each part of the URL.

---

### OR Operator

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
The OR operator in this regular expression code is represented by the "?" symbol. It is used to specify that one of two options should match the string. In this code, the OR operator is used to indicate that the string may or may not start with "http://" or "https://". The "?" symbol following the "s" in "https" makes the "s" optional, allowing either "http://" or "https://" to match the string. This way, the code can validate both types of URL formats and ensure that the string is a valid URL, regardless of whether it starts with "http://" or "https://". The OR operator is a useful tool in regular expressions, allowing the matching of multiple alternative patterns in a single expression.

---

### Character Classes

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
Character classes in this regular expression code are represented by square brackets, "[ ]". They define a set of characters that should match a single character in the string. In this code, the character class "[\da-z.-]" is used to match domain name characters, which can be letters, numbers, dots, or hyphens. The character class "[a-z.]" is used to match the domain extension, which must be between two and six letters. The character class "[/\w .-]" is used to match characters representing the path and file name, including forward slashes, letters, numbers, spaces, dots, and hyphens. These character classes help to validate the structure of the URL and ensure that each part of the URL is made up of the correct type of characters. Character classes are a powerful tool in regular expressions, allowing the matching of multiple alternative characters in a single expression.

---

### Flags

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
Flags are not used in this regular expression code. Regular expression flags are optional symbols that modify the behavior of the regular expression. Some common flags include "i" for case-insensitive matching, "g" for global matching, and "m" for multiline matching. However, in this code, no flags are used, meaning that the regular expression will match the string in its default behavior, which is case-sensitive and only matches the first occurrence of the pattern. The absence of flags in this code does not affect the overall functionality of the regular expression and the code will still match URLs in the specified format.

---

### Grouping and Capturing

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
Grouping and capturing are important features in this regular expression code, as they allow individual parts of the URL to be extracted and used. Grouping is represented by parentheses "()" and is used to group together characters to form a single element. In this code, the first grouping "https?://" is used to capture either "http://" or "https://". The second grouping "([\da-z.-]+)" is used to capture the domain name, which can be made up of letters, numbers, dots, or hyphens. The third grouping "([a-z.]{2,6})" is used to capture the domain extension, which must be between two and six letters. The fourth grouping "([/\w .-]*)" is used to capture the path and file name, which can include forward slashes, letters, numbers, spaces, dots, and hyphens. Capturing allows the regular expression to extract specific parts of the URL and use them for further processing. Grouping and capturing are essential tools in regular expressions and are used in many applications to extract information from strings.

---

### Bracket Expressions

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
Bracket expressions are a powerful feature in regular expressions and are used in this code to match sets of characters. Bracket expressions are represented by square brackets "[]" and can include individual characters, ranges of characters, or special character classes. In this code, bracket expressions are used in several places, such as "[\da-z.-]+" to match the domain name, which can contain letters, numbers, dots, and hyphens. Another example is "[a-z.]{2,6}" to match the domain extension, which must be between two and six letters. Bracket expressions provide a concise and flexible way to match sets of characters, making them an important tool in regular expressions. They allow the regular expression to match strings based on complex patterns, making them suitable for a wide range of applications, such as validating URLs, email addresses, and more.

---

### Boundaries

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
 the regular expression has boundaries. The ^ symbol at the beginning of the expression represents the start of the string boundary, meaning that the expression must match from the start of the string. The $ symbol at the end of the expression represents the end of the string boundary, meaning that the expression must match until the end of the string.

These boundaries ensure that the entire string matches the pattern defined by the regular expression, and not just a part of it. For example, the expression /^(https?:\/\/)/ would match the first part of a URL, but the boundaries ^ and $ in the full expression /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ ensure that the entire URL must match the pattern.

---

## Author

I'm Nick L. Bonner and I love full stack development.
https://github.com/Nicklb3


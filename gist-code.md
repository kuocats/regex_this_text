# An Introduction to Regex (tutorial)

What is a Regex? A regex is a sequence of both basic and special characters that define a specific search pattern. 
A regex consists of a sequence of characters, metacharacters (such as ., \d, \D, \s, \S, \w, \W) and operators (such as +, *, ?, |, ^).

## Summary
 
When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace 
a character or sequence of characters within a string.

### :bangbang: Example: 

       /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
        
             Matching a Hex Value



What does that even mean? How is this translated into code? 
Let's took a look and break down each character....

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components
:wavy_dash: 

### Anchors
Anchor: `^` 
- `/^#` is our main anchor tag; known for the start of the expression

The characters do not define anything, but only to assert the beginning of the string. 

Anchor: `$`
- It is another form of anchor tag; known for the end of the expression

This character is typically used to check if the string matches a pattern. 

:wavy_dash: 

### Quantifiers

Quantifier indicates how many time the preceding pattern matches. 

Quantifier:  `?` 

This indicates a boolean value; either 0 or 1, meaning any character/symbol before `?` is optional. 
-  `/^#?` specifies how many instances of a character, group, or class must be present in the input for it to match. 
 > In our example, `#` would be optional in the regex. 

Quantifier: `{}`

- `[a-f0-9]{6}`
- `[a-f0-9]{3}`

This indicates that amount of occurrences a particular pattern needs to match. 
> In our example, `{6}` means that there are 6 instances of the string in the regex. It only allows 6 characters in the string betwen a-f and/or an interger between 0-9. 

> In our example, `{3}` means that there are 3 instances of the string in the regex. It only allows 3 characters in the string between a-f and/or an interger between 0-9.

:wavy_dash:

### OR Operator

OR Operator: ` | `

This indicates a boolean that matches either before or after the regex.

- `[a-f0-9]{6}|[a-f0-9]{3}` 

> `{6}` implies that there are 6 characters in the regex that contain a-f and/or an interger between 0-9 

>`{3}` implies that there are 3 characters in the regex that contain a-f and/or an interger between 0-9

Overall, the regex string must have 3 or 6 character with the specificed pattern. Anything less or more will be invalid.

:wavy_dash:

### Character Classes

- `[a-f0-9]` 

This is an example of Character Classes. 

It defines specific one set of select characters. A hyphen (-) in between character classes indicates the range it can be. 

> In our example, `[a-f0-9]` means that the range can only be selected from lower classe a-f and/or an interger from 0-9. 


:wavy_dash:


### Grouping and Capturing

Grouping & Caputuring: `()`

- `([a-f0-9]{6}|[a-f0-9]{3})`

Grouping allows multiple characters to be treated as a single compontent. 
In our example, this portion of the regex is also known as a  Bracket Expression.

:wavy_dash:


###  Bracket Expressions

Bracket Expression: `[]`

This symbolizes that it matches a specific set/pattern of characters. Typically, the hyphen in between indicates what range of characters the string can use.

-  `[a-f0-9]`

> In our example, this means that the string uses lower case characters between a-f or any interger from 0-9. 


:wavy_dash:



### Greedy and Lazy Match

Indicated by Quantifier: `{}`

Greedy - The longest string possible in order to match
Lazy - The shortest string possible in order to match 

> `[a-f0-9]{6}`
> `[a-f0-9]{3}`


:wavy_dash:


### Hope this was helpful! :+1: 





## Author


I'm Viv. This was written by a really basic level coder. 

:thought_balloon: My main goal for the bootcamp this was written for was to learn what Coding was about......and it is safe to say 
that it is one of the hardest things I have ever experienced/learned. 
The chances I make a career out of Coding is very slim. But, hey, it was an interesting ride :joy_cat: 

Bye!

Github: https://github.com/kuocats

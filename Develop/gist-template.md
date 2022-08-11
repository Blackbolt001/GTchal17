# Title (It's a bird, It's a plane, It's Regular Expressions!!)

Introductory paragraph 

    (they have been called puzzles, games, digit selectors, and all in all crazy strings, but most shudder at the phrase Regular Expressions.)

    Regular Expression is a sequense of characters that define a search pattern. The jumple of these comes from an origin of mathematical steps in order to find and search for data. as seen below the benifit of a very small and accurate shorthand comes at the cost of confusion and technical know how to code.


## Summary

Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

the 3 main expressions you will see are Anchors, Character sets, and modifiers
think of these as the overall syntax for reading regular expressions and we all konw from reading documentaitions that most things 
mean something eslse.

### Anchors
^ 
Start of a String or a Line - this specifies the pattern to match or seach must begin at this location

### Quantifiers
+
Quantifiers specify how many times an element can or must be found to be considered a match.

### Character Classes

[a-z0-9_\.-] [\da-z\.-] [a-z\.]
$ - Match the end of the input string. 

### Grouping and Capturing

([a-z0-9_\.-]+)  - grouping is where we capture text matched by the regex - think of it as a formula for our search 
since we are looking for an email we are looking for 
- somthing or  

/^([a-z0-9_\.-]+)

@ somthingElse ( one word)

@([\da-z\.-]+)\

.com or .org or . net or . something 
([a-z\.]{2,6})

### Bracket Expressions

basic regular expressions - ¬ $ . * \( \) [ \{ \} \
here we use the $ symbol to state that this is the endpoint for the regex imput line 
consequently the \ character turns of the special meaning of any characters directly behind it

### Greedy and Lazy Match

([a-z0-9_\.-]+)@
here the + quantifier also acts as a greedy match quantifer
here we are telling the regex that this match could be 
Mach123
Mach123match
Mach123matchmore
ItcouldAlsobeThis123
Or123this@

so even if Mach123 fits our search criteria it will be greedy and keep looking for more 


### Back-references

([a-z\.]{2,6}) - here we see the group capturing in the () but this unique add on is called the back reference
more specifically the {2,6} - here we are capturing the text and number that allows us to backreference or call back apply 
operators to the enire group.




## Author
 Joseph Gossett
A short section about the author with a link to the author's GitHub profile (Joseph Gossett is a cool person, I have known him my entire life)

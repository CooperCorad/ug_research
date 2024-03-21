PYTHON -- [text](https://docs.python.org/3/library/re.html)

 re.VERBOSE

This flag allows you to write regular expressions that look nicer and are more readable by __allowing you to visually separate logical sections of the pattern and add comments.__ Whitespace within the pattern is ignored, except when in a character class, or when preceded by an unescaped backslash, or within tokens like *?, \(?: or \(?P<...>. For example, \(? : and * ? are not allowed

RUST -- [text](https://docs.rs/regex/latest/regex/#syntax)

 Character Classes

[\a-y&&xyz]    Intersection (matching x or y)

[0-9&&[\^4]]   Subtraction using intersection and negation (matching 0-9 except 4)

[\0-9--4]      Direct subtraction (matching 0-9 except 4)

[\a-g~~b-h]    Symmetric difference (matching `a` and `h` only)

\b{start}, \<   start-of-word boundary assertion

\b{end}, \\>     end-of-word boundary assertion

https://blog.logrocket.com/getting-started-regexbuilder-swift/#regexbuilder-api

https://pomsky-lang.org/

https://perldoc.perl.org/perlre

https://www.rand.org/content/dam/rand/pubs/research_memoranda/2008/RM704.pdf [pp43-...]
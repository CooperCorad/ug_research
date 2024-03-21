# An Outline of a new Regular Expression Sublanguage for Rhombus

__Major Changes__
1. no escapes! operators are used outside of strings as literals
2. <ins>The Thrifty Operator:</ins> using ``?`` after a \<repeater> seems silly and confusing, both syntactically and at a macro level thus a rewrite:

&nbsp;&nbsp;&nbsp; | \<repeater>``?`` -> \<repeater>``~`` or ``<`` (undecided but probably first?)

3. <ins>Back References:</ins> \<atom>``\n`` -> \<atom>``@n``

4. <ins>Word Boundaries:</ins> ``\b`` -> ``b`` && ``\B`` -> ``B``

5. <ins>Property Notation:</ins> ``\p{``\<property>``}`` -> ``p{``\<property>``}`` && ``\P{``\<property>``}`` -> ``P{``\<property>``}``

6. <ins>POSIX Classes:</ins> ``[[:alpha:][:upper:]]`` -> ``[[:alpha, upper:]]`` Matching on strings??

7. <ins>Modes && Only First</ins> ``(?>(?``\<mode>``:`` \<regexp>``))`` -> ``(?>``\<mode>``:``\<regexp>``)`` | macro just converts it back but it's simpler and I don't think it causes any problems(??)

8. named and numbered capture groups, invocation of a bound capture group vs using it as a backref
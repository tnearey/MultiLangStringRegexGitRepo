#MultiLngStringRegexes#

## Refering to common punctuation symbols encountered in code translation
Ratforish refers to labels for ASCII constants in 
Kernighan, B. W., & Plauger, P. J. (1976). Software tools. ACM SIGSOFT Software Engineering Notes, 1(1), 15–20.

BACKSLASH = 92 = <\> | SQUOTE = 39 = <'>    (== Unicode Apostrophe) |  DQUOTE = 34 = <"> (==UNICODE Quotation Mark) | 
In addition note BACKTICK = 96 = <`> (== Unicode Grave Accent)
## Quoting quotes
Language      | Quote Char       | Ratforish | Escaped| Ratforish |Example
--------------|:----------------:|:---------:|--------|-----------|-------------|
Matlab        | '  <SQUOTE>      | ''       :| SQUOTE |SQUOTE SQUOTE | str='Joe''s'    |
R             | '  <SQUOTE>       | \' |  BACKSLASH SQUOTE  | str = 'Joe\'s' |
R   (alt)     |" <DQUOTE>   | \' | BACKSLASH DQUOTE*  | str = "He says \"Hi\""
JavaScript| ' | <SQUOTE>     | \' | BACKSLASH SQUOTE  | str = 'Joe\'s' |
JavaScrip (alt) |" <DQUOTE> | \' | BACKSLASH DQUOTE  | str = "He says \"Hi\""
_____________


Note Languages R JavaScript also allow DQUOTE/SQUOTE switching "Joe's" or 'He says "Hi"'
* R escape behavior is a little goofy with escaped double quote in double quoted string
 
````
# Single quotes work as expected
> s='Joe\'s'
> s
[1] "Joe's"
# Double quotes escape the second " but keep the \
> s2="Joe\"s"
> s2
[1] "Joe\"s"
````


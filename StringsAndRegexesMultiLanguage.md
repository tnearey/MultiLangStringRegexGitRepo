<<<<<<< Updated upstream
#MultiLngStringRegexes#
I just changed this to see if I can get it to show up on Github.com

## Refering to common punctuation symbols encountered in code translation
Ratforish refers to labels for ASCII constants in
Kernighan, B. W., & Plauger, P. J. (1976). Software tools. ACM SIGSOFT Software Engineering Notes, 1(1), 15–20.

BACKSLASH = 92 = <\> | SQUOTE = 39 = <'>    (== Unicode Apostrophe) |  DQUOTE = 34 = <"> (==UNICODE Quotation Mark) |
In addition note BACKTICK = 96 = <`> (== Unicode Grave Accent)
## Quoting quotes
Language        | Quote Char  | Ratforish | Escaped| Ratforish       | Example
----------------|:-----------:|:---------:|--------|-----------------|-----------------|
Matlab          | '           |  SQUOTE   |''      | SQUOTE SQUOTE | str='Joe''s'      |
R               | '           |  SQUOTE   | \'     | BACKSLASH SQUOTE| str = 'Joe\'s'  |
R   (alt)       |"            |  DQUOTE   | \'     | BACKSLASH DQUOTE*| str = "He says \"Hi\""|
JavaScript      | '           |    SQUOTE     | \' | BACKSLASH SQUOTE  | str = 'Joe\'s' |
JavaScript (alt) | " | DQUOTE | \' | BACKSLASH DQUOTE  | str = "He says \"Hi\""



Note: Languages R JavaScript also allow DQUOTE/SQUOTE switching "Joe's" or 'He says "Hi"'

*Note: R escape behavior is a little goofy with escaped double quote in double quoted string. It captures the DQUOTE correctly but also shows the BACKSLASH.

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

=======
This will be a markdown

See this page for special characters
    	    https://stat.ethz.ch/R-manual/R-devel/library/base/html/Quotes.html
>

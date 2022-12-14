# Markdown Cheatsheet
created 2022-12-1 15:27

# Headings

```
# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------
```

# H1
## H2
### H3
#### H4
##### H5
###### H6

Alternatively, for H1 and H2, an underline-ish style:

Alt-H1
======

Alt-H2
------

# Emphasis

```
Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~
```

Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

# Links

```
[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com
```

[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links. 
http://www.example.com or <http://www.example.com> and sometimes 
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

# Lists

```
1. First ordered list item
2. Another item
??????* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
??????1. Ordered sub-list
4. And another item.

?????????You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

?????????To have a line break without a paragraph, you will need to use two trailing spaces.??????
?????????Note that this line is separate, but within the same paragraph.??????
?????????(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses
```

1. First ordered list item
2. Another item
??????* Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
??????1. Ordered sub-list
4. And another item.

?????????You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

?????????To have a line break without a paragraph, you will need to use two trailing spaces.??????
?????????Note that this line is separate, but within the same paragraph.??????
?????????(This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

* Unordered list can use asterisks
- Or minuses
+ Or pluses

# Images

You can use the same syntax as links, but add an exclamation mark in front of the brackets. Also you can use HTML img tag , which allows you to set the image size.

```
![Image](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="git logo" width="300">
```
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="git logo" width="300">

# Code and Syntax Highlighting

Use three backticks for a fenced code block:

```
function test() {
 console.log("look ma???, no spaces");
}
```

Adding language identifier to enable syntax highlighting:

```javascript
function test() {
 console.log("look ma???, no spaces");
}
```

# Tables

```
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

# Blockquotes

```
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.
```

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.



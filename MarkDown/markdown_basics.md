# Markdown Basics CheatSheet
The cheatsheet is broken down into sections of code, followed by their output.

## Headers

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
# H1
## H2
### H3
#### H4
##### H5
###### H6


## Text Emphasis
```markdown
*Italic* or _Italic_
**Bold** or __Bold__
***Bold and Italic*** or ___Bold and Italic___
```

## Lists Unordered
```markdown
- Item 1
- Item 2
  - Subitem 1
  - Subitem 2
* Item 1
* Item 2
  * Subitem 1
  * Subitem 2
```
- Item 1
- Item 2
  - Subitem 1
  - Subitem 2
* Item 1
* Item 2
  * Subitem 1
  * Subitem 2

## Lists Ordered
```markdown
1. Item 1
2. Item 2
   1. Subitem 1
   2. Subitem 2
```
1. Item 1
2. Item 2
   1. Subitem 1
   2. Subitem 2

## Hyperlink
```markdown
[Cheatsheet Repo](https://github.com/RaphCodec/MD_Cheatsheets "Optional Title")
```
[Cheatsheet Repo](https://github.com/RaphCodec/MD_Cheatsheets "Optional Title")

## Images
```markdown
![Photo](pexels-tdcat-59523.jpg "Photo by Torsten Dettlaff: https://www.pexels.com/photo/brown-and-black-german-shepherd-puppy-sitting-on-gray-textile-59523/")
```
![Photo](pexels-tdcat-59523.jpg "Photo by Torsten Dettlaff: https://www.pexels.com/photo/brown-and-black-german-shepherd-puppy-sitting-on-gray-textile-59523/")

### Images with caption and HTML
```html
<p align="center">
  <img src=pexels-tdcat-59523.jpg alt="Alt text" title="Optional Title"/>
  <br>
  <em>Figure 1: This is the caption for the image.</em>
</p>
```
<p align="center">
  <img src=pexels-tdcat-59523.jpg alt="Alt text" title="Optional Title"/>
  <br>
  <em>Figure 1: Puppy Photo by Torsten Dettlaff.</em>
</p>

## Quotes
```markdown
> Blockquote
>> Nested Blockquote
```
> Blockquote
>> Nested Blockquote

## Inline Code
`pip install pandas`
```markdown
`inline code`
```

## Block Code
```python
import pandas
```
\```python
import pandas
\```

## Horizontal Rule
```markdown
---
***
___
```

---
***
___

## Escape Characters
```markdown
\*literal asterisks\*
```

\*literal asterisks\*

## Tables
```markdown
| Header 1 | Header 2 |
|----------|----------|
| Cell 1   | Cell 2   |
| Cell 3   | Cell 4   |
```
| Header 1 | Header 2 |
|----------|----------|
| Cell 1   | Cell 2   |
| Cell 3   | Cell 4   |

## Strikethrough
```markdown
~~strikethrough~~
```
~~strikethrough~~

## Task Lists
```markdown
- [x] Task 1
- [ ] Task 2
```
- [x] Task 1
- [ ] Task 2

## Definition Lists
```markdown
Term 1
: Definition 1

Term 2
: Definition 2
```
Term 1
: Definition 1

Term 2
: Definition 2

## Footnotes
```markdown
Here's a sentence with a footnote.[^1]

[^1]: Footnote text.
```
Here's a sentence with a footnote.[^1]

[^1]: Footnote text.

## Syntax Highlighting
```makrdown
```python
def function():
    return "Hello, World!"
```
```python
def function():
    return "Hello, World!"
```

## Admonitions
```markdown
!!! note
    This is a note.
!!! warning
    This is a warning.
```
!!! note
    This is a note.
!!! warning
    This is a warning.

## Math using LaTex
```markdown
$$
E = mc^2
$$
```
$$
E = mc^2
$$


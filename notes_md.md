
# Markdown Cheatsheet

This is a reference to the markdown syntax based on [Markdown Crash Course](https://www.youtube.com/watch?v=HUBNt18RFbo "Mardown Youtube tutorial").


## Definition

Markdown is a lightweight markup language with plain text formatting syntax designed so that it can be converted to HTML ([source](https://duckduckgo.com/?q=markdown+cheatsheet&t=chromentp&ia=answer&iax=1)).


## Use cases

Markdown can be used for several purposes. For example:

* Readme files

* Blog posts

* Static websites (Static Site Generators)

## Editor Preview

There are different editor extensions that allow you to preview the formated text. The __*Auto Open Markdown Previewer*__ extension is available in VSCode. Similar extensions are also available for other editors.

## Formating


### Emphasis

* *Italics*: `*Italics*` or `_Italics_` 
* **Bold**: `**Bold**` or `__Bold__`
* ~~Strikethrough~~: `~~Strikethrough~~`
* Horizontal rules: `---` (three hyphens), `***` (three asteriks) or `___` (three underscores) 

### Heading 

Markdown syntax:
```Markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

HTML output:
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
    
### Horizontal Rule
 
A horizontal rule is produced with `---` (three hyphens) or `___` (three underscores) 

---

### Paragraphs

To create HTML paragraph tags (`<p></p>`), leave a white line between pieces of text.

##### Markdown syntax:
```Markdown
This is paragraph 1.

This is paragraph 2.
```
##### HTML output:
```HTML
<p>This is paragraph 1.</p>

<p>This is paragraph 2.</p>
```

### Line break

To create a line break or new line (`<br>`), end a line with two or more spaces, and then type return.

##### Markdown syntax:
```Markdown
This is a line with two trailing spaces.  The following line starts here.
```
##### HTML output:
```HTML
<p>This is a line with two trailing spaces. <br> The following line starts here.</p>
```
##### Rendered output:
```
This is a line with two trailing spaces.  
The following line starts here.
```

### Escaping

To escape special characters (`#`, `*`, `-`, etc.), precede them with a backslash (`\`).

##### Markdown syntax:
```Markdown
\# Heading 1
```
##### Rendered output:
```HTML
\# Heading 1
```

### Blockquote

To create blockquotes in one or multiple lines, start each line with a *greater than* symbol (`>`).  

> This is a quote. (trailing spaces)  
> This is its second line.

### Links

To embed a link that redirects to some website, we use the following syntax:

##### Markdown syntax:
```Markdown
[Google](https://www.google.com "Some hover message") 
```
Within the squared brackets write the text to be displayed. The parenthesis includes the embeded link and optionally a hover message in quotes or double quotes.

##### Rendered output:  
[Google (embedded link dummy; try it out!)](https://www.google.com 'Some hover message') 

### Images

Use the same syntax as with links, preceded by an exclamation mark (`!`), to import an image.

##### Markdown syntax:
```Markdown
![Markdown Logo](https://markdown-here.com/img/icon256.png)
```
##### Rendered output:
![Markdown Logo](https://markdown-here.com/img/icon256.png)

### Unordered Lists

 To create an unordered list, start the line with the asterisk symbol (`*`). Precede it with a *tab* to create a nested lists. 

##### Markdown syntax:
```Markdown
* Item 1
* Item 2
* Item 3
  * Nested Item 1
  * Nested Item 2
```
##### Rendered output:
* Item 1
* Item 2
* Item 3
  * Nested Item 1
  * Nested Item 2

### Ordered lists

To create an ordered list, start the line with the number one followed by a period (`1.`). The value of the following list numbers is not relevant.  

Use the same syntax to create nested lists by preceding it with a *tab*.

##### Markdown syntax:
```Markdown
1. Item 1
3. Item 2
2. Item 3
    1. Sub-item 1
    1. Sub-item 2
```
##### Rendered output:
1. Item 1
3. Item 2
2. Item 3
    1. Sub-item 1
    1. Sub-item 2

### Inline Code Block

Embed code in text using backticks (` `` `).

##### Markdown syntax:

```Markdown
Here is an HTML tag `<p>`
```
##### Rendered output:

Here is an HTML tag `<p>`

## Github Markdown syntax

Some Markdown syntax is specific to Github. 

### Code Blocks

Use three backticks (` ``` `) to open and close a code block. Specify the language in question after the opening backticks.

##### Markdown syntax: 

>` ``` `javascript  
>  function add(num1, num2) {  
>    return num1 + num2;  
>  }
` ``` `
##### Rendering output:

```javascript  
function add(num1, num2) {  
  return num1 + num2;  
}
```

### Tables

To create a table, use vertical pipes (`|`) and hyphens (`---`) for cell divisions.

##### Markdown syntax: 

``` Markdown
| Name     | Email          |
| ---      | ---            |
| John Doe | john@gmail.com |
| Jane Doe | jane@gmail.com |
``` 
##### Rendering output:

| Name     | Email          |
| ---      | ---            |
| John Doe | john@gmail.com |
| Jane Doe | jane@gmail.com |

### Task lists

To create checked or unchecked boxes, use :

##### Markdown syntax: 

``` Markdown
* [x] Task 1
* [x] Task 2
* [ ] Task 3
```

##### Rendering output:

* [x] Task 1
* [x] Task 2
* [ ] Task 3
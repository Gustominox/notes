# Markdown Cheat Sheet

From [The Markdown Guide](https://www.markdownguide.org)!

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. 
It doesn't cover every edge case.

## Basic Syntax

These are the elements outlined in John Gruber’s original design document.
All Markdown applications support these elements.

### Heading

# H1
## H2
### H3

### Bold

**bold text**

### Italic

*italicized text*

### Blockquote

> blockquote

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- First item
- Second item
- Third item

### Code

`code code code code code `

### Horizontal Rule

---

### Link

[My_Git_Profile](https://github.com/Gustominox)

### Image

![My_Git_Avatar](https://avatars.githubusercontent.com/u/59740441?s=60&v=4)

## Extended Syntax

These elements extend the basic syntax by adding additional features. 
Not all Markdown applications support these elements.

### Table

| Syntax    | Description | Something |
| :---      |    :----:   |      ---: |
| Header    | Title       | thing |
| Graph     | Text 	  | thing |

### Fenced Code Block

```c
#include <stdio.h>

void main(){

printf("Hello World");
return 0;

}
```

### Footnote

Here's a simple footnote[^1]

[^1]: This is the footnote.

### Heading ID

### My Great Heading {#custom-id}

### Definition List

term
: definition

### Strikethrough

~~The world is flat.~~

### Task List

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

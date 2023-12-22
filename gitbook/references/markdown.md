---
description: Spacehall markdown formatting reference
---

# Markdown

### Headings

To create a heading, add one to six `#` symbols before your heading text. The number of `#` you use will determine the hierarchy level and typeface size of the heading.

```markdown
# A first-level heading
## A second-level heading
### A third-level heading
```

### Styling text

You can indicate emphasis with bold, italic, strikethrough, subscript, or superscript text.

| Style                  | Syntax             | Example                                  | Output                                         |
| ---------------------- | ------------------ | ---------------------------------------- | ---------------------------------------------- |
| Bold                   | `** **` or `__ __` | `**This is bold text**`                  | **This is bold text**                          |
| Italic                 | `* *` or `_ _`     | `_This text is italicized_`              | _This text is italicized_                      |
| Strikethrough          | `~~ ~~`            | `~~This was mistaken text~~`             | ~~This was mistaken text~~                     |
| Bold and nested italic | `** **` and `_ _`  | `**This text is _extremely_ important**` | **This text is **_**extremely**_** important** |
| All bold and italic    | `*** ***`          | `***All this text is important***`       | _**All this text is important**_               |

### Quoting text

You can quote text with a `>`.

```markdown
Text that is not a quote

> Text that is a quote
```

Quoted text is indented.

### Quoting code

You can call out code or a command within a sentence with single backticks. The text within the backticks will not be formatted.

```markdown
Use `cat file.txt` to output the content of the text file.
```

To format code into its own distinct block, use triple backticks.

````markdown
Print a text string:

```
print("Hello World!")
```
````

Spacehall will try to infer the programming language from the block's content.

You can also set it manually by adding the language name after the first backticks.

````markdown
Print a text string:

```rust
println!("Hello World!")
```
````

### Links

You can create an inline link by wrapping link text in brackets `[ ]`, and then wrapping the URL in parentheses `( )`.

```markdown
This discussion is hosted on [Spacehall](https://spacehall.app).
```

Valid URLs are automatically transformed as links.

### Images

You can display an image by adding ! and wrapping the alt text in \[ ].

Alt text is a short text equivalent of the information in the image.

Then, wrap the link for the image in parentheses ().

```markdown
![My screenshot](https://some-url.com/my-screenshot.jpg)
```

For more information on how to upload a picture to Spacehall, see Uploading assets.

### Lists

You can make an unordered list by preceding one or more lines of text with `-`, `*`, or `+`.

```markdown
- George Washington
- John Adams
- Thomas Jefferson
```

To order your list, precede each line with a number.

```markdown
1. James Madison
1. James Monroe
1. John Quincy Adams
```

#### Nested Lists

You can create a nested list by indenting one or more list items below another item.

```markdown
1. First list item
   - First nested list item
     - Second nested list item
```

### Task lists

You can create a task list by preceding one or more line with `- [ ]` for new tasks, and `- [x]` for completed tasks.

```markdown
- [x] buy bread
- [ ] buy cheese
- [ ] buy ham
```

### Uploading assets

You can upload assets like images by using the file uploader.

| Limitations           |                                    |
| --------------------- | ---------------------------------- |
| Supported assets      | images                             |
| Format                | jpeg, png, svg, gif, webp          |
| Maximum size          | 10 MB                              |
| Maximum dimension     | 12,000 px                          |
| Maximum resolution    | 100 megapixels (ex: 10,000x10,000) |
| Maximum metadata size | 1024 bytes                         |
| Animated GIFs         | Limited to 50 mp                   |

### Paragraphs

You can create a new paragraph by leaving a blank line between lines of text.

### Footnotes

You can add footnotes to your content by using this bracket syntax:

```markdown
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

[^1]: My reference.
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
```

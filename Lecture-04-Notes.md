# 📖 Lecture 04: Semantic HTML and Advanced HTML Elements

## Introduction

As websites become larger and more complex, organizing content properly becomes important.

Semantic HTML provides meaningful structure to webpages, making them easier to understand for developers, browsers, and search engines.

---

# Semantic HTML

Semantic tags clearly describe the purpose of the content they contain.

Benefits:

- Better code readability
- Better website structure
- Improved SEO (Search Engine Optimization)
- Easier maintenance

---

# Header Element

The `<header>` tag represents the introductory section of a webpage.

```html
<header>
    <h1>My Website</h1>
</header>
```

Common Uses:

- Website logo
- Navigation menu
- Website title

---

# Main Element

The `<main>` tag contains the primary content of the webpage.

```html
<main>
    <h2>Welcome to my website</h2>
</main>
```

A webpage should only have one main element.

---

# Footer Element

The `<footer>` tag contains closing information.

```html
<footer>
    <p>Copyright © 2026</p>
</footer>
```

Common Uses:

- Copyright information
- Contact details
- Social media links

---

# Strong Tag

The `<strong>` tag indicates important text.

```html
<strong>Important Notice</strong>
```

Output:

**Important Notice**

---

# Em Tag

The `<em>` tag emphasizes text.

```html
<em>Learning HTML is important.</em>
```

Output:

*Learning HTML is important.*

---

# Blockquote Tag

Used for long quotations.

```html
<blockquote>
    Success is the sum of small efforts repeated daily.
</blockquote>
```

Blockquotes appear on a separate line.

---

# Q Tag

Used for short quotations.

```html
<q>Consistency Creates Success</q>
```

Output:

"Consistency Creates Success"

---

# Dfn Tag

The `<dfn>` tag represents a term being defined.

```html
<dfn>HTML</dfn>
```

Example:

HTML stands for HyperText Markup Language.

---

# Abbreviation Tag

The `<abbr>` tag is used for abbreviations.

```html
<abbr title="HyperText Markup Language">HTML</abbr>
```

When the user hovers over HTML, the full form appears.

---

# Meta Tags

Meta tags provide information about a webpage.

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Purpose:

### charset

Defines character encoding.

```html
<meta charset="UTF-8">
```

### viewport

Makes webpages responsive on different devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

---

# Div Tag

The `<div>` tag is a container element.

```html
<div>
    <h2>About Me</h2>
    <p>Hello World</p>
</div>
```

Used for:

- Grouping elements
- Page layout
- Styling with CSS

---

# Span Tag

The `<span>` tag is an inline container.

```html
<p>Hello <span>World</span></p>
```

Used for styling specific text.

---

# Block Elements

Block elements start on a new line and occupy full width.

Examples:

```html
<h1></h1>
<p></p>
<div></div>
<ul></ul>
<ol></ol>
```

Characteristics:

- Starts on a new line
- Takes full available width

---

# Inline Elements

Inline elements do not start on a new line.

Examples:

```html
<span></span>
<a></a>
<strong></strong>
<em></em>
```

Characteristics:

- Appears within a line
- Takes only required width

---

# Anchor Tag

The `<a>` tag creates hyperlinks.

```html
<a href="https://github.com">GitHub</a>
```

Common Attributes:

### href

Specifies destination URL.

```html
<a href="https://google.com">Google</a>
```

### target

Opens link in a new tab.

```html
<a href="https://github.com" target="_blank">
GitHub
</a>
```

---

# Iframe Tag

The `<iframe>` tag embeds another webpage inside a webpage.

```html
<iframe src="https://www.wikipedia.org"></iframe>
```

Uses:

- Google Maps
- YouTube Videos
- External Websites

---

# Video Tag

HTML allows videos to be embedded directly.

```html
<video controls width="500">
    <source src="video.mp4" type="video/mp4">
</video>
```

Attributes:

### controls

Shows video controls.

### autoplay

Automatically starts video.

### loop

Repeats video continuously.

### muted

Mutes audio.

Example:

```html
<video controls autoplay muted loop>
    <source src="video.mp4">
</video>
```

---

# Audio Tag

The `<audio>` tag is used to play sound files.

```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
</audio>
```

Attributes:

### controls

Shows audio controls.

### autoplay

Automatically starts audio.

### loop

Repeats audio continuously.

### muted

Starts audio muted.

Example:

```html
<audio controls loop>
    <source src="audio.mp3">
</audio>
```

---

# HTML Entities

Used to display reserved characters.

Examples:

```html
&lt;
&gt;
&amp;
&nbsp;
```

Output:

< > &

---

# HTML Comments

Comments are ignored by browsers.

```html
<!-- This is a comment -->
```

Used for:

- Notes
- Documentation
- Code organization

---

# Complete HTML Journey Summary

Topics Covered During HTML Course:

### Lecture 01

- Introduction to HTML
- HTML Structure
- Head
- Body
- Title
- Headings
- Paragraphs
- Lists
- Attributes
- Comments

### Lecture 02

- Tables
- Table Rows
- Table Headings
- Table Data
- Forms Introduction

### Lecture 03

- Form Elements
- Input Types
- Radio Buttons
- Checkboxes
- Select
- Option
- Textarea
- File Upload
- URL Input
- Color Picker
- Range Input

### Lecture 04

- Semantic HTML
- Header
- Main
- Footer
- Strong
- Em
- Blockquote
- Q
- Dfn
- Abbr
- Meta Tags
- Div
- Span
- Block vs Inline Elements
- Anchor Tags
- Iframe
- Video
- Audio

---

# Conclusion

HTML (HyperText Markup Language) is the foundation of every website.

It provides structure and content for web pages. HTML works together with CSS for styling and JavaScript for interactivity.

After learning HTML, the next step is CSS, which is used to design and beautify web pages.

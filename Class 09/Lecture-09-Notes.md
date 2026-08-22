# 📖 Lecture 08: CSS Fonts, Units & Text Styling

## Introduction

Fonts and text styling play an important role in web design. CSS allows us to control the appearance of text by changing fonts, sizes, spacing, alignment, decorations, and shadows.

In this lecture, we learned:

- Font Family
- Font Weight
- Google Fonts
- CSS Units
- Relative Units
- Absolute Units
- Font Style
- Text Transform
- Text Decoration
- Line Height
- Letter Spacing
- Word Spacing
- Text Align
- Text Shadow

---

# Font Family

The `font-family` property is used to change the font of text.

```css
p {
    font-family: Arial, sans-serif;
}
```

Example:

```css
body {
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}
```

---

# Types of Fonts

There are two common ways to use custom fonts.

## 1. Import Fonts

Using `@import`.

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap');
```

Example:

```css
body {
    font-family: 'Poppins', sans-serif;
}
```

---

## 2. Link Fonts in HTML

```html
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
```

---

## 3. Download Fonts

You can download fonts from Google Fonts and use them locally.

```css
@font-face {
    font-family: "MyFont";
    src: url("fonts/MyFont.ttf");
}
```

---

# Font Weight

Controls the thickness of text.

```css
h1 {
    font-weight: bold;
}
```

Common Values:

```css
font-weight: 100;
font-weight: 300;
font-weight: 400;
font-weight: 500;
font-weight: 700;
font-weight: 900;
```

### Default

```css
font-weight: 400;
```

---

# Font Size

Changes the size of text.

```css
h1 {
    font-size: 40px;
}
```

---

# Default Browser Font Sizes

### Heading

```html
<h1>Hello</h1>
```

Default:

```css
32px
```

### Paragraph

```html
<p>Hello World</p>
```

Default:

```css
16px
```

---

# CSS Units

CSS uses different units to define size.

There are two major categories:

## Relative Units

Relative units depend on another element.

### rem

Relative to the root element (`html`).

```css
html {
    font-size: 16px;
}

h1 {
    font-size: 2rem;
}
```

Calculation:

```text
2 × 16px = 32px
```

---

### em

Relative to the parent element.

```css
.parent {
    font-size: 20px;
}

.child {
    font-size: 2em;
}
```

Calculation:

```text
2 × 20px = 40px
```

---

### Percentage (%)

Relative to parent size.

```css
div {
    width: 50%;
}
```

Example:

```text
Parent = 1000px
50% = 500px
```

---

# Root Element

The root element is:

```html
<html>
```

Example:

```css
html {
    font-size: 16px;
}
```

All `rem` values are calculated from the html element.

---

# Absolute Units

Absolute units do not depend on parent font size.

## px (Pixels)

Most common unit.

```css
h1 {
    font-size: 32px;
}
```

---

## vh (Viewport Height)

Relative to screen height.

```css
div {
    height: 100vh;
}
```

Meaning:

```text
100% of screen height
```

---

## vw (Viewport Width)

Relative to screen width.

```css
div {
    width: 100vw;
}
```

Meaning:

```text
100% of screen width
```

---

# Difference Between Relative and Absolute Units

## Relative Units

```css
rem
em
%
```

Depend on:

- Root element
- Parent element
- Container size

---

## Absolute Units

```css
px
vh
vw
```

Depend on:

- Screen size
- Viewport size

Not affected by parent font size.


---

# Understanding VW, VH and Overflow

## Viewport Width (vw)

`vw` stands for **Viewport Width**.

```css
width: 100vw;
```

Meaning:

```text
100% of browser width
```

Examples:

```css
width: 50vw;
```

Means:

```text
50% of screen width
```

---

## Viewport Height (vh)

`vh` stands for **Viewport Height**.

```css
height: 100vh;
```

Meaning:

```text
100% of browser height
```

Example:

```css
height: 50vh;
```

Means:

```text
50% of screen height
```

---

# Common Problem with VW

Example:

```css
.box {
    width: 80vw;
    border: 2px solid black;
    padding: 20px;
}

.box > div {
    width: 90vw;
    border: 1px solid black;
}
```

HTML:

```html
<div class="box">
    <div>
        Child Element
    </div>
</div>
```

---

## What Happens?

Parent Width:

```css
80vw
```

Child Width:

```css
90vw
```

The child becomes wider than its parent.

Example:

```text
Parent = 80% of screen

Child = 90% of screen
```

Result:

❌ Child overflows outside the parent

❌ Horizontal scrollbar may appear

---

## Better Approach

Use percentages when sizing children.

```css
.box {
    width: 80vw;
}

.box > div {
    width: 100%;
}
```

Now:

```text
Child = 100% of Parent
```

Result:

✅ Fits perfectly inside parent

✅ Responsive layout

---

# Difference Between % and VW

## Percentage (%)

Relative to parent.

```css
width: 50%;
```

Meaning:

```text
50% of parent width
```

---

## VW

Relative to browser window.

```css
width: 50vw;
```

Meaning:

```text
50% of screen width
```

---

# Best Practice

✅ Use `%` for child elements

✅ Use `vw` and `vh` for full-page layouts

✅ Avoid giving children larger viewport widths than their parents

✅ Check for horizontal scrolling when using `vw`

---

# Width Using Percentage

```css
.container {
    width: 80%;
}
```

Useful for responsive design.

---

# Border

Adds a border around elements.

```css
div {
    border: 2px solid black;
}
```

Syntax:

```css
border: width style color;
```

Example:

```css
border: 3px dashed red;
```

---

# Font Style

Used for italic text.

```css
p {
    font-style: italic;
}
```

Values:

```css
normal
italic
oblique
```

---

# Text Transform

Changes letter case.

```css
text-transform: uppercase;
```

Values:

```css
uppercase
lowercase
capitalize
none
```

Example:

```css
h1 {
    text-transform: uppercase;
}
```

---

# Text Decoration

Used to decorate text.

```css
text-decoration: underline;
```

Values:

```css
underline
overline
line-through
none
```

Example:

```css
a {
    text-decoration: none;
}
```

---

# Line Height

Controls spacing between lines.

```css
p {
    line-height: 30px;
}
```

Example:

```css
line-height: 1.5;
```

---

# Letter Spacing

Controls space between letters.

```css
h1 {
    letter-spacing: 5px;
}
```

---

# Word Spacing

Controls space between words.

```css
p {
    word-spacing: 10px;
}
```

---

# Text Align

Controls horizontal alignment.

```css
text-align: center;
```

Values:

```css
left
right
center
justify
```

Example:

```css
h1 {
    text-align: center;
}
```

---

# Text Shadow

Adds shadow behind text.

Syntax:

```css
text-shadow: horizontal vertical blur color;
```

Example:

```css
h1 {
    text-shadow: 2px 2px 5px gray;
}
```

---

# Text Shadow Generator

Useful Website:

https://cssgenerator.org/text-shadow-css-generator.html

Used to generate custom text shadows visually.

---

# Font Best Practices

✅ Use readable fonts

✅ Limit font families

✅ Use rem for scalable typography

✅ Use percentage widths for responsive layouts

✅ Avoid excessive text shadows

✅ Use proper line-height

✅ Use meaningful font weights

---

# Lecture Summary

Topics Covered:

✅ Font Family

✅ Font Weight

✅ Google Fonts

✅ Import Fonts

✅ Download Fonts

✅ Font Size

✅ Default Browser Font Sizes

✅ Relative Units

✅ rem

✅ em

✅ Percentage (%)

✅ Root Element (html)

✅ Absolute Units

✅ px

✅ vh

✅ vw

✅ Border

✅ Font Style

✅ Text Transform

✅ Text Decoration

✅ Line Height

✅ Letter Spacing

✅ Word Spacing

✅ Text Align

✅ Text Shadow

---

# Conclusion

Typography is one of the most important parts of web design.

By using CSS fonts, units, spacing, alignment, and shadows correctly, we can create beautiful, readable, and professional websites.

These concepts are the foundation of responsive and modern web design.
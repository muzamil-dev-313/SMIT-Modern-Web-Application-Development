# 📖 Lecture 07: CSS Selectors, Backgrounds, Priority & Inheritance

## Introduction

CSS allows us to select HTML elements and apply styling.

In this lecture, we learned:

- Background Images
- Background Properties
- CSS Selectors
- CSS Specificity & Priority
- CSS Inheritance

---

# Background Image

Used to place an image in the background of an element.

Syntax:

```css
body {
    background-image: url("image.jpg");
}
```

Example:

```css
body {
    background-image: url("background.jpg");
}
```

---

# Background Repeat

Controls whether the background image repeats.

```css
background-repeat: repeat;
background-repeat: no-repeat;
background-repeat: repeat-x;
background-repeat: repeat-y;
```

### no-repeat

Displays the image only once.

```css
background-repeat: no-repeat;
```

---

# Background Position

Used to control the position of the image.

```css
background-position: center;
background-position: center center;
background-position: top center;
background-position: bottom center;
background-position: left;
background-position: right;
```

Example:

```css
background-position: center center;
```

---

# Background Size

Controls the size of the background image.

### Cover

```css
background-size: cover;
```

The image covers the entire container.

### Contain

```css
background-size: contain;
```

The entire image remains visible.

---

# Background Attachment

Controls scrolling behavior.

```css
background-attachment: scroll;
background-attachment: fixed;
```

Example:

```css
background-attachment: fixed;
```

The image remains fixed while the page scrolls.

---

# CSS Selectors

Selectors are used to target HTML elements.

---

# Universal Selector

Targets all elements.

```css
* {
    margin: 0;
    padding: 0;
}
```

---

# Type Selector

Targets elements by tag name.

```css
h1 {
    color: red;
}
```

---

# Class Selector

Targets elements using a class.

```css
.heading {
    color: blue;
}
```

HTML:

```html
<h1 class="heading">Hello World</h1>
```

---

# ID Selector

Targets a unique element.

```css
#title {
    color: green;
}
```

HTML:

```html
<h1 id="title">Welcome</h1>
```

---

# Descendant Selector

Targets elements inside another element.

```css
div p {
    color: blue;
}
```

HTML:

```html
<div>
    <p>Hello World</p>
</div>
```

---

# Child Selector

Targets direct children only.

```css
div > p {
    color: red;
}
```

Example:

```html
<div>
    <p>Direct Child</p>
</div>
```

---

# Adjacent Sibling Selector

Targets the immediate next sibling.

```css
h2 + p {
    color: green;
}
```

Example:

```html
<h2>Heading</h2>
<p>This paragraph is selected.</p>
```

---

# General Sibling Selector

Targets all siblings after an element.

```css
h2 ~ p {
    color: purple;
}
```

Example:

```html
<h2>Heading</h2>

<p>Paragraph One</p>
<p>Paragraph Two</p>
<p>Paragraph Three</p>
```

All paragraphs will be selected.

---

# CSS Priority (Specificity)

When multiple CSS rules target the same element, CSS decides which style should be applied based on Priority (Specificity).

---

# Example

```html
<h1 id="title" class="heading">
    Welcome
</h1>
```

```css
h1{
    color: blue;
}

.heading{
    color: green;
}

#title{
    color: red;
}
```

Output:

```text
Red
```

Because the ID selector has higher priority than the Class and Element selectors.

---

# CSS Priority Order

Highest Priority → Lowest Priority

1. !important
2. Inline CSS
3. ID Selector
4. Class Selector
5. Element (Type) Selector
6. Universal Selector

---

# 1. !important

The `!important` rule has the highest priority.

Example:

```css
h1{
    color: blue !important;
}

#title{
    color: red;
}
```

Output:

```text
Blue
```

Because `!important` overrides normal CSS rules.

⚠️ Use `!important` only when necessary.

---

# 2. Inline CSS

Inline CSS is written directly inside an HTML element.

```html
<h1 style="color: green;">
    Hello World
</h1>
```

Inline CSS has higher priority than:

- ID Selector
- Class Selector
- Element Selector
- Universal Selector

Example:

```html
<h1 id="title" style="color: green;">
    Welcome
</h1>
```

```css
#title{
    color: red;
}
```

Output:

```text
Green
```

Because Inline CSS wins.

---

# 3. ID Selector

ID selectors have higher priority than classes and elements.

```css
#title{
    color: red;
}
```

```html
<h1 id="title">
    Welcome
</h1>
```

---

# 4. Class Selector

Class selectors have higher priority than element selectors.

```css
.heading{
    color: blue;
}
```

```html
<h1 class="heading">
    Hello
</h1>
```

---

# 5. Element (Type) Selector

Targets HTML tags.

```css
h1{
    color: purple;
}
```

---

# 6. Universal Selector

Lowest priority selector.

```css
*{
    color: black;
}
```

Targets all elements.

---

# External CSS Priority

If two rules have the same priority, the last rule written will be applied.

Example:

```css
h1{
    color: red;
}

h1{
    color: blue;
}
```

Output:

```text
Blue
```

Because the last rule wins.

---

# Internal vs External CSS

Example:

External CSS:

```css
h1{
    color: red;
}
```

Internal CSS:

```html
<style>
h1{
    color: blue;
}
</style>
```

Output:

```text
Blue
```

Because Internal CSS is loaded after External CSS.

---

# Complete Specificity Example

```html
<h1
id="title"
class="heading"
style="color: orange;">
Welcome
</h1>
```

```css
*{
    color:black;
}

h1{
    color:blue;
}

.heading{
    color:green;
}

#title{
    color:red;
}
```

Output:

```text
Orange
```

Because Inline CSS has higher priority than all selectors.

If we use:

```css
h1{
    color: purple !important;
}
```

Output:

```text
Purple
```

Because `!important` has the highest priority.

---

# Final Specificity Order

```text
!important
↓
Inline CSS
↓
ID Selector
↓
Class Selector
↓
Element Selector
↓
Universal Selector
```

Remember:

✅ Higher Specificity Wins

✅ If Specificity is Equal → Last Rule Wins

✅ Avoid Overusing !important

✅ Use Classes for Most Styling

# CSS Inheritance

Inheritance means some CSS properties automatically pass from parent elements to child elements.

Example:

```css
body {
    color: blue;
}
```

```html
<body>
    <p>Hello World</p>
</body>
```

The paragraph automatically inherits the blue color.

---

# Common Inherited Properties

- color
- font-size
- font-family
- text-align
- line-height

---

# Non-Inherited Properties

These properties do not inherit automatically.

- margin
- padding
- border
- width
- height
- background-color

---

# Best Practices

✅ Use classes whenever possible

✅ Keep CSS organized

✅ Use meaningful class names

✅ Prefer external CSS files

✅ Avoid unnecessary selectors

✅ Write clean and readable code

---

# Summary

In this lecture we learned:

✅ Background Image

✅ Background Repeat

✅ Background Position

✅ Background Size

✅ Background Attachment

✅ Universal Selector

✅ Type Selector

✅ Class Selector

✅ ID Selector

✅ Descendant Selector

✅ Child Selector

✅ Adjacent Sibling Selector

✅ General Sibling Selector

✅ CSS Priority

✅ CSS Specificity

✅ CSS Inheritance

---

# Conclusion

CSS Selectors help us target elements efficiently, while Background properties improve webpage design. Understanding Priority and Inheritance is important because they determine how styles are applied to elements.

These concepts are essential before moving to Box Model, Positioning, Flexbox, Grid, and Responsive Design.

# 📖 Lecture 06: Display Property and Visibility

## Introduction

HTML elements are generally divided into two categories:

1. Block Elements
2. Inline Elements

Understanding the difference between them is important for controlling webpage layouts using CSS.

---

# Block Elements

Block elements always start on a new line and occupy the full available width.

Examples:

```html
<h1>Hello</h1>
<p>Paragraph</p>
<div>Container</div>
```

Common Block Elements:

- h1 to h6
- p
- div
- section
- article
- header
- footer

Characteristics:

✅ Starts on a new line

✅ Takes full available width

✅ Width and height can be applied

---

# Inline Elements

Inline elements do not start on a new line.

They only take as much width as needed.

Examples:

```html
<span>Hello</span>
<a href="#">Link</a>
<strong>Important</strong>
```

Common Inline Elements:

- span
- a
- strong
- em
- img

Characteristics:

✅ Stays in the same line

✅ Takes only required width

❌ Width and height usually do not work properly

---

# Changing Display Types

CSS allows us to change the display behavior of elements.

---

## Display: Block

Converts an element into a block element.

Example:

```css
img {
    display: block;
}
```

Now the image starts on a new line.

---

## Display: Inline

Converts an element into an inline element.

Example:

```css
h1 {
    display: inline;
}
```

Now the heading behaves like text.

---

## Display: None

Completely removes an element from the webpage.

Example:

```css
.hidden {
    display: none;
}
```

The element is not displayed and does not occupy space.

---

# Visibility Property

The visibility property controls whether an element is visible.

---

## Visibility Hidden

Example:

```css
.hidden {
    visibility: hidden;
}
```

The element becomes invisible but still occupies its original space.

Difference:

```css
visibility: hidden;
```

✅ Hidden but space remains.

```css
display: none;
```

✅ Hidden and space is removed.

---

# CSS Priority (Introduction)

Sometimes multiple CSS rules target the same element.

Example:

```css
h1 {
    color: red;
}

h1 {
    color: green;
}
```

Result:

```css
green
```

The last rule written is applied because it has higher priority when specificity is equal.

We will study CSS Priority and Specificity next class in detail. 

---

# Example From Class

```css
h1 {
    color: green;
    border: 1px solid;
}

a {
    background-color: aqua;
}

p {
    color: rgb(225, 233, 230);
    background-color: blueviolet;
    font-family: Courier New;
    font-size: 25px;
}

span {
    background-color: brown;
}

img {
    display: block;
}

.hidden {
    visibility: hidden;
}
```

---

# Important Points

✅ Block elements start on a new line

✅ Inline elements stay in the same line

✅ Width and height work on block elements

✅ Width and height generally do not work on inline elements

✅ display:block converts inline to block

✅ display:inline converts block to inline

✅ display:none removes the element completely

✅ visibility:hidden hides the element but keeps its space

---

# Conclusion

In this lecture, we learned:

- Block Elements
- Inline Elements
- Display Property
- display:block
- display:inline
- display:none
- visibility:hidden
- Basic CSS Priority

These concepts are important for webpage layout and styling.


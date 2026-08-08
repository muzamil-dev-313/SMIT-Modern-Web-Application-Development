# 🎨 Lecture 05: Introduction to CSS

## What is CSS?

CSS stands for **Cascading Style Sheets**.

CSS is used to style and design HTML webpages. HTML provides the structure of a webpage, while CSS makes it attractive and visually appealing.

### Why CSS?

Without CSS:

- Websites look plain
- No colors
- No styling
- Poor user experience

With CSS:

- Attractive designs
- Better layouts
- Improved readability
- Professional appearance

---

# CSS Syntax

CSS follows this structure:

```css
selector {
    property: value;
}
```

Example:

```css
h1 {
    color: blue;
}
```

### Parts of CSS

- Selector → `h1`
- Property → `color`
- Value → `blue`

---

# Types of CSS

## 1. Inline CSS

Inline CSS is applied directly inside an HTML element using the `style` attribute.

Example:

```html
<h1 style="color: blue;">Hello World</h1>
```

### Advantages

- Quick styling
- Useful for testing

### Disadvantages

- Difficult to manage
- Not recommended for large projects

---

## 2. Internal CSS

Internal CSS is written inside the `<style>` tag within the `<head>` section.

Example:

```html
<head>
    <style>
        h1{
            color:red;
        }
    </style>
</head>
```

### Advantages

- Easy for small projects
- Keeps styling inside one file

---

## 3. External CSS

External CSS is written in a separate `.css` file.

HTML File:

```html
<link rel="stylesheet" href="style.css">
```

CSS File:

```css
h1{
    color:green;
}
```

### Advantages

- Best practice
- Reusable
- Easy to maintain
- Cleaner code

---

# CSS Selectors

Selectors are used to target HTML elements.

---

## Tag Selector

Targets all elements of a specific tag.

```css
p{
    color:red;
}
```

Example:

```html
<p>Hello World</p>
```

---

## Class Selector

Targets elements using a class name.

HTML:

```html
<p class="info">Hello</p>
```

CSS:

```css
.info{
    color:blue;
}
```

Class selectors start with a dot (`.`).

---

## ID Selector

Targets a specific element using its ID.

HTML:

```html
<h1 id="title">Welcome</h1>
```

CSS:

```css
#title{
    color:red;
}
```

ID selectors start with a hash (`#`).

---

## Div Selector

The `<div>` element is commonly used as a container.

HTML:

```html
<div class="box">
    Content Here
</div>
```

CSS:

```css
.box{
    background-color:lightblue;
}
```

---

## Span Selector

The `<span>` element is an inline container.

HTML:

```html
<p>Hello <span class="highlight">World</span></p>
```

CSS:

```css
.highlight{
    color:green;
}
```

---

# CSS Properties and Values

A CSS rule contains a property and a value.

Example:

```css
color: blue;
```

- Property → `color`
- Value → `blue`

Example:

```css
background-color: lightgray;
```

- Property → `background-color`
- Value → `lightgray`

---

# Text Alignment

Used to align text.

### Left Alignment

```css
text-align:left;
```

### Center Alignment

```css
text-align:center;
```

### Right Alignment

```css
text-align:right;
```

Example:

```css
h1{
    text-align:center;
}
```

---

# Background Color

Used to change the background color of an element.

Example:

```css
body{
    background-color:lightgray;
}
```

Another Example:

```css
div{
    background-color:skyblue;
}
```

---

# Border Property

Used to create borders around elements.

Example:

```css
border:2px solid black;
```

### Border Components

```css
border-width:2px;
border-style:solid;
border-color:red;
```

---

# Border Styles

Common border styles:

```css
solid
dashed
dotted
double
groove
ridge
```

Example:

```css
border:3px dashed blue;
```

---

# Colors in CSS

CSS supports multiple color formats.

---

## Color Names

Example:

```css
color:red;
```

Other Examples:

```css
blue
green
yellow
black
white
purple
```

---

## RGB Colors

RGB stands for:

- Red
- Green
- Blue

Example:

```css
color:rgb(255,0,0);
```

Range:

```text
0 - 255
```

---

## RGBA Colors

RGBA includes transparency.

Example:

```css
color:rgba(255,0,0,0.5);
```

A = Alpha (Transparency)

Range:

```text
0.0 - 1.0
```

---

## HEX Colors

Hexadecimal color values.

Example:

```css
color:#ff0000;
```

Examples:

```css
#000000
#ffffff
#ff0000
#00ff00
#0000ff
```

---

## HSL Colors

HSL stands for:

- Hue
- Saturation
- Lightness

Example:

```css
color:hsl(0,100%,50%);
```

---

# CSS Best Practices

✅ Use External CSS whenever possible

✅ Use meaningful class names

✅ Keep code clean and organized

✅ Use proper indentation

✅ Avoid excessive Inline CSS

✅ Reuse classes when possible

✅ Write readable CSS

---

# Practice Topics Covered

### CSS Introduction

- What is CSS
- Why CSS

### Types of CSS

- Inline CSS
- Internal CSS
- External CSS

### Selectors

- Tag Selector
- Class Selector
- ID Selector
- Div Selector
- Span Selector

### Properties

- color
- background-color
- text-align
- border

### Colors

- Named Colors
- RGB
- RGBA
- HEX
- HSL

---

# Conclusion

CSS (Cascading Style Sheets) is used to style HTML webpages.

HTML creates the structure, while CSS controls the appearance and design.

By learning CSS, you can create professional, responsive, and visually attractive websites.


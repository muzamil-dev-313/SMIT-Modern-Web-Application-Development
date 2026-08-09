# 📖 Lecture 08: CSS Colors, Opacity & Color Systems

## Introduction

Colors play a very important role in web design. They improve user experience, readability, branding, and visual appeal.

In this lecture, we learned:

- Understanding Colors
- RGB Colors
- RGBA Colors
- HEX Colors
- Color Names
- HSL Colors
- HSLA Colors
- Opacity
- Alpha Channel
- Color Contrast
- Hue, Saturation & Lightness

---

# Understanding Colors

Computer monitors are made up of thousands of tiny squares called **pixels**.

Each pixel displays a combination of:

- Red
- Green
- Blue

These three colors combine to create millions of different colors on the screen.

This is known as the **RGB Color Model**.

---

# RGB Colors

RGB stands for:

- Red
- Green
- Blue

Each value ranges from:

```text
0 → 255
```

Syntax:

```css
color: rgb(red, green, blue);
```

Example:

```css
color: rgb(255, 0, 0);
```

Output:

```text
Red
```

---

# RGB Examples

### Red

```css
rgb(255, 0, 0)
```

### Green

```css
rgb(0, 255, 0)
```

### Blue

```css
rgb(0, 0, 255)
```

### Yellow

```css
rgb(255, 255, 0)
```

Explanation:

```text
255 Red
255 Green
0 Blue
```

Red + Green = Yellow

---

### White

```css
rgb(255, 255, 255)
```

Maximum values of all colors.

---

### Black

```css
rgb(0, 0, 0)
```

No color/light.

---

# RGBA Colors

RGBA stands for:

- Red
- Green
- Blue
- Alpha

Alpha controls transparency.

Syntax:

```css
rgba(red, green, blue, alpha);
```

Example:

```css
background-color: rgba(255, 0, 0, 0.5);
```

---

# Alpha Channel

Alpha determines transparency.

Range:

```text
0 → 1
```

Examples:

```css
rgba(255,0,0,1)
```

Fully visible.

```css
rgba(255,0,0,0.5)
```

50% transparent.

```css
rgba(255,0,0,0)
```

Completely invisible.

---

# HEX Colors

HEX (Hexadecimal) colors are another way to represent RGB values.

Syntax:

```css
#RRGGBB
```

Example:

```css
#66cdaa
```

Explanation:

```text
66 = Red
CD = Green
AA = Blue
```

Equivalent RGB:

```css
rgb(102,205,170)
```

---

# Color Names

Browsers support predefined color names.

Examples:

```css
color: red;
color: blue;
color: green;
color: yellow;
```

Example:

```css
color: MediumAquaMarine;
```

There are approximately 147 supported color names.

---

# HSL Colors

HSL stands for:

- Hue
- Saturation
- Lightness

Syntax:

```css
hsl(hue, saturation, lightness);
```

Example:

```css
hsl(120, 100%, 50%);
```

Output:

```text
Green
```

---

# Hue

Hue represents the actual color.

Range:

```text
0° → 360°
```

Examples:

```text
0° = Red
120° = Green
240° = Blue
360° = Red
```

---

# Saturation

Saturation controls the amount of gray.

Range:

```text
0% → 100%
```

### 100%

Pure color.

### 0%

Completely gray.

Example:

```css
hsl(120,100%,50%)
```

Very vibrant green.

---

# Lightness

Lightness controls brightness and darkness.

Range:

```text
0% → 100%
```

### 0%

Black

### 50%

Normal Color

### 100%

White

Example:

```css
hsl(240,100%,50%)
```

Blue

---

# HSLA Colors

HSLA stands for:

- Hue
- Saturation
- Lightness
- Alpha

Syntax:

```css
hsla(240,100%,50%,0.5);
```

Alpha controls transparency.

---

# Opacity

The opacity property controls transparency of an entire element.

Syntax:

```css
opacity: 0.5;
```

Range:

```text
0 → 1
```

### Example

```css
opacity: 1;
```

Fully visible.

```css
opacity: 0.5;
```

50% visible.

```css
opacity: 0;
```

Invisible.

---

# Color Contrast

Color contrast is the difference between text color and background color.

Good contrast improves readability.

---

# High Contrast

Easy to read.

Example:

```css
background-color: black;
color: white;
```

---

# Low Contrast

Difficult to read.

Example:

```css
background-color: lightgray;
color: white;
```

---

# Medium Contrast

Readable but not ideal.

Example:

```css
background-color: gray;
color: white;
```

---

# Color Contrast Checker Tools

Useful websites:

### WebAIM Contrast Checker

https://webaim.org/resources/contrastchecker/

### Coolors Contrast Checker

https://coolors.co/contrast-checker

### Adobe Color

https://color.adobe.com

---

# CSS Color Formats Summary

| Format | Example |
|----------|----------|
| Color Name | red |
| RGB | rgb(255,0,0) |
| RGBA | rgba(255,0,0,0.5) |
| HEX | #ff0000 |
| HSL | hsl(0,100%,50%) |
| HSLA | hsla(0,100%,50%,0.5) |

---

# pH Scale Assignment

In today's class we created a pH Scale project using different color shades.

Concepts Used:

✅ Background Colors

✅ HEX Colors

✅ Color Shades

✅ Typography

✅ CSS Selectors

✅ Layout Spacing

Example:

```css
.fourteen{
    background-color:#3185c6;
}
```

Different shades were used to represent:

- Alkaline Values
- Neutral Value
- Acidic Values

This project helped us understand color selection and visual hierarchy.

---

# Quiz Activity

Today we also completed an HTML Quiz to revise:

---

# Best Practices

✅ Maintain good color contrast

✅ Use HEX or RGB for consistency

✅ Avoid too many bright colors

✅ Test readability on different screens

✅ Use opacity carefully

✅ Follow accessibility guidelines

---

# Summary

In this lecture we learned:

✅ Understanding Colors

✅ RGB Colors

✅ RGBA Colors

✅ Alpha Channel

✅ HEX Colors

✅ Color Names

✅ HSL Colors

✅ HSLA Colors

✅ Opacity

✅ Hue

✅ Saturation

✅ Lightness

✅ Color Contrast

✅ Contrast Checker Tools

✅ pH Scale Project

---

# Conclusion

Colors are one of the most important parts of web design. Understanding RGB, HEX, HSL, Opacity, and Contrast helps developers create visually appealing and accessible websites.

A good developer not only makes websites functional but also makes them beautiful and easy to read.

🎨 Good Colors Improve User Experience

💡 Good Contrast Improves Accessibility

🚀 Keep Practicing CSS Daily

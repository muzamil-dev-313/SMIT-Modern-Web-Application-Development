# 📖 Lecture 03: HTML Forms and Input Types

## Introduction

HTML forms are used to collect information from users and send data to a server.

Forms are one of the most important parts of web development because they allow users to interact with websites.

Basic Form Structure:

```html
<form>
    <!-- Form Elements -->
</form>
```

---

# Form Elements

## Label

The <label> tag provides a description for an input field.

```html
<label for="name">Full Name:</label>
```

---

## Input Tag

The <input> tag is used to collect user data.

```html
<input type="text">
```

Different input types are available for different purposes.

---

# Input Types

## 1. Text Input

Used to enter normal text.

```html
<input type="text">
```

Example:

- Name
- Username
- City

---

## 2. Email Input

Used to enter email addresses.

```html
<input type="email">
```

Example:

- example@gmail.com

---

## 3. Password Input

Used to hide typed characters.

```html
<input type="password">
```

Example:

- Login Password
- Account Password

---

## 4. Number Input

Used to enter numeric values.

```html
<input type="number">
```

Example:

- Age
- Experience
- Salary

---

## 5. Telephone Input

Used to enter phone numbers.

```html
<input type="tel">
```

Example:

- Mobile Number

---

## 6. Date Input

Used to select a date.

```html
<input type="date">
```

Example:

- Date of Birth

---

## 7. Time Input

Used to select time.

```html
<input type="time">
```

Example:

- Interview Time

---

## 8. DateTime Local

Used to select both date and time.

```html
<input type="datetime-local">
```

---

## 9. File Upload

Allows users to upload files.

```html
<input type="file">
```

Example:

- Resume
- Profile Picture

---

## 10. URL Input

Used to enter website links.

```html
<input type="url">
```

Example:

- Portfolio Website
- GitHub Profile

---

## 11. Color Picker

Allows users to select colors.

```html
<input type="color">
```

---

## 12. Range Input

Creates a slider.

```html
<input type="range">
```

Example:

- Salary Range
- Volume Control

---

# Radio Buttons

Radio buttons allow users to select only one option from a group.

```html
<input type="radio" name="gender">
```

Example:

- Male
- Female
- Other

---

# Checkboxes

Checkboxes allow users to select multiple options.

```html
<input type="checkbox">
```

Example Skills:

- HTML
- CSS
- JavaScript
- Python

---

# Select Dropdown

Used to create a dropdown menu.

```html
<select>
    <option>HTML</option>
    <option>CSS</option>
</select>
```

Example:

- Job Categories
- Country Selection

---

# Textarea

Used for multi-line text input.

```html
<textarea rows="5" cols="30"></textarea>
```

Example:

- Feedback
- Comments
- Cover Letter

---

# Buttons

## Submit Button

Used to submit form data.

```html
<input type="submit">
```

---

## Button Element

```html
<button>Submit</button>
```

---

# Attributes Used in Forms

## Placeholder

Displays hint text.

```html
<input type="text" placeholder="Enter your name">
```

---

## Required

Makes an input field mandatory.

```html
<input type="email" required>
```

---

## Value

Provides a default value.

```html
<input type="submit" value="Register">
```

---

## Selected

Sets the default selected option.

```html
<option selected>HTML</option>
```

---

# Practice Project

Job Application Form

Concepts Used:

- Form
- Label
- Text Input
- Email Input
- Password Input
- Number Input
- Telephone Input
- Date Input
- Time Input
- DateTime Local
- Radio Buttons
- Checkboxes
- Dropdown Menu
- File Upload
- URL Input
- Color Picker
- Range Input
- Textarea
- Submit Button

---

# Summary

Topics Covered:

- Forms
- Labels
- Input Tag
- Input Types
- Radio Buttons
- Checkboxes
- Select & Option
- Textarea
- Buttons
- File Upload
- URL Input
- Color Picker
- Range Input
- Form Attributes

Forms are used to collect information from users and are an essential part of modern websites.

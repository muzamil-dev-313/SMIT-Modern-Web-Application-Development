# 📖 Lecture 02: HTML Tables and Forms

## HTML Tables

Tables are used to organize data into **rows and columns**. They help display structured information such as student records, employee data, marksheets, and schedules.

### Basic Table Structure

```html
<table border="1">
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>Muzamil</td>
        <td>21</td>
    </tr>
</table>
```

### Output

| Name | Age |
|------|-----|
| Muzamil | 21 |

---

## Understanding Table Tags

### `<table>`

The `<table>` tag is the main container used to create a table.

```html
<table>
    ...
</table>
```

All table elements must be placed inside the `<table>` tag.

---

### `<tr>` (Table Row)

The `<tr>` tag creates a **row** in a table.

Example:

```html
<tr>
    <td>Muzamil</td>
    <td>21</td>
</tr>
```

This creates one row containing two cells.

---

### `<th>` (Table Header)

The `<th>` tag creates a **heading cell**.

Text inside `<th>` is usually:

- Bold
- Center aligned

Example:

```html
<th>Name</th>
<th>Age</th>
```

Output:

| Name | Age |

---

### `<td>` (Table Data)

The `<td>` tag creates a normal data cell.

Example:

```html
<td>Muzamil</td>
<td>21</td>
```

Output:

| Muzamil | 21 |

---

## How Rows and Columns Work

Example:

```html
<table border="1">
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>Muzamil</td>
        <td>21</td>
    </tr>

    <tr>
        <td>Ali</td>
        <td>20</td>
    </tr>
</table>
```

### Table Structure

| Name | Age |
|------|-----|
| Muzamil | 21 |
| Ali | 20 |

Explanation:

- The first `<tr>` creates the header row.
- The second `<tr>` creates the first data row.
- The third `<tr>` creates the second data row.
- `<th>` is used for headings.
- `<td>` is used for actual data.

---

## HTML Forms

Forms are used to collect information from users.

Examples:

- Login Form
- Registration Form
- Contact Form
- Feedback Form

### Basic Form Structure

```html
<form>
    <label>Name:</label>
    <input type="text">

    <br><br>

    <label>Email:</label>
    <input type="email">

    <br><br>

    <button>Submit</button>
</form>
```

---

## Common Form Elements

### `<form>`

The main container that holds all form elements.

```html
<form>
    ...
</form>
```

---

### `<label>`

Provides a label or description for an input field.

```html
<label>Name:</label>
```

---

### `<input>`

Used to accept user input.

Examples:

```html
<input type="text">
<input type="email">
<input type="password">
<input type="number">
```

---

### `<textarea>`

Used for multi-line text input.

```html
<textarea></textarea>
```

Example use:

- Comments
- Feedback
- Messages

---

### `<button>`

Creates a clickable button.

```html
<button>Submit</button>
```

---

## Common Form Elements Summary

| Element | Purpose |
|----------|----------|
| `<form>` | Creates a form |
| `<label>` | Defines labels |
| `<input>` | Accepts user input |
| `<textarea>` | Multi-line text input |
| `<button>` | Creates a button |

---

## Key Concepts Learned

### HTML Tables

- Creating tables
- Rows and columns
- Table headings
- Table data cells
- Organizing information

### HTML Forms

- Collecting user data
- Labels
- Input fields
- Text areas
- Buttons

---

## Conclusion

HTML Tables are used to display structured data in rows and columns, while HTML Forms are used to collect information from users through input fields and buttons.


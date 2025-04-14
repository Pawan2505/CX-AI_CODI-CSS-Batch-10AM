# 📘 **CSS Text Properties**

---

## 🔸 **What are Text Properties in CSS?**

Text properties help in designing the appearance of text in a webpage.  
They control size, color, alignment, spacing, decoration, and more.

---

## ✅ **Common Text Properties:**

| Property           | Description                                           | Example                          |
|--------------------|-------------------------------------------------------|----------------------------------|
| `color`            | Changes the color of text                            | `color: green;`                  |
| `font-size`        | Sets the size of the text                            | `font-size: 24px;`               |
| `font-family`      | Sets the typeface/font of text                       | `font-family: Arial;`            |
| `font-weight`      | Makes text bold or light                             | `font-weight: 500;`              |
| `font-style`       | Italic or normal font style                          | `font-style: italic;`            |
| `text-align`       | Aligns text (left, right, center, justify)           | `text-align: center;`            |
| `line-height`      | Sets space between lines                             | `line-height: 50px;`             |
| `letter-spacing`   | Sets space between letters                           | `letter-spacing: 2px;`           |
| `word-spacing`     | Sets space between words                             | `word-spacing: 10px;`            |
| `text-decoration`  | Adds underline, overline, etc.                       | `text-decoration: underline;`    |
| `text-transform`   | Changes case (uppercase, lowercase, capitalize)      | `text-transform: lowercase;`     |
| `text-indent`      | Indents the first line of paragraph                  | `text-indent: 200px;`            |
| `list-style`       | Removes bullets from list                            | `list-style: none;`              |

---

## 🔸 **CSS Code Examples:**

### 🧾 Paragraph Styling
```css
.para {
    color: green;
    font-size: 24px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 500;
    line-height: 50px;
    letter-spacing: 2px;
    word-spacing: 10px;
    text-indent: 200px;
    text-decoration: underline;
}
```

### 🧾 Anchor Tag Styling
```css
a {
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}
```

### 🧾 Heading Styling
```css
#heading {
    text-align: center;
}
```

### 🧾 Text Transform Example
```css
.para-second {
    text-transform: lowercase;  /* Other options: capitalize, uppercase */
}
```

### 🧾 List Style Example (Optional)
```css
li {
    list-style: none;
}
```

---

## 💡 Note:

- Use **`text-transform`** to change letter case without changing HTML text.
- **`letter-spacing`** and **`word-spacing`** improve readability in designs.
- Avoid overusing **`text-indent`** unless needed for design formatting.
- Combine multiple text properties for beautiful typography!

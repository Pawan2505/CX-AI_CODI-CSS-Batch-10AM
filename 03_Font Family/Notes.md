## 📒 **CSS - Online Font Family**

---

### 🔶 **What is a Font Family?**
A **font-family** defines the typeface used to display the text.  
Example: Arial, Verdana, Times New Roman, etc.

---

### 🔶 **What is an Online Font?**
- Fonts that are loaded from the **internet**, not your computer.
- Most popular source: **Google Fonts**
- These fonts make web pages look beautiful and stylish.

---

### 🔶 **How to Use Google Fonts (2 Ways)**

#### 1. Using `<link>` in HTML `<head>` (Recommended):
```html
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
```

#### 2. Using `@import` inside CSS:
```css
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
```

---

### 🔶 **Apply Online Font to Text:**
```css
p {
  font-family: 'Roboto', sans-serif;
}
```

📝 Use the font name from Google Fonts. Always add a backup font like `sans-serif`.

---

### 🔶 Example (Google Font: Edu AU VIC WA NT Arrows):

```css
@import url('https://fonts.googleapis.com/css2?family=Edu+AU+VIC+WA+NT+Arrows:wght@400..700&display=swap');

p {
  font-family: "Edu AU VIC WA NT Arrows", cursive;
}
```

---

### 🔶 Extra: `font-optical-sizing`  
Used with **variable fonts**  
Automatically adjusts for different screen sizes and weights  
```css
font-optical-sizing: auto;
```

---

### 🔶 Why Use Online Fonts?
- For stylish, modern typography  
- No need to install fonts manually  
- Easy to use  
- Loads fast and improves design


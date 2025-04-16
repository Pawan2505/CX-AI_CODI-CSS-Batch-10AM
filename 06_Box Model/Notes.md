## 📒 **Box Model**
---

Every HTML element is like a **box**. This box has 4 parts:

```
|  MARGIN   |
|  BORDER   |
|  PADDING  |
|  CONTENT  |
```

Let’s understand each part in simple terms.

---

### 1️⃣ **Content**
👉 This is the actual text or image inside the box.

```html
<div>Hello World</div>
```

---

### 2️⃣ **Padding**
👉 Space **inside** the box – between **content** and **border**.

```css
padding: 20px;
```

Padding increases inner spacing.

---

### 3️⃣ **Border**
👉 Line around the padding/content.

```css
border: 2px solid red;
```

You can change:
- **Size** → `2px`
- **Style** → `solid`, `dashed`, `dotted`
- **Color** → `red`, `green`, etc.

---

### 4️⃣ **Margin**
👉 Space **outside** the box. Creates distance from other elements.

```css
margin: 30px;
```

Good for spacing between boxes.

---

### 🧠 Extra: Box Sizing

Normally:
```
Total Width = width + padding + border
```

To fix that and include everything inside width:

```css
box-sizing: border-box;
```

Now the box won't overflow due to padding/border.

---

### 🎨 Background Color

```css
background-color: lightblue;
```

🎯 Sets background of the element.

---

### 🔁 Border Radius

```css
border-radius: 10px;
```

👉 Makes the corners **rounded**

```css
border-radius: 50%;
```

🎯 Makes a **circle** (if width = height)

---

### Example

```html
<div class="box">Hello</div>
```

```css
.box {
    width: 200px;
    height: 200px;
    background-color: lightblue;
    padding: 20px;
    margin: 30px;
    border: 2px solid black;
    border-radius: 10px;
    box-sizing: border-box;
}
```

📝 This box will have:
- Light blue background
- 20px space inside (padding)
- 2px black border
- 30px gap around it (margin)
- Rounded corners (10px)
- Everything fits nicely inside defined width (due to `box-sizing`)


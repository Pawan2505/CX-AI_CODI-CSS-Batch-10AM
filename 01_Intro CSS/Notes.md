## CSS – Introduction
(Types of CSS + Selectors)

---

## What is CSS?

- **CSS** stands for **Cascading Style Sheets**.  
- It is used to **style** web pages.  
- With CSS, you can change the color, font size, background, layout, and much more.

---

## Types of CSS

### 1. Inline CSS

- This CSS is written **directly inside the HTML element**.  
- It is used for applying styles to individual elements.  
- Example:
  ```html
  <p style="color: red;">Hello</p>
  ```

- Not recommended for large projects as it can make the code messy.

---

### 2. Internal CSS

- This CSS is written inside the **<head> section** of the HTML page, within a `<style>` tag.  
- It only applies to the page it is written on.  
- Example:
  ```html
  <style>
    h1 {
      color: blue;
    }
  </style>
  ```

---

### 3. External CSS

- This is the best and most **professional way** to use CSS.  
- The CSS is written in a **separate file** (e.g., `style.css`) and linked to the HTML page.  
- Example:
  ```html
  <link rel="stylesheet" href="style.css">
  ```

- In the `style.css` file:
  ```css
  body {
    background-color: lightgray;
    font-family: Arial;
  }
  ```

---

## CSS Selectors

Selectors are used to **target HTML elements** that you want to style.

### 1. Tag Selector

- This applies style to **all elements of a certain type** (like all `<p>`, `<h1>`, etc.).  
- Example:
  ```css
  p {
    color: green;
  }
  ```

---

### 2. Class Selector

- This applies style to **multiple elements** with the same class.  
- You use a **dot (.)** before the class name.  
- Example:
  ```css
  .box {
    background: yellow;
    padding: 10px;
  }
  ```

  ```html
  <div class="box">Hello</div>
  ```

---

### 3. ID Selector

- This applies style to a **unique element** with a specific ID.  
- You use a **hash (#)** before the ID name.  
- Example:
  ```css
  #header {
    color: purple;
    font-size: 30px;
  }
  ```

  ```html
  <h1 id="header">Welcome</h1>
  ```

---

## Note:

| Selector  | Use              | CSS Syntax    | HTML Syntax                |
|-----------|------------------|---------------|----------------------------|
| Tag       | All elements     | `p {}`        | `<p>...</p>`                |
| Class     | Multiple elements| `.class {}`   | `class="..."`              |
| ID        | Unique element   | `#id {}`      | `id="..."`                 |

---

## Tips:

- **Inline CSS** – Use it for quick testing or for a small style change.  
- **Internal CSS** – Use it for styling a single page.  
- **External CSS** – Use it for professional projects, especially when there are multiple pages.  
- Use **Class** selectors for styling many elements.  
- Use **ID** selectors for unique elements.


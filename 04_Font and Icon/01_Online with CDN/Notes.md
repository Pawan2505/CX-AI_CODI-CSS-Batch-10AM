# **Fonts & Icons Attachment**

**Topics Covered:**

- Font Attachment (Offline)
- Icon Attachment using IcoMoon
- Remix Icon Attachment
- Practice Example using Fonts and Icons

---

## Fonts Attachment (Offline Method)

Fonts define the overall look and readability of our webpage content. Instead of using system-default fonts like Arial or Times New Roman, we can use custom fonts to make the design more attractive.

### Steps for Offline Font Attachment:

1. First, download a custom font from websites like:

   - [Google Fonts](https://fonts.google.com)
   - [DaFont](https://www.dafont.com)

2. Place the downloaded font files (usually `.woff`, `.woff2`, or `.ttf`) inside a folder named `fonts` in your project directory.

3. Use the `@font-face` rule in your `<style>` section to register the font.

Example:

```html
<style>
  @font-face {
    font-family: "MyCustomFont";
    src: url("fonts/myfont.woff2") format("woff2"), url("fonts/myfont.woff")
        format("woff");
  }

  body {
    font-family: "MyCustomFont", sans-serif;
  }
</style>
```

Points to remember:

- Use multiple font formats for better browser support.
- Always include a fallback font like `sans-serif` or `serif`.

---

## Icon Attachment using IcoMoon (Offline)

IcoMoon allows us to create our own icon sets and use them like fonts. These icons are lightweight and scalable.

### Steps to Use IcoMoon Offline:

1. Go to [IcoMoon App](https://icomoon.io/app)
2. Select the icons you want and click on **Generate Font**
3. Download the zip file and extract it
4. Place the `style.css` file and `fonts` folder into your project

Now include the CSS file in your HTML and use icon class names directly.

Example:

```html
<head>
  <link rel="stylesheet" href="icomoon/style.css" />
</head>
<body>
  <i class="icon-home"></i>
  <p class="icon-user">Welcome</p>
</body>
```

The `icon-home` or `icon-user` classes are defined in the IcoMoon CSS file.

---

## Remix Icon Attachment (Using CDN)

Remix Icon is an open-source icon library available through CDN. It's very easy to integrate in web projects.

### Steps to Use Remix Icon:

1. Add the CDN link inside the `<head>` section of your HTML file

```html
<link
  href="https://cdn.jsdelivr.net/npm/remixicon/fonts/remixicon.css"
  rel="stylesheet"
/>
```

2. Use icon class names directly in the HTML

Example:

```html
<i class="ri-home-line"></i> <i class="ri-user-fill"></i>
```

You can explore more icons and class names here: [Remix Icon Official Website](https://remixicon.com)

---

## Practice Example – Font and Icon Attachment Together

This example uses:

- Offline custom font for headings and paragraph
- IcoMoon icons for contact
- Remix icons for user and home

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Font and Icon Example</title>

    <!-- Offline Font -->
    <style>
      @font-face {
        font-family: "MyFont";
        src: url("fonts/myfont.woff2") format("woff2");
      }
      body {
        font-family: "MyFont", sans-serif;
      }
    </style>

    <!-- IcoMoon Icon CSS -->
    <link rel="stylesheet" href="icomoon/style.css" />

    <!-- Remix Icon CDN -->
    <link
      href="https://cdn.jsdelivr.net/npm/remixicon/fonts/remixicon.css"
      rel="stylesheet"
    />
  </head>
  <body>
    <h1><i class="ri-home-line"></i> Welcome to My Page</h1>
    <p>This text is displayed using an offline custom font.</p>

    <p><i class="icon-phone"></i> Call us at: +91-9999999999</p>
    <p><i class="ri-user-fill"></i> User Profile</p>
  </body>
</html>
```

---

## Note:

- Use **offline fonts** when you want full control and when working without internet access.
- Use **IcoMoon** if you want to create custom icon packs that are lightweight and offline.
- Use **Remix Icon** for quick integration using internet-based CDN.

Both offline and online methods are important depending on the project need. Practice both to become comfortable with each approach.

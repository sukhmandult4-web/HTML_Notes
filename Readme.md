# 🌐 Web Development Notes

## 🚀 Introduction to Web Development

Client ↔️ Browser ↔️ Server

- Client sends a request through the browser.
- Server processes the request and sends a response.
- Frontend consists of:
  - 🏗️ HTML → Structure
  - 🎨 CSS → Design
  - ⚡ JavaScript → Interaction and Logic

### 📄 HTML (HyperText Markup Language)

- HTML is used to create websites.
- HTML provides the structure of a webpage.
- CSS is used to add styling and design.
- JavaScript is used to add functionality and logic.

### 🧱 Basic HTML Structure

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Website</title>
</head>
<body>
    <h1>Heading</h1>
    <p>Paragraph</p>
</body>
</html>
```

Explanation:

- `<!DOCTYPE html>` specifies that this is an HTML document.
- `<html>` is the root element.
- `<head>` contains metadata.
- `<title>` sets the title of the webpage.
- `<body>` contains the visible content.

---

# 🏷️ HTML Attributes

Attributes provide additional information about HTML elements.

Example:

```html
<h1 align="center">Heading</h1>
```

---

# 📝 Headings

HTML provides six heading levels.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

- `<h1>` is the largest heading.
- Font size decreases from h1 to h6.

---

# 📄 Paragraph Tag

```html
<p>This is a paragraph.</p>
```

Used to display paragraphs.

---

# 🔗 Anchor Tag

Used to add links.

```html
<a href="https://example.com">Visit Website</a>
```

### Types of Links

- Relative Link → Link to your own webpage.
- Absolute Link → Link to an external website.

### Open Link in New Tab

```html
<a target="_blank" href="https://example.com">
    Open Website
</a>
```

---

# ➖ Horizontal Rule

```html
<hr>
```

Adds a horizontal line.

---

# ✍️ Bold and Italic

```html
<b>Bold Text</b>

<i>Italic Text</i>
```

---

# 🖼️ Image Tag

Used to add images.

```html
<img src="image.png" alt="Image Description">
```

### Alt Attribute

- Displays text if the image cannot load.
- Helps search engines understand the image.

### Width and Height

```html
<img src="image.png" width="230" height="200" alt="Image">
```

Used to change image size.

---

# 📊 Table Tag

Used to create tables.

```html
<table>
    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>John</td>
        <td>20</td>
    </tr>
</table>
```

### Table Elements

- `<table>` → Table
- `<tr>` → Table Row
- `<th>` → Table Heading
- `<td>` → Table Data

---

# 🔀 Colspan and Rowspan

Used to merge columns and rows.

### Rowspan

```html
<td rowspan="2">Data</td>
```

### Colspan

```html
<td colspan="2">Data</td>
```

Default value = 1

---

# 📌 Caption

Used to provide information about the table.

```html
<table>
    <caption>Student Details</caption>
</table>
```

---

# 📑 Table Headers and Footers

Help in grouping table content.

```html
<table>

    <thead>
        Table Head Details
    </thead>

    <tbody>
        Table Body Details
    </tbody>

    <tfoot>
        Table Footer Details
    </tfoot>

</table>
```

---

# 📋 Lists

Three Types of Lists:

1. Unordered List
2. Ordered List
3. Definition List

---

## 🔹 Unordered List

Displays items using bullets.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
</ul>
```

### Square Bullets

```html
<ul type="square">
    <li>Item</li>
</ul>
```

---

## 🔢 Ordered List

Displays items in numerical sequence.

```html
<ol>
    <li>Item 1</li>
    <li>Item 2</li>
</ol>
```

### Ordered List Types

Uppercase Roman Numbers

```html
<ol type="I">
```

Lowercase Roman Numbers

```html
<ol type="i">
```

Arabic Numbers

```html
<ol type="1">
```

Lowercase Alphabet

```html
<ol type="a">
```

Uppercase Alphabet

```html
<ol type="A">
```

---

## 📖 Definition List

Used like a dictionary.

```html
<dl>

    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>

</dl>
```

- `<dt>` → Definition Term
- `<dd>` → Definition Data

---

# 🔍 SEO (Search Engine Optimization)

Used to improve website visibility on search engines.

## 📈 Core Web Vitals

### CLS (Cumulative Layout Shift)

Measures visual stability of a webpage.

To improve CLS:

- Use width and height for images.
- Avoid layout shifts.

### LCP (Largest Contentful Paint)

Measures loading time of the largest element.

Good LCP Score:

- Less than 2.5 seconds

### ⚡ FID (First Input Delay)

Measures how quickly the page responds after user interaction.

Good FID Score:

- Less than 100 milliseconds

---

## 🏷️ Meta Description

Used to describe a webpage.

```html
<meta
    name="description"
    content="Description of your webpage">
```

Helps improve SEO.

---

# 📝 Forms in HTML

Forms collect user input.

```html
<form>

    Form Elements

</form>
```

---

## ⌨️ Input Element

Used for different types of input.

```html
<input type="text">
```

Other Types:

```html
<input type="password">
<input type="radio">
<input type="checkbox">
<input type="submit">
<input type="file">
<input type="email">
```

---

## 📝 Textarea

Used for multiline input.

```html
<textarea rows="4" cols="50"></textarea>
```

Example:

```html
<label for="comment">
    Enter Your Comment
</label>

<textarea
id="comment"
name="comment"
rows="4"
cols="50">
</textarea>
```

---

## ⬇️ Select Tag

Creates a dropdown menu.

```html
<select>

    <option>Male</option>
    <option>Female</option>

</select>
```

---

# ⚙️ Form Attributes

## Action

Specifies where form data is sent.

```html
<form action="url">
```

## Method

Defines how data is sent.

### GET

Used for limited data.

```html
<form method="GET">
```

### POST

Used for large amounts of data.

```html
<form method="POST">
```

## Name

Specifies the name of the form element.

```html
<input type="text" name="username">
```

## Placeholder

Provides hints to users.

```html
<input
type="text"
placeholder="Enter Username">
```

## Required

Makes a field mandatory.

```html
<input
type="text"
required>
```

## Autofocus

Automatically focuses the input field.

```html
<input
type="text"
autofocus>
```

## Pattern

Validates input using patterns.

```html
<input
type="text"
pattern="[A-Za-z0-9]+">
```

---

# 📦 Inline and Block Elements

## Inline Elements

- Do not start on a new line.
- Take only required width.

Examples:

```html
<span></span>
<a></a>
```

## Block Elements

- Start on a new line.
- Take full width by default.

Examples:

```html
<div></div>
<p></p>
```

> 💡 **Note:** `span` is similar to `div` but is an inline element.

---

# 🆔 ID and Classes

## ID

- Unique identifier.
- Used for only one element.

```html
<div id="firstDiv"></div>
```

## Class

- Can be used on multiple elements.

```html
<div class="red"></div>
```

---

# 🎥 Embedding Videos

```html
<video
src="video.mp4"
controls>
</video>
```

Video Attributes:

- ▶️ Autoplay
- 🔁 Loop
- 🔇 Muted
- 🖼️ Poster

---

# 🎵 Audio Tag

```html
<audio
src="audio.mp3"
controls>
</audio>
```

---

# 🎨 SVG

SVG stands for **Scalable Vector Graphics**.

Used to create scalable graphics without losing quality.

---

# 🖥️ Iframe

Used to embed another webpage.

```html
<iframe
src="URL"
width="500"
height="300">
</iframe>
```

---

# 🔢 Subscript and Superscript

Subscript:

```html
<sub>2</sub>
```

Example: H<sub>2</sub>O

Superscript:

```html
<sup>2</sup>
```

Example: x<sup>2</sup>

---

# 📜 Pre Tag

Displays text exactly as written.

```html
<pre>
This text
will appear
exactly
as written.
</pre>
```

---

# 🏠 Page Layout Tags

```html
<header></header>

<main></main>

<footer></footer>
```

### Header

Contains navigation.

### Main

Main content area.

### Footer

Bottom section of webpage.

### Elements Inside Main

- 📂 `<section>` → Represents a page section.
- 📰 `<article>` → Represents self-contained content.
- 📌 `<aside>` → Represents side content such as advertisements.

---

# 🛠️ Useful Tags

- `<br>` → Line Break
- `<hr>` → Horizontal Line
- `<b>` → Bold
- `<i>` → Italic

---

# 🎉 End of HTML Notes

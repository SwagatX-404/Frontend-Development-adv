# Introduction to Basic HTML Tags

This document provides an overview of fundamental HTML tags for beginners. It covers the basic structure of an HTML document and commonly used tags, with examples to aid understanding.

## 1. Document Structure Tags

These tags form the foundation of an HTML document, defining its structure and metadata.

### 1.1 `<!DOCTYPE html>`
- **Purpose**: Declares the document as HTML5, ensuring browsers render it in standards mode.
- **Usage**: Must be the first line of the HTML file.
- **Example**:
  ```html
  <!DOCTYPE html>
  ```

### 1.2 `<html>`
- **Purpose**: The root element that contains all other HTML elements.
- **Attributes**: `lang="en"` sets the document language (e.g., English for accessibility and SEO).
- **Example**:
  ```html
  <html lang="en">
  </html>
  ```

### 1.3 `<head>`
- **Purpose**: Contains metadata, such as character encoding, viewport settings, and the page title. Content is not visible on the webpage.
- **Example**:
  ```html
  <head>
    <meta charset="UTF-8">
    <title>My Webpage</title>
  </head>
  ```

### 1.4 `<title>`
- **Purpose**: Sets the title of the webpage, displayed in the browser tab, search results, and bookmarks.
- **Example**:
  ```html
  <title>Welcome to My Site</title>
  ```

### 1.5 `<body>`
- **Purpose**: Contains the visible content of the webpage, such as text, images, or links.
- **Example**:
  ```html
  <body>
    Hello, World!
  </body>
  ```

## 2. Content Formatting Tags

These tags structure and format visible content within the `<body>`.

### 2.1 `<h1>` to `<h6>`
- **Purpose**: Define headings, with `<h1>` being the largest/most important and `<h6>` the smallest/least important. Used for organizing content hierarchically.
- **Example**:
  ```html
  <h1>Main Heading</h1>
  <h2>Subheading</h2>
  <h3>Smaller Subheading</h3>
  ```

### 2.2 `<p>`
- **Purpose**: Defines a paragraph of text, adding spacing before and after for readability.
- **Example**:
  ```html
  <p>This is a paragraph of text.</p>
  ```

### 2.3 `<br>`
- **Purpose**: Inserts a single line break within text, without creating a new paragraph.
- **Note**: Self-closing tag (no closing tag needed).
- **Example**:
  ```html
  <p>First line<br>Second line</p>
  ```

### 2.4 `<hr>`
- **Purpose**: Creates a horizontal rule (line) to visually separate content sections.
- **Note**: Self-closing tag.
- **Example**:
  ```html
  <p>Section 1</p>
  <hr>
  <p>Section 2</p>
  ```

## 3. Comments

### 3.1 `<!-- -->`
- **Purpose**: Adds notes or comments in the HTML code that are not displayed on the webpage. Useful for documentation or debugging.
- **Example**:
  ```html
  <!-- This is a comment -->
  <p>Visible text</p>
  ```

## Example: Putting It All Together
Below is a complete HTML document using the tags discussed:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
</head>
<body>
    <h1>Welcome to My Site</h1>
    <h2>About Me</h2>
    <p>This is a paragraph about my site.<br>Here's a new line.</p>
    <!-- Add a separator -->
    <hr>
    <h3>Contact</h3>
    <p>Email me for more info.</p>
</body>
</html>
```

## Key Points to Remember
- **Structure**: Always start with `<!DOCTYPE html>`, followed by `<html>`, `<head>`, and `<body>`.
- **Headings**: Use `<h1>` to `<h6>` for hierarchy, not just for size.
- **Formatting**: Use `<p>` for paragraphs, `<br>` for line breaks, and `<hr>` for section dividers.
- **Comments**: Use `<!-- -->` for non-visible notes to keep code organized.

This document serves as a quick reference for studying basic HTML tags. Practice by creating your own HTML file with these tags!
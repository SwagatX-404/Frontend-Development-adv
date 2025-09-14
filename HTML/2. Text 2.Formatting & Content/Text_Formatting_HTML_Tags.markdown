# Text Formatting and Content Tags in HTML

This document introduces HTML tags for formatting text and presenting specific types of content, such as emphasis, quotations, and code. It is designed for beginners to study and understand these tags with examples.

## 1. Text Formatting Tags

These tags apply visual styling to text, often for emphasis or readability, and some carry semantic meaning.

### 1.1 `<b>`
- **Purpose**: Makes text **bold** for visual emphasis without implying importance.
- **Example**:
  ```html
  <p>This is <b>bold</b> text.</p>
  ```

### 1.2 `<i>`
- **Purpose**: Italicizes text for visual style, often used for technical terms, foreign words, or thoughts.
- **Example**:
  ```html
  <p>The term <i>homo sapiens</i> refers to humans.</p>
  ```

### 1.3 `<u>`
- **Purpose**: Underlines text for visual distinction. Use sparingly, as it may be confused with links.
- **Example**:
  ```html
  <p>This is <u>underlined</u> text.</p>
  ```

### 1.4 `<small>`
- **Purpose**: Displays text in a smaller font size, often for fine print or disclaimers.
- **Example**:
  ```html
  <p>Regular text. <small>Terms and conditions apply.</small></p>
  ```

### 1.5 `<strong>`
- **Purpose**: Makes text **bold** and indicates **semantic importance** (e.g., for accessibility or SEO).
- **Example**:
  ```html
  <p><strong>Warning:</strong> Read instructions carefully.</p>
  ```

### 1.6 `<em>`
- **Purpose**: Italicizes text and indicates **semantic emphasis**, often read differently by screen readers.
- **Example**:
  ```html
  <p>I <em>really</em> mean it!</p>
  ```

### 1.7 `<mark>`
- **Purpose**: Highlights text with a background color (usually yellow) to draw attention.
- **Example**:
  ```html
  <p>Search results: <mark>found</mark> 10 items.</p>
  ```

## 2. Subscript and Superscript Tags

These tags format text for mathematical or scientific notation.

### 2.1 `<sub>`
- **Purpose**: Displays text as a subscript, below the baseline (e.g., for chemical formulas).
- **Example**:
  ```html
  <p>Water is H<sub>2</sub>O.</p>
  ```

### 2.2 `<sup>`
- **Purpose**: Displays text as a superscript, above the baseline (e.g., for exponents or footnotes).
- **Example**:
  ```html
  <p>E = MC<sup>2</sup></p>
  ```

## 3. Quotation and Citation Tags

These tags are used for quoting text or providing citations, often with semantic meaning.

### 3.1 `<q>`
- **Purpose**: Indicates a short inline quotation, typically rendered with quotation marks.
- **Example**:
  ```html
  <p>She said, <q>Live and let live.</q></p>
  ```

### 3.2 `<blockquote>`
- **Purpose**: Represents a longer quotation, often displayed as an indented block.
- **Attributes**: `cite` (optional) specifies the source URL.
- **Example**:
  ```html
  <blockquote cite="https://example.com">
    <p>Not all who wander are lost.</p>
  </blockquote>
  ```

### 3.3 `<abbr>`
- **Purpose**: Defines an abbreviation or acronym, with an optional `title` attribute for the full form.
- **Example**:
  ```html
  <p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
  ```

### 3.4 `<cite>`
- **Purpose**: Indicates a citation or reference to a source, such as a book or article title.
- **Example**:
  ```html
  <p>I read <cite>The Great Gatsby</cite> last week.</p>
  ```

## 4. Code Display Tags

These tags format text related to programming or user input/output.

### 4.1 `<code>`
- **Purpose**: Displays inline code snippets, typically in a monospace font.
- **Example**:
  ```html
  <p>Use the <code>print()</code> function in Python.</p>
  ```

### 4.2 `<pre>`
- **Purpose**: Displays preformatted text, preserving whitespace and line breaks, often for code blocks.
- **Example**:
  ```html
  <pre>
    def hello():
        print("Hello, World!")
  </pre>
  ```

### 4.3 `<kbd>`
- **Purpose**: Represents user input, such as keyboard keys or commands.
- **Example**:
  ```html
  <p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.</p>
  ```

### 4.4 `<samp>`
- **Purpose**: Shows sample output from a program or script.
- **Example**:
  ```html
  <p>The program returned: <samp>Error 404</samp>.</p>
  ```

## Example: Combining Tags
Here’s an example HTML document using these tags:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Text Formatting Demo</title>
</head>
<body>
    <h1>Text Formatting Examples</h1>
    <p>This is <b>bold</b>, <i>italic</i>, and <u>underlined</u> text.</p>
    <p><strong>Important:</strong> Read the <em>instructions</em> carefully.</p>
    <p>Highlight <mark>key terms</mark> in the document.</p>
    <p>Chemical formula: H<sub>2</sub>O, Equation: E = MC<sup>2</sup>.</p>
    <p>She said, <q>Carpe diem!</q></p>
    <blockquote cite="https://example.com">
        <p>Seize the day!</p>
    </blockquote>
    <p>The <abbr title="HyperText Markup Language">HTML</abbr> standard is evolving.</p>
    <p>I enjoyed <cite>1984</cite> by George Orwell.</p>
    <p>Use the <code>console.log()</code> function in JavaScript.</p>
    <pre>
function greet() {
    return "Hello!";
}
    </pre>
    <p>Press <kbd>Enter</kbd> to submit. Output: <samp>Success!</samp></p>
</body>
</html>
```

## Key Points to Remember
- **Formatting**: Use `<b>`, `<i>`, `<u>` for visual styling; prefer `<strong>`, `<em>` for semantic emphasis.
- **Sub/Sup**: Use `<sub>` and `<sup>` for scientific or mathematical notation.
- **Quotations**: Use `<q>` for short quotes, `<blockquote>` for longer ones, `<abbr>` for abbreviations, and `<cite>` for source references.
- **Code**: Use `<code>` for inline code, `<pre>` for code blocks, `<kbd>` for input, and `<samp>` for output.
- Combine tags thoughtfully to enhance readability and accessibility.

This document is a concise reference for studying HTML text formatting and content tags. Practice by creating an HTML file with these examples!
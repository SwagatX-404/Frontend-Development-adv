## Inshort HTML Structure Detailes....

- <!DOCTYPE html>: Declares HTML5 document.
- <html lang="en">: Root element, sets language to English.
- <head>: Contains metadata (not visible on page).

- <meta charset="UTF-8">: Sets character encoding to UTF-8 (supports all characters).
- <meta name="viewport" content="width=device-width, initial-scale=1.0">: Makes page mobile-friendly, no zoom.
- <title>Document</title>: Sets browser tab title to "Document".


- <body>: Visible content; here, displays "This is Web page.".

---
##
## explain its components and their purpose:

# HTML5 Document Structure Guide

## Overview
This document explains the essential components of a basic HTML5 document structure and their purposes.

## Document Structure Components

### 1. `<!DOCTYPE html>`
- **Purpose**: Document Type Declaration (doctype)
- **Position**: Must be the very first line in an HTML document
- **Function**: 
  - Informs web browsers that the document is written in HTML5
  - Ensures the browser renders the page in standards mode
  - Prevents browsers from using "quirks mode" which can cause inconsistent rendering

### 2. `<html lang="en">`
- **Purpose**: Root element of the HTML document
- **Attributes**:
  - `lang="en"`: Specifies the document language as English
- **Benefits**:
  - **Accessibility**: Screen readers use this to select correct language pronunciation
  - **SEO**: Search engines understand the document's language
  - **Styling**: CSS can target language-specific content using `:lang(en)` selectors

### 3. `<head>` Section
- **Purpose**: Contains metadata and non-visible information
- **Content**: Includes elements like `<meta>`, `<title>`, `<link>`, and `<script>`
- **Note**: Content in `<head>` does not appear directly on the webpage

#### 3.1. `<meta charset="UTF-8">`
- **Purpose**: Specifies character encoding
- **Importance**:
  - UTF-8 supports virtually all characters and symbols
  - Prevents text display issues (garbled characters)
  - Should be one of the first tags in `<head>`

#### 3.2. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- **Purpose**: Defines viewport settings for responsive design
- **Parameters**:
  - `width=device-width`: Matches page width to device screen width
  - `initial-scale=1.0`: Sets initial zoom level to 100%
- **Critical** for mobile-friendly websites

#### 3.3. `<title>Document</title>`
- **Purpose**: Defines the webpage title
- **Appears in**:
  - Browser title bar/tab
  - Search engine results
  - Bookmarks/favorites
- **Recommendation**: Use descriptive titles instead of generic "Document"

### 4. `<body>` Section
- **Purpose**: Contains visible webpage content
- **Content**: Everything users see (text, images, interactive elements)
- **Example**: In the basic structure, it contains "This is Web page." text

## Complete HTML5 Structure Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <!-- Visible content goes here -->
    This is Web page.
</body>
</html>
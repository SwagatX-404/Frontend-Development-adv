# Semantic HTML (HTML5)

This README provides a comprehensive guide to HTML5 semantic elements, covering their purpose, usage, and a complete example to demonstrate their application in a structured web page.

## Table of Contents
- [Overview](#overview)
- [Semantic Elements](#semantic-elements)
- [Example](#example)
- [Notes](#notes)

## Overview
Semantic HTML5 elements provide meaning to the structure of a web page, improving accessibility, SEO, and maintainability. Unlike non-semantic elements like `<div>`, semantic elements clearly describe their content's purpose to both browsers and developers.

## Semantic Elements

### Structural Elements
- **`<header>`**: Represents introductory content or a group of navigational links, typically containing headings, logos, or navigation. Often used at the top of a page or section.
  ```html
  <header>
    <h1>Website Title</h1>
    <nav>...</nav>
  </header>
  ```

- **`<nav>`**: Defines a navigation block with links to other pages or sections. Not all links need to be in a `<nav>`, but major navigation should be.
  ```html
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
    </ul>
  </nav>
  ```

- **`<main>`**: Contains the primary content of the page, unique to the document. There should only be one `<main>` per page, and it should not be nested within other semantic elements like `<header>` or `<footer>`.
  ```html
  <main>
    <h2>Main Content</h2>
    <p>This is the core content of the page.</p>
  </main>
  ```

- **`<section>`**: Groups related content with a specific theme or purpose. It should typically contain a heading.
  ```html
  <section>
    <h2>Section Title</h2>
    <p>Content related to this section.</p>
  </section>
  ```

- **`<article>`**: Represents a self-contained piece of content that could stand alone, such as a blog post or news article.
  ```html
  <article>
    <h2>Article Title</h2>
    <p>Independent content goes here.</p>
  </article>
  ```

- **`<aside>`**: Contains content tangentially related to the main content, such as sidebars, callouts, or advertisements.
  ```html
  <aside>
    <h3>Related Links</h3>
    <p>Additional information or ads.</p>
  </aside>
  ```

- **`<footer>`**: Represents the footer of a page or section, typically containing metadata like author info, copyright, or contact details.
  ```html
  <footer>
    <p>&copy; 2025 Website Name</p>
  </footer>
  ```

### Media and Content Elements
- **`<figure>` and `<figcaption>`**: `<figure>` groups media content (e.g., images, diagrams) with an optional `<figcaption>` for a caption.
  ```html
  <figure>
    <img src="image.jpg" alt="Description">
    <figcaption>Caption for the image.</figcaption>
  </figure>
  ```

### Text and Inline Elements
- **`<mark>`**: Highlights text for emphasis or reference, typically rendered with a yellow background.
  ```html
  <p>This is <mark>highlighted</mark> text.</p>
  ```

- **`<time>`**: Represents a specific time or date, with an optional `datetime` attribute for machine-readable formats.
  ```html
  <p>Event on <time datetime="2025-09-21">September 21, 2025</time>.</p>
  ```

### Progress and Measurement Elements
- **`<progress>`**: Displays the progress of a task, with `value` and `max` attributes to indicate completion.
  ```html
  <progress value="70" max="100">70%</progress>
  ```

- **`<meter>`**: Represents a scalar measurement within a known range, with attributes like `min`, `max`, `low`, `high`, and `value`.
  ```html
  <meter min="0" max="100" low="30" high="80" value="60">60%</meter>
  ```

### Interactive Elements
- **`<details>` and `<summary>`**: `<details>` creates a disclosure widget that can be toggled to show or hide content, with `<summary>` defining the visible heading.
  ```html
  <details>
    <summary>More Info</summary>
    <p>Hidden content revealed when clicked.</p>
  </details>
  ```

## Example
Below is a complete HTML5 page demonstrating all the semantic elements listed above, styled for clarity and accessibility.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Semantic HTML5 Example</title>
  <style>
    body { font-family: Arial, sans-serif; max-width: 800px; margin: 20px auto; line-height: 1.6; }
    header { background: #f4f4f4; padding: 20px; text-align: center; }
    nav ul { list-style: none; padding: 0; }
    nav ul li { display: inline; margin-right: 10px; }
    main { padding: 20px; }
    section { margin-bottom: 20px; }
    article { border: 1px solid #ddd; padding: 15px; margin-bottom: 10px; }
    aside { background: #e0f7fa; padding: 15px; margin-bottom: 20px; }
    footer { background: #f4f4f4; padding: 10px; text-align: center; }
    figure { text-align: center; }
    details { margin: 10px 0; }
    mark { background: yellow; }
    progress, meter { width: 200px; }
  </style>
</head>
<body>
  <!-- Header with navigation -->
  <header>
    <h1>Welcome to My Website</h1>
    <nav>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#blog">Blog</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Main content -->
  <main>
    <!-- Section with articles -->
    <section>
      <h2>Latest Posts</h2>
      <article>
        <h3>Blog Post 1</h3>
        <p>This is an <mark>important</mark> post published on <time datetime="2025-09-21">September 21, 2025</time>.</p>
        <figure>
          <img src="https://via.placeholder.com/150" alt="Sample image">
          <figcaption>Sample image caption.</figcaption>
        </figure>
      </article>
      <article>
        <h3>Blog Post 2</h3>
        <p>Another post with a task progress: <progress value="50" max="100">50%</progress></p>
        <p>Performance score: <meter min="0" max="100" low="40" high="80" value="75">75%</meter></p>
      </article>
    </section>

    <!-- Section with interactive details -->
    <section>
      <h2>More Information</h2>
      <details>
        <summary>Click to Learn More</summary>
        <p>This content is hidden until the user clicks the summary.</p>
      </details>
    </section>
  </main>

  <!-- Aside for related content -->
  <aside>
    <h3>Related Links</h3>
    <p>Check out our <a href="#resources">resources</a> for more info.</p>
  </aside>

  <!-- Footer -->
  <footer>
    <p>&copy; <time datetime="2025">2025</time> My Website. All rights reserved.</p>
  </footer>
</body>
</html>
```

## Notes
- **Accessibility**: Semantic elements improve screen reader compatibility. Always include `alt` attributes for `<img>` and `lang` for `<html>`.
- **SEO**: Search engines prioritize semantic markup for better indexing.
- **Styling**: The example includes basic CSS for visual clarity, but you can customize it further.
- **Additional Elements**:
  - `<mark>` is useful for highlighting search terms or key phrases.
  - `<time>` enhances machine-readable date/time data.
  - `<progress>` and `<meter>` are ideal for dynamic applications (e.g., task trackers).
  - `<details>` and `<summary>` reduce JavaScript dependency for toggling content.
- **Best Practices**:
  - Use only one `<main>` per page.
  - Ensure `<section>` and `<article>` have headings for clarity.
  - Nest `<nav>` inside `<header>` or `<footer>` for major navigation blocks.
  - Use `<figure>` for any media with captions, not just images.

This example covers all requested semantic HTML5 elements and provides a practical, accessible implementation. Test it in a browser to see the structure and interactive elements like `<details>` in action.
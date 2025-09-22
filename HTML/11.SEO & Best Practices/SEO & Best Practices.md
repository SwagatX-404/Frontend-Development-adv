# SEO & Best Practices for HTML

This guide introduces key SEO (Search Engine Optimization) and best practices for building modern, optimized HTML websites. It covers `<meta>` tags, Open Graph and Twitter Cards, heading hierarchy, sitemap basics, and Schema markup. Each section includes a brief explanation and a simple code example to get you started.

## Table of Contents
- [Meta Tags (charset, description, keywords, author)](#meta-tags-charset-description-keywords-author)
- [Open Graph & Twitter Cards](#open-graph--twitter-cards)
- [Heading Hierarchy (H1–H6)](#heading-hierarchy-h1h6)
- [Sitemap Basics](#sitemap-basics)
- [Schema Markup (Intro)](#schema-markup-intro)

---

## Meta Tags (charset, description, keywords, author)
Meta tags provide metadata about your HTML document, helping search engines understand your content. Key tags include `charset` for character encoding, `description` for a page summary, `keywords` for relevant terms (less critical today), and `author` for content ownership.

### Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="A beginner-friendly guide to SEO and HTML best practices.">
  <meta name="keywords" content="SEO, HTML, meta tags, web development">
  <meta name="author" content="Your Name">
  <title>SEO Best Practices</title>
</head>
<body>
  <h1>Welcome to My SEO Guide</h1>
  <p>Learn how to optimize your website for search engines.</p>
</body>
</html>
```

**Key Points**:
- `charset="UTF-8"` ensures proper character encoding (place it first in `<head>`).
- `description` should be a concise 150–160 character summary for search engine snippets.
- `keywords` are less important now but can include 3–5 relevant terms.
- `author` credits the content creator (optional).

---

## Open Graph & Twitter Cards
Open Graph (OG) and Twitter Cards are meta tags that control how your content appears when shared on social media platforms like Facebook, LinkedIn, or Twitter. They define the title, description, image, and more.

### Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!-- Open Graph Tags -->
  <meta property="og:title" content="SEO Best Practices Guide">
  <meta property="og:description" content="Learn SEO and HTML best practices for better search rankings.">
  <meta property="og:image" content="https://example.com/images/seo-guide.jpg">
  <meta property="og:url" content="https://example.com/seo-guide">
  <meta property="og:type" content="article">
  <!-- Twitter Card Tags -->
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:title" content="SEO Best Practices Guide">
  <meta name="twitter:description" content="Learn SEO and HTML best practices.">
  <meta name="twitter:image" content="https://example.com/images/seo-guide.jpg">
  <title>SEO Best Practices</title>
</head>
<body>
  <h1>SEO Guide</h1>
  <p>Share this page to see custom social media previews!</p>
</body>
</html>
```

**Key Points**:
- Open Graph tags use `property="og:..."` (e.g., `og:title`, `og:image`).
- Twitter Cards use `name="twitter:..."` (e.g., `twitter:card`, `twitter:image`).
- Use absolute URLs for images and links.
- Test with tools like Facebook’s Sharing Debugger or Twitter’s Card Validator.

---

## Heading Hierarchy (H1–H6)
Headings (`<h1>` to `<h6>`) structure your content for readability and SEO. They signal the importance of content to search engines and improve accessibility.

### Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Heading Hierarchy</title>
</head>
<body>
  <h1>Main Topic: SEO Best Practices</h1>
  <h2>Section 1: Meta Tags</h2>
  <p>Meta tags help search engines understand your content.</p>
  <h3>Subsection: Description Tag</h3>
  <p>Keep it under 160 characters.</p>
  <h2>Section 2: Headings</h2>
  <p>Use headings to organize content logically.</p>
</body>
</html>
```

**Key Points**:
- Use one `<h1>` per page for the main topic.
- Follow with `<h2>`, `<h3>`, etc., in a logical hierarchy (don’t skip levels).
- Include relevant keywords in headings for SEO.
- Ensure headings are descriptive and clear for users and screen readers.

---

## Sitemap Basics
A sitemap is an XML file that lists your website’s URLs, helping search engines crawl and index your content. It’s especially useful for large or dynamic sites.

### Example
**sitemap.xml**
```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://example.com/</loc>
    <lastmod>2025-09-22</lastmod>
    <changefreq>monthly</changefreq>
    <priority>1.0</priority>
  </url>
  <url>
    <loc>https://example.com/about</loc>
    <lastmod>2025-09-22</lastmod>
    <changefreq>yearly</changefreq>
    <priority>0.8</priority>
  </url>
</urlset>
```

**Key Points**:
- Place `sitemap.xml` in your website’s root directory.
- Include key pages with `<loc>`, and optionally `<lastmod>`, `<changefreq>`, and `<priority>`.
- Submit the sitemap to search engines via Google Search Console or Bing Webmaster Tools.
- Use tools like XML-Sitemaps.com for automatic generation on small sites.

---

## Schema Markup (Intro)
Schema markup (structured data) uses JSON-LD (or other formats) to provide search engines with detailed information about your content, enabling rich snippets like star ratings or event details in search results.

### Example
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Schema Markup Example</title>
  <script type="application/ld+json">
  {
    "@context": "https://schema.org",
    "@type": "Article",
    "headline": "SEO Best Practices Guide",
    "author": {
      "@type": "Person",
      "name": "Your Name"
    },
    "datePublished": "2025-09-22",
    "description": "A guide to SEO and HTML best practices."
  }
  </script>
</head>
<body>
  <h1>SEO Guide</h1>
  <p>Learn how to optimize your website with Schema markup.</p>
</body>
</html>
```

**Key Points**:
- Use JSON-LD format with `<script type="application/ld+json">`.
- Common types include `Article`, `Product`, `Event`, or `Organization`.
- Test with Google’s Rich Results Test to ensure proper implementation.
- Explore [Schema.org](https://schema.org/) for available types and properties.

---

## Getting Started
1. Copy
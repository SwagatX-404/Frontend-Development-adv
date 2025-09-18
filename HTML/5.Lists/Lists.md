# 📑 HTML Lists

Lists are used to organize items on a webpage. There are **three main types of lists** in HTML, plus nested lists.

---

## 1️⃣ Ordered List (`<ol>`)
- Displays items in **numbered order**.
- Each item goes inside `<li>`.
- The `type` attribute changes numbering style:
  - `type="1"` → 1, 2, 3 (default)  
  - `type="A"` → A, B, C  
  - `type="a"` → a, b, c  
  - `type="I"` → I, II, III  
  - `type="i"` → i, ii, iii  

```html
<ol type="1">
  <li>One</li>
  <li>Two</li>
</ol>

<ol type="A">
  <li>One</li>
  <li>Two</li>
</ol>

<ol type="i">
  <li>One</li>
  <li>Two</li>
</ol>
```

👉 Output:  
1. One, Two  
A. One, Two  
i. One, Two  

---

## 2️⃣ Unordered List (`<ul>`)
- Displays items with **bullets**.  
- The `type` attribute changes bullet style:
  - `disc` → ● (default)  
  - `circle` → ○  
  - `square` → ■  

```html
<ul type="disc">
  <li>Apple</li>
  <li>Banana</li>
</ul>

<ul type="circle">
  <li>Apple</li>
  <li>Banana</li>
</ul>

<ul type="square">
  <li>Apple</li>
  <li>Banana</li>
</ul>
```

👉 Output:  
● Apple, Banana  
○ Apple, Banana  
■ Apple, Banana  

---

## 3️⃣ Description List (`<dl>`, `<dt>`, `<dd>`)
- Displays **terms and their descriptions**.  
- `<dt>` → term  
- `<dd>` → description  

```html
<dl>
  <dt>HTML</dt>
  <dd>- Markup language for web pages</dd>
  <dt>CSS</dt>
  <dd>- Styles the web page</dd>
</dl>
```

👉 Output:  
**HTML** – Markup language for web pages  
**CSS** – Styles the web page  

---

## 4️⃣ Nested Lists
- A **list inside another list**.  

```html
<ul>
  <li>Frontend
    <ol type="I">
      <li>HTML</li>
      <li>CSS</li>
    </ol>
  </li>
  <li>Backend
    <ul type="square">
      <li>Node.js</li>
      <li>Python</li>
    </ul>
  </li>
</ul>
```

👉 Output:  
- Frontend  
  I. HTML  
  II. CSS  
- Backend  
  ■ Node.js  
  ■ Python  

---

# ✅ Summary
✔ Ordered List `<ol>` → supports number styles (1, A, a, I, i)  
✔ Unordered List `<ul>` → supports bullet styles (disc, circle, square)  
✔ Description List `<dl>` → term + description  
✔ Nested Lists → mix of lists inside lists

# HTML Images & Multimedia

This `README.md` is a study guide for **Images & Multimedia** in HTML.  
It explains the main tags, attributes, and use cases with examples.

---

## 1. `<img>` Tag

The `<img>` tag is used to embed images into a webpage. It is a **self-closing tag**.

### Syntax
```html
<img src="image.jpg" alt="Description" width="300" height="200">
```

### Attributes
- **`src`**: Path to the image file (absolute or relative).  
- **`alt`**: Alternative text (important for accessibility & SEO).  
- **`width` / `height`**: Dimensions of the image (in pixels or %).  

✅ Example:
```html
<img src="cat.png" alt="A cute cat" width="200" height="150">
```

---

## 2. Image Formats

Different image formats are commonly used on the web:

- **JPG / JPEG** → Best for photographs, lossy compression, small file size.  
- **PNG** → Supports transparency, lossless compression, good for graphics & logos.  
- **SVG** → Scalable Vector Graphics, resolution-independent, best for icons/illustrations.  
- **WebP** → Modern format, smaller size, supports both transparency & animations.  

✅ Example:
```html
<img src="logo.svg" alt="Website Logo" width="100">
```

---

## 3. `<audio>` Tag

The `<audio>` tag is used to embed sound content like music or recordings.

### Common Attributes
- **`controls`**: Displays play/pause/volume controls.  
- **`autoplay`**: Plays automatically (not recommended for UX).  
- **`loop`**: Repeats the audio when finished.  

✅ Example:
```html
<audio controls loop>
  <source src="song.mp3" type="audio/mpeg">
  <source src="song.ogg" type="audio/ogg">
  Your browser does not support the audio tag.
</audio>
```

---

## 4. `<video>` Tag

The `<video>` tag is used to embed video content.

### Common Attributes
- **`controls`**: Adds play/pause/volume/fullscreen controls.  
- **`autoplay`**: Plays automatically (muted is usually required).  
- **`loop`**: Replays video continuously.  
- **`poster`**: Defines an image thumbnail shown before playback.  

✅ Example:
```html
<video width="400" controls poster="thumbnail.jpg">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
```

---

## 5. Embedding YouTube (using `<iframe>`)

The `<iframe>` tag is used to embed external media like YouTube videos.

✅ Example:
```html
<iframe width="560" height="315" 
  src="https://www.youtube.com/embed/dQw4w9WgXcQ" 
  title="YouTube video player" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>
```

---

## 📌 Quick Summary

- `<img>` embeds images (`src`, `alt`, `width`, `height`).  
- Image formats: **JPG, PNG, SVG, WebP** (use based on purpose).  
- `<audio>` supports music/recordings with `controls`, `autoplay`, `loop`.  
- `<video>` supports video playback with `controls`, `poster`, `captions`.  
- `<iframe>` is used to embed external media like YouTube videos.  

---

## 📝 Practice Exercise

1. Add an **image** with `alt` text and set its size.  
2. Insert an **audio file** with `controls` and `loop`.  
3. Insert a **video** with `poster` and `controls`.  
4. Embed a **YouTube video** using `<iframe>`.  

This will give hands-on practice with **Images & Multimedia** in HTML.

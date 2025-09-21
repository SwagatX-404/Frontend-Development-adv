
# HTML5 APIs & Advanced Features

This document covers the major HTML5 APIs and advanced features with explanations and code examples.

---

## 🌍 1. Geolocation API
- Allows websites to get the user’s current location (with permission).
- Methods:
  - `navigator.geolocation.getCurrentPosition(successCallback, errorCallback)`
  - `navigator.geolocation.watchPosition(successCallback, errorCallback)`

**Example:**
```html
<button onclick="getLocation()">Get My Location</button>
<p id="demo"></p>

<script>
function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(showPosition, showError);
  } else {
    document.getElementById("demo").innerHTML = "Geolocation not supported.";
  }
}

function showPosition(position) {
  document.getElementById("demo").innerHTML =
    "Latitude: " + position.coords.latitude +
    "<br>Longitude: " + position.coords.longitude;
}

function showError(error) {
  document.getElementById("demo").innerHTML = error.message;
}
</script>
```

---

## 🖱️ 2. Drag & Drop API
- Lets users drag elements and drop them into others.
- Uses `draggable="true"`, and JS events (`ondragstart`, `ondrop`, `ondragover`).

**Example:**
```html
<div id="div1" 
     ondrop="drop(event)" 
     ondragover="allowDrop(event)" 
     style="width:200px;height:200px;border:1px solid black;">
</div>

<img id="drag1" src="https://via.placeholder.com/100" draggable="true" ondragstart="drag(event)">

<script>
function allowDrop(ev) {
  ev.preventDefault();
}

function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}

function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  ev.target.appendChild(document.getElementById(data));
}
</script>
```

---

## 💾 3. Web Storage (localStorage & sessionStorage)
- Store data in the browser.
  - **localStorage** → persists after browser closes.
  - **sessionStorage** → cleared when tab/window closes.

**Example:**
```html
<button onclick="saveData()">Save Data</button>
<button onclick="getData()">Get Data</button>
<p id="output"></p>

<script>
function saveData() {
  localStorage.setItem("username", "Swagat");
}

function getData() {
  let user = localStorage.getItem("username");
  document.getElementById("output").innerText = "Hello " + user;
}
</script>
```

---

## ⚡ 4. Web Workers (Intro)
- Run background tasks without blocking UI.
- Useful for heavy calculations.

**Example:**
```html
<!-- index.html -->
<button onclick="startWorker()">Start Worker</button>
<p id="result"></p>

<script>
let worker;

function startWorker() {
  if (window.Worker) {
    worker = new Worker("worker.js");
    worker.onmessage = function(e) {
      document.getElementById("result").innerHTML = e.data;
    };
  }
}
</script>
```

```js
// worker.js
let i = 0;
function timedCount() {
  i++;
  postMessage(i);
  setTimeout(timedCount, 1000);
}
timedCount();
```

---

## 🎨 5. Canvas API (`<canvas>`)
- Draw graphics, charts, animations dynamically with JavaScript.

**Example:**
```html
<canvas id="myCanvas" width="300" height="200" style="border:1px solid black;"></canvas>

<script>
let c = document.getElementById("myCanvas");
let ctx = c.getContext("2d");

ctx.fillStyle = "blue";
ctx.fillRect(20, 20, 150, 100);

ctx.beginPath();
ctx.arc(200, 100, 40, 0, 2 * Math.PI);
ctx.stroke();
</script>
```

---

## 🖼️ 6. SVG in HTML
- Scalable Vector Graphics (vector-based, don’t lose quality on zoom).
- Can be styled with CSS & manipulated with JS.

**Example:**
```html
<svg width="200" height="200">
  <circle cx="100" cy="100" r="80" stroke="blue" stroke-width="4" fill="lightblue" />
</svg>
```

---

## 🎵🎥 7. Audio & Video API (Custom Controls)
- `<audio>` & `<video>` tags introduced in HTML5.
- Can build custom controls with JavaScript.

**Example:**
```html
<video id="myVideo" width="320" height="240">
  <source src="sample.mp4" type="video/mp4">
</video>
<br>
<button onclick="playVideo()">Play</button>
<button onclick="pauseVideo()">Pause</button>

<script>
let video = document.getElementById("myVideo");
function playVideo() { video.play(); }
function pauseVideo() { video.pause(); }
</script>
```

---

# ✅ Summary
- **Geolocation** → get user’s location.  
- **Drag & Drop** → move elements interactively.  
- **Web Storage** → save data (`localStorage`, `sessionStorage`).  
- **Web Workers** → run background tasks.  
- **Canvas** → draw graphics dynamically.  
- **SVG** → scalable vector graphics.  
- **Audio/Video API** → custom media controls.

# OpenTrack Racer 🏎️

OpenTrack Racer is a browser-based pseudo-3D racing game built using **HTML5 Canvas**, **CSS**, and **Vanilla JavaScript**. The project simulates a classic arcade racing experience with dynamic road generation, AI-controlled traffic, perspective projection, and real-time rendering.

---

## 🎮 Features

* Pseudo-3D road rendering
* Dynamic curves, hills, and road generation
* AI-controlled traffic cars
* Collision detection system
* Real-time speed and lap timer HUD
* Adjustable graphics and gameplay settings
* Smooth animations using `requestAnimationFrame`
* Browser-based — no installation required

---

## 🛠️ Technologies Used

* **HTML5 Canvas**
* **JavaScript (Vanilla JS)**
* **CSS3**
* Browser APIs:

  * `requestAnimationFrame`
  * `localStorage`
  * Keyboard Event Listeners

---

## 📂 Project Structure

```bash
├── index.html
├── style.css
├── game.js
├── images/
│   ├── cars.png
│   ├── sprites.png
│   └── background.png
└── README.md
```

---

## 🚗 How the Game Works

The game uses a **pseudo-3D projection system** to simulate depth and perspective on a 2D canvas.

### Core Concepts

* World coordinates are transformed into camera coordinates.
* Objects are projected from 3D space to 2D screen space.
* Road segments are dynamically rendered based on distance and perspective.

### Main Systems

* Projection Engine
* Road Generation
* Car AI
* Collision Detection
* HUD & Lap Timing
* Animation Loop

---

## 📌 Important Functions

### `project()`

Converts 3D world coordinates into 2D screen coordinates.

```javascript
p.screen.scale = cameraDepth / p.camera.z;
```

Used to create the pseudo-3D effect.

---

### `overlap()`

Checks collisions between cars and objects.

```javascript
return !((max1 < min2) || (min1 > max2));
```

---

### `increase()`

Handles looping positions along the track.

```javascript
result += increment;
```

---

## 🎨 Graphics Techniques Used

* Perspective Projection
* Camera Transformations
* Distance-based Fog
* Sprite Scaling
* Smooth Animation & Easing

---

## 🎮 Controls

| Key            | Action     |
| -------------- | ---------- |
| ⬆️ Up Arrow    | Accelerate |
| ⬇️ Down Arrow  | Brake      |
| ⬅️ Left Arrow  | Move Left  |
| ➡️ Right Arrow | Move Right |

---

## ▶️ How to Run

1. Download or clone the repository.
2. Open `index.html` in any modern browser.
3. Start racing!

No installation or external dependencies required.

---

## 📷 Screenshots

Add screenshots of:

* Gameplay
* HUD
* Curves & Hills
* Settings Menu

---

## 🚀 Future Improvements

* Add sound effects and music
* Multiplayer support
* More tracks and environments
* Improved AI behavior
* Mobile controls support

---

## 👨‍💻 Author
Ahmed Ashraf (TL)
Rawan Hossam 
Ahmed Haytham

Developed as a graphics/game development project using JavaScript and HTML5 Canvas.

<img src="KinematicsJS.png">

KinematicsJS is a high-performance 2D physics engine built completely from scratch using vanilla JavaScript and HTML5 Canvas[cite: 1, 2, 5]. It uses a custom **Spatial Hash Grid (v4)** to handle ultra-fast collision lookups without lagging, keeping the simulation buttery smooth on everything from older smartphones to 240Hz gaming monitors[cite: 1, 5].

I built this project to simulate real-world vector mechanics, material limits, and fluid drag dynamics directly inside a web browser—no heavy frameworks or installations required[cite: 1, 2, 5].

---

## ✨ Key Features

* **High-Performance Collisions:** Uses a Spatial Hash Grid to quickly look up nearby objects. Instead of checking every single shape against each other ($O(n^2)$ complexity), it only checks objects sharing the same grid cells.
* **FEA Stress & Heatmaps:** Objects don't just bounce off each other[cite: 1]. They accumulate structural stress when they collide with high forces[cite: 1]. The engine dynamically applies a color gradient (heatmap) to show exactly where the impact load is highest before it cools down[cite: 1].
* **CAD Custom Polygon Pen:** A built-in geometry tool that lets you click directly on the screen to draw custom shapes. The engine mathematically handles the center of gravity (area centroid) calculations and bakes them instantly into moving physical meshes[cite: 1].
* **Real-Time Thermodynamics Tracking:** Driven by a live Chart.js dashboard that plots Kinetic Energy (KE), Potential Energy (PE), Fluid/Air Drag Losses, and Net Total Energy conservation to prove the physics engine respects the laws of thermodynamics.
* **Materials & Environments:** Swap material matrices on the fly (Structural Steel, Concrete, Aluminum) to alter density and elasticity coefficients, or toggle environmental mediums (Vacuum, Air, Hydraulic Fluid) to introduce different viscosity drag variables[cite: 1, 2, 5].
* **Blueprint Light Mode:** A quick UI toggle instantly shifts the workspace from a high-tech dark mode lab matrix into a clean, physical engineering blueprint schematic style[cite: 1, 2, 3].

---

## 📁 Project Structure

* `app.js` — Core multi-physics engine vector math, spatial grid register, and Chart.js telemetry logic.
* `index.html` — The structural layout, interactive sidebar control menus, and cinematic entry screen.
* `style.css` — Responsiveness layout rules, customized input sliders, and dual light/dark theme variables[cite: 2, 3].

---

## 🛠️ Tech Stack

* **Core Logic:** Vanilla JavaScript (ES6+), HTML5 Canvas (Hardware Accelerated context)[cite: 1, 2, 5]
* **Data Visualization:** Chart.js (v4+)[cite: 2, 5]
* **Typography & Styling:** CSS3, Plus Jakarta Sans & JetBrains Mono via Google Fonts[cite: 2, 3]

---

## ⚙️ Quick Start

Because this project is built entirely on native web standards, you don't need a single `npm install` or heavy build toolchain to run it[cite: 2, 5].

1. **Clone the Repository:**
```bash
   git clone [https://github.com/your-username/kinematicsjs.git](https://github.com/your-username/kinematicsjs.git)
   cd kinematicsjs

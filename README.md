# 🌈 Colourfull Wave

> A mesmerizing full-screen animated wave visualizer built with **HTML5 Canvas**, **CSS**, and **JavaScript**.

**Colourfull Wave** creates a smooth, continuously moving rainbow wave across the screen using mathematical sine-wave animation and dynamic HSL colors. The project is lightweight, responsive, and requires no external libraries or frameworks.

---

## ✨ Features

* 🌈 Dynamic rainbow-colored wave
* 🌊 Smooth sine-wave animation
* 🎨 Continuously changing HSL colors
* 🖥️ Full-screen canvas experience
* 📱 Responsive to different screen sizes
* 👆 Touch interaction support
* ⚡ Lightweight and dependency-free
* 🔄 Real-time animation using `requestAnimationFrame`
* 🖤 Minimal black background
* 🎯 Simple single-file implementation

---

## 🖥️ Tech Stack

* HTML5
* CSS3
* JavaScript
* HTML5 Canvas API
* HSL Color System
* `requestAnimationFrame`

---

## 🚀 Live Project

View the source code and project on GitHub:

[Colourfull Wave — GitHub Repository](https://github.com/rsamwilson2323-cloud/Colourfull-wave?utm_source=chatgpt.com)

---

## 📦 Installation

No installation or external dependencies are required.

### Clone the repository

```bash
git clone https://github.com/rsamwilson2323-cloud/Colourfull-wave.git
```

### Go into the project

```bash
cd Colourfull-wave
```

### Open the project

Simply open:

```text
Colourfull wave.html
```

in any modern web browser.

You can also double-click the HTML file directly.

---

# 🎨 How It Works

The project uses the **HTML5 Canvas API** to draw and animate a mathematical sine wave.

The animation continuously calculates the vertical position of each point using a sine function:

```javascript
y = Math.sin(x * waveLength + t) * amplitude + mid;
```

The wave moves continuously as the animation time value increases.

```javascript
t += speed;
```

The animation is rendered repeatedly using:

```javascript
requestAnimationFrame(animate);
```

This creates a smooth and fluid visual effect.

---

# 🌈 Dynamic Colors

Each section of the wave receives a different HSL color.

```javascript
ctx.strokeStyle = `hsl(${(x/4 + t*20) % 360},100%,60%)`;
```

As the wave moves, the hue continuously changes across the full color spectrum, producing the animated rainbow effect.

---

# 🌊 Wave Animation

The wave is generated using a sine function with configurable properties:

| Property        | Value  |
| --------------- | ------ |
| Wave Length     | `0.02` |
| Base Amplitude  | `80`   |
| Animation Speed | `0.05` |
| Line Width      | `6px`  |
| Background      | Black  |

The wave is positioned around the vertical center of the screen.

---

# 📱 Responsive Canvas

The canvas automatically adapts to the browser window.

```javascript
function resize(){
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
}
```

The resize function is called whenever the browser window changes size.

```javascript
window.onresize = resize;
```

This allows the animation to work across different screen sizes.

---

# 👆 Touch Interaction

The project also includes a simple touch interaction.

When the screen is touched, the wave amplitude increases:

```javascript
document.addEventListener("touchstart", () => touchBoost = 25);
```

When the touch ends, the additional amplitude is removed:

```javascript
document.addEventListener("touchend", () => touchBoost = 0);
```

This creates a small interactive effect on touch-enabled devices.

---

# 🖥️ User Experience

The project intentionally uses a minimal interface.

There are:

* No buttons
* No menus
* No external controls
* No configuration panels

The entire browser viewport becomes the animated canvas.

This makes **Colourfull Wave** suitable as a visual background, creative coding experiment, screensaver-style animation, or interactive web-art project.

---

# 📁 Project Structure

```text
Colourfull-wave/
│
├── Colourfull wave.html
├── README.md
└── LICENSE
```

The main application is contained entirely inside:

```text
Colourfull wave.html
```

The HTML file contains:

* HTML structure
* CSS styling
* Canvas element
* JavaScript animation
* Touch interaction
* Responsive resizing

---

# 🎯 Use Cases

Colourfull Wave can be used for:

* 🌈 Creative coding experiments
* 🎨 Generative art
* 🖥️ Animated website backgrounds
* 🌊 Visual effects
* 📱 Interactive mobile experiments
* 🎬 Background animations
* 🧪 JavaScript Canvas learning
* 📚 Educational demonstrations
* 💻 Frontend portfolio projects
* 🖼️ Digital art experiments

---

# ⚡ Performance

The animation uses the browser's native:

```javascript
requestAnimationFrame()
```

This allows the browser to synchronize rendering with the display refresh rate and provides a smooth animation experience.

The project also uses a semi-transparent black fill:

```javascript
ctx.fillStyle = "rgba(0,0,0,0.15)";
```

instead of completely clearing the canvas. This creates the visual fading/trailing effect behind the moving wave.

---

# 🧠 Concepts Demonstrated

This project is a simple example of several important web-development concepts:

* HTML Canvas
* JavaScript animation
* Mathematical sine waves
* Dynamic colors
* HSL color generation
* Browser rendering
* Animation loops
* Responsive layouts
* Touch events
* Real-time graphics

---

# 🔮 Future Improvements

Possible improvements for future versions include:

* 🎚️ Interactive amplitude controls
* 🎨 Color palette selector
* 🌈 Multiple wave layers
* 🌀 Circular wave modes
* 💫 Particle effects
* 🖱️ Mouse interaction
* 👆 Improved touch gestures
* 🎛️ Speed controls
* 🌊 Adjustable wave frequency
* 📸 Screenshot/export feature
* 🎵 Audio-reactive waves
* 🌌 Background gradient effects
* 📱 Enhanced mobile interactions
* 🎨 Custom color themes
* 🖥️ Fullscreen toggle

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature/amazing-feature
```

3. Make your changes
4. Commit your changes

```bash
git commit -m "Add amazing feature"
```

5. Push your branch

```bash
git push origin feature/amazing-feature
```

6. Open a Pull Request

---

# 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for more information.

---

# ⭐ Show Your Support

If you like **Colourfull Wave**:

⭐ Star the repository

🍴 Fork the project

🐞 Report bugs

💡 Suggest new features

🚀 Build something creative with it

---

## 👨‍💻 Author

**Sam Wilson**

AI & Full Stack Developer

Interested in:

* 🤖 Artificial Intelligence
* 🧠 Machine Learning
* 👁️ Computer Vision
* 🌐 Web Development
* 🎨 UI/UX Design
* 🧊 3D Web Graphics
* 💻 Creative Coding

---

## 🌈 Made with

**HTML + CSS + JavaScript + Canvas API**

Made with ❤️ and a little bit of mathematics.

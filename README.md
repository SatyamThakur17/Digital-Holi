# 🌈 Holi for Google Meet – Chrome Extension  

Play Holi digitally on Google Meet — because distance shouldn’t cancel color.

This Chrome Extension lets you spray physics-based gulal on top of a live Google Meet call without interrupting the session. Built as a Manifest V3 extension with a real-time Canvas particle engine.

---

## ✨ What It Does

This extension injects a high-z-index overlay into Google Meet and renders a real-time particle system using HTML5 Canvas. You can spray color, trigger bursts, switch shades, and toggle the effect — all without dropping the call.

It works by attaching the rendering layer to `document.documentElement` (not `document.body`) to bypass Google Meet’s stacking context issues and ensure the overlay appears above everything.

---

## 🎨 Features

- 8 traditional Holi colors (Gulal Red, Panna Green, Kesari Orange & more)  
- Physics-based particle engine (gravity, velocity, decay, alpha blending)  
- Spray mode for fine mist dispersion  
- Welcome burst animation on activation  
- Custom cursor matching selected color  
- Keyboard shortcuts:  
  - `1–8` → Switch colors  
  - `S` → Toggle spray mode  
  - `C` → Clear screen  
  - `Esc` → Exit / Toggle off  
- On/off toggle without disconnecting Google Meet  
- Works as a Manifest V3 Chrome extension  

---

## 🛠 Tech Stack

- Chrome Extension (Manifest V3)
- Content Scripts
- HTML5 Canvas API
- Vanilla JavaScript
- Custom particle physics engine
- CSP-compliant script structure

---

## ⚙️ Technical Highlights

- Solved Chrome CSP inline-script violations by restructuring script injection  
- Handled Google Meet’s aggressive z-index stacking  
- Attached overlay to `document.documentElement` for guaranteed top rendering  
- Optimized animation loop for smooth real-time rendering  
- Built modular particle system with velocity vectors and gravity simulation  

---

## 🚀 Installation (Manual)

1. Clone this repository:

   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

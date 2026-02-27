# Day 6: Interactive Custom Cursor 🖱️

Part of my **30-Day Series 6 Challenge**. Today’s project focuses on custom UI pointers and advanced CSS background blending.

## 🛠 Project Overview
A dual-element cursor that follows the user's mouse in real-time. It consists of a large multi-colored outer ring and a solid inner core, providing a modern, high-end feel to any landing page.

## ✨ Key Features
- **Dynamic Tracking:** Smooth XY coordinate mapping using Vanilla JS.
- **Visual Depth:** Triple-linear gradients combined with `background-blend-mode: multiply`.
- **Performance:** Lightweight code with minimal reflow.

## 🔗 Demo
[Click here to see it in action!](https://nimble-twilight-d8ae1f.netlify.app/)

## 📝 Quick Snippet: The Logic
```javascript
document.addEventListener("mousemove", (e) => {
  // Syncing both cursor layers to the mouse coordinates
  cursor1.style.cssText = cursor2.style.cssText =
    "left:" + e.clientX + "px; top: " + e.clientY + "px";
});

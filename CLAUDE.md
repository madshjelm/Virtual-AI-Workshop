# Project Overview
This is a 3D interactive web experience hosted on GitHub Pages.
The live URL is: https://madshjelm.github.io/Virtual-AI-Workshop/

# Architecture & Environment
- **Important Context:** This game is embedded directly into a WordPress website via the following full-screen `<iframe>`:
  ```html
  <iframe 
    src="[https://madshjelm.github.io/Virtual-AI-Workshop/](https://madshjelm.github.io/Virtual-AI-Workshop/)" 
    style="position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; border: none; margin: 0; padding: 0; z-index: 9999;" 
    allow="autoplay">
  </iframe>
- **Tech Stack:** Vanilla HTML, CSS, JavaScript, and Three.js.
- **Styling:** The canvas must always remain 100vw and 100vh with `margin: 0` and `overflow: hidden` to prevent scrollbars in the WordPress iframe.

# Current Focus: Spatial Audio
The user is a musician focusing on interactive sound design. We are using the Web Audio API and Three.js `PositionalAudio`.

# Coding Guidelines
- Keep code clean and well-commented.
- If introducing new Three.js concepts, briefly explain the math or logic being used.
- Prioritize performance (avoiding memory leaks) so the WordPress site hosting the iframe does not freeze or drop FPS.

# Shifra - Browser‑Based Virtual Assistant

A voice‑activated assistant for the web using the **Web Speech API** to recognize your commands and speak responses. Click the mic button, talk naturally, and let Shifra open sites, tell the time/date, or search the web.

---

## Features
- Voice input via `SpeechRecognition` and spoken replies via `SpeechSynthesis` (no backend needed)
- Quick actions: open YouTube, Google, Facebook, Instagram
- Information: current **time** and **date**
- Fallback: hands‑free web search for other queries
- Simple, responsive UI with a glowing mic button and animated voice GIF

---

## Tech Stack
- **HTML5** (`index.html`)
- **CSS3** (`style.css`)
- **Vanilla JavaScript** (`script.js`)
- **Web Speech API** (browser feature)

---

## Getting Started
1. Clone or download this folder.
2. Open `index.html` in a modern browser (Chrome recommended).
   - For reliable mic access, serve over **HTTPS** or **localhost** (e.g., VS Code **Live Server**).
3. When prompted, **allow microphone** permission.

> Quick local server options
> - VS Code extension: *Live Server*
> - Node: `npx serve .`
> - Python: `python -m http.server 5500`

---

## Usage
1. Click the **microphone** button.
2. Speak a command, for example:
   - "hello" / "who are you"
   - "open youtube" / "open google" / "open facebook" / "open instagram"
   - "time" or "date"
3. If the command isn’t recognized, Shifra will open a web search.

---

## Project Structure
```
.
├─ index.html        # Page layout, assets, and button hook
├─ style.css         # Styles and button/glow effects
├─ script.js         # Speech recognition, TTS, and command handling
├─ logo.jpg          # App icon/logo
├─ mic.svg           # Mic icon in the button
└─ voice.gif         # Animated voice indicator
```

---

## Customization
- **Assistant name**: Edit the `#name` span in `index.html`.
- **Greetings/phrases**: Adjust text in `wishMe()` and `speak()` calls in `script.js`.
- **Commands**: Extend the `takeCommand()` function with new `if/else` branches.
- **Look & feel**: Tweak colors, sizes, and effects in `style.css`.

---

## Notes & Browser Support
- The Web Speech API works best in **Chrome**. Some browsers require a **secure context** (HTTPS or localhost) for the mic.
- Custom URL schemes like `calculator://` or `whatsapp://` may not be supported on all platforms.

---

## License
See `LICENSE` for terms.


Standalone Music Player

This folder contains a static standalone player that runs without installing `node_modules`.

Files:
- index.html — stand-alone entry that loads React via CDN and mounts the player.
- MusicPlayer.css — existing styles used by the standalone page.
- MusicPlayer.jsx — original React source (for reference).

How to run:

Option A — quick (recommended): start a minimal static server and open in browser

```bash
# from this folder
python3 -m http.server 8000
# then open http://localhost:8000/index.html in your browser
```

Option B — open file directly

- Open `index.html` in your browser. (Some browsers may restrict local file access; use the server if media fails to load.)

Notes:
- The standalone page uses CDN React + Babel to transpile JSX in the browser — no build step required.
- Local audio/image files referenced (Borderline.mp3, Twilight.mp3, borderline.webp, Twilight.jpeg) are used as-is and must remain in this folder.

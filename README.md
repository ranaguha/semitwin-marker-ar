
# SemiTwin — Marker-based AR Frontend (A-Frame + AR.js)

This is a **Web AR** version that works on many phones even if **WebXR is not supported**.
It uses **A-Frame + AR.js** with the classic **HIRO marker**, and consumes live data from the same Socket.IO backend.

## Quick Start

1) **Deploy the backend** somewhere with **HTTPS** (Render/Railway).
   - Use your existing `semitwin/backend`:
   - On Render: Build `npm install`, Start `npm start`
   - After deploy, you'll get `https://<your-backend>.onrender.com`

2) **Configure the frontend**
   - Edit `config.js` and set:
     ```js
     window.BACKEND_URL = "https://<your-backend>.onrender.com";
     ```

3) **Host this folder (marker-ar-frontend) as static files**
   - Easiest: GitHub Pages
     - Create a repo, add these files, push, and enable **Pages**.
     - Your site will be at `https://<you>.github.io/<repo>/` (HTTPS ✅).

4) **Open on your phone**
   - Print the HIRO marker: https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/hiro.png
   - Visit your GitHub Pages URL.
   - Allow camera permission.
   - Point the camera at the marker. The 6 boxes (machines) appear on top of it and **update colors** live.

SPIRIT GUIDE APP — ZIP PACKAGE
================================

Files included:
  • index.html                     — The app (deterministic selection + localStorage)
  • style.css                      — Neon green on black styling
  • backstories_full_fixed.json    — 12 guides, each with a long backstory, keywords, and metadata
  • README.txt                     — This file

HOW IT WORKS
------------
• Deterministic selection:
  The app hashes YOUR NAME + BIRTH DATE (YYYY-MM-DD) with a DJB2-style hash and combines it
  with your numerology Life Path number (with 11/22/33 treated as master numbers). The result
  maps to a guide index. Same inputs → same guide every time.

• localStorage:
  Your result is saved privately in your browser (key: "spiritGuideResult_v2"). Use the Reset
  button to clear it and run the app again.

• Backstories:
  The app loads "backstories_full_fixed.json" by default. If you open the app directly via
  "file://", some browsers block fetches; in that case you'll see a tiny inline fallback with
  2 sample guides. For the full set, serve the files locally or deploy them (see below).


RUN LOCALLY (no internet needed)
--------------------------------
Option A) Quick Python server (any OS)
  1. Open a terminal in this folder.
  2. Run:  python -m http.server 8080
  3. Visit: http://localhost:8080  (then click index.html)

Option B) Node "serve"
  1. npm i -g serve
  2. serve .
  3. Open the shown localhost URL.

DEPLOY (Netlify / GitHub Pages / any static host)
-------------------------------------------------
• Netlify (drag‑and‑drop):
  1. Go to https://app.netlify.com/drop
  2. Drag the whole folder (or just upload this ZIP and unzip on Netlify) — Netlify will host it.
  3. Open the URL Netlify gives you. Everything will work immediately.

• GitHub Pages:
  1. Create a new repo and upload all the files.
  2. Enable GitHub Pages in repo settings (root or /docs).
  3. Visit the Pages URL it provides.

CUSTOMISING
-----------
• Add/modify guides in backstories_full_fixed.json. Keep structure:
  {
    "guides":[
      {
        "id":"unique-slug",
        "name":"Name",
        "element":"Element",
        "domains":["A","B","C"],
        "keywords":["x","y","z"],
        "sigil":"optional symbol",
        "color":"#hex",
        "mantra":"Optional mantra sentence",
        "backstory":"~300–400 words of lore."
      }
    ]
  }

• You can safely change colours and glow in style.css.

ACCESSIBILITY & OFFLINE
-----------------------
• No analytics. No network requests beyond loading the local JSON.
• Works offline once loaded on a static host.
• Keyboard friendly. Copy summary button to capture output quickly.

CREDITS
-------
• © 2025 7 Tarot. You are free to use, modify, and deploy for your project.

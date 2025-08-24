SPIRIT GUIDE APP — NUMEROLOGY EDITION (v2)
===========================================

This build adds a full numerology chart + text-to-speech narration.

FILES
-----
• index.html                   — App logic (deterministic selection using full numerology)
• style.css                    — Neon green on black styling
• backstories_full_fixed.json  — 12 guides with ~400-word backstories
• README.txt                   — This file

WHAT'S NEW VS v1
----------------
• Calculates and displays:
  - Life Path (from date of birth)
  - Destiny/Expression (from full name)
  - Soul Urge / Heart's Desire (vowels of name)
  - Personality (consonants of name)
  - Birthday Number (day of month)
  - Maturity / Realization (Life Path + Expression)
  - Karmic Debts (13/4, 14/5, 16/7, 19/1) when present
  - Karmic Lessons (missing name numbers 1–9)
• Deterministic guide mapping now blends all of the above for a richer, stable result.
• Built‑in narration (Web Speech API) reads the backstory + numerology summary aloud.
• localStorage caches the full result so users return to the same guide and chart.

RUN LOCALLY
-----------
Option A) Python
  python -m http.server 8080
  → Open http://localhost:8080/

Option B) Netlify Drop (zero config)
  https://app.netlify.com/drop  → drag the folder in.

GITHUB PAGES
------------
1) Create a repo and upload all four files at the root.
2) Settings → Pages → Deploy from branch → branch: main, folder: / (root).
3) Open the Pages URL.

NOTES
-----
• Y-as-vowel is handled with a sensible heuristic (between consonants counts as vowel).
• Master numbers 11/22/33 are preserved in reduction when relevant.
• Speech synthesis uses the browser’s voices (prefers en‑GB if available).

© 2025 7 Tarot — free to use and modify.

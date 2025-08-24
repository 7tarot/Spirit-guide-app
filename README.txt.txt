SPIRIT GUIDE APP — NUMEROLOGY EDITION (v2.5)

Features
- Deterministic guide selection (name normalized + DOB + full chart)
- Full numerology chart: Life Path, Expression, Soul Urge, Personality, Birthday, Maturity
- Karmic Debts (13/14/16/19) + Karmic Lessons (missing name numbers with meanings)
- Compatibility (good/challenging), Tarot & zodiac mapping (Majors reduced to 1–9; Sun=19→1)
- Connections presets (Classic vs Steve’s House); Personal Year timeline with color highlights
- Pinnacles & Challenges (4 each), Hidden Passion, Balance number
- Lucky Days calendar (Personal Days)
- Narration with voice + mood; optional ambient soundscapes (stubs to swap later)
- Save as PDF (print stylesheet) + Shareable Mystic Card (PNG)
- Works offline; data stays in localStorage

Quick Start
1) Put index.html, style.css, backstories_full_fixed.json, README.txt in one folder.
2) Double-click index.html to preview OR run a local server:
   python -m http.server 8080  → http://localhost:8080/

Deploy — GitHub Pages
1) New repo → upload all four files at the root
2) Settings → Pages → Source: Deploy from branch (main), root
3) Wait for the green check → your site URL appears

Deploy — Netlify Drop
1) https://app.netlify.com/drop
2) Drag your folder in → get instant URL

Editing Guides
- Replace backstories_full_fixed.json with your full “guides” array (400-word backstories)
- Keep fields: id, name, element, domains[], backstory, mantra, keywords[], sigil

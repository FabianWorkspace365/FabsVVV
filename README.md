# 🌴 Vakantie Ommen 2025 — PWA

Retro vakantie-app voor de zomervakantie op Camping Ommerland, Ommen.

## Bestanden

```
vakantie-app/
├── index.html        ← De complete app
├── manifest.json     ← PWA manifest (installeerbaar op Android)
├── sw.js             ← Service Worker (offline werking)
├── icons/
│   ├── icon-192.svg  ← App-icoon (klein)
│   └── icon-512.svg  ← App-icoon (groot)
└── README.md
```

## Installeren op je Android telefoon (PWA)

### Via GitHub Pages (aanbevolen)

1. Maak een gratis GitHub account via github.com
2. Maak een nieuw repository aan: `vakantie-ommen`
3. Upload alle bestanden (drag & drop in de GitHub interface)
4. Ga naar **Settings → Pages → Branch: main → Save**
5. Je app is nu live op: `https://[jouwusername].github.io/vakantie-ommen`
6. Open die URL op je Android telefoon in Chrome
7. Chrome toont een banner: **"Toevoegen aan beginscherm"** → tik erop
8. De app verschijnt als echt app-icoontje op je thuisscherm!

### Lokaal testen (Claude Code)

```bash
# Installeer een simpele webserver
npm install -g serve

# Start de app
cd vakantie-app
serve .

# Open in browser: http://localhost:3000
```

### Via Claude Code op GitHub zetten

```bash
# In je terminal (Claude Code):
git init
git add .
git commit -m "Vakantie app eerste versie"
gh repo create vakantie-ommen --public --push --source=.
# Zet daarna GitHub Pages aan in de repository settings
```

## Features

- 📅 Volledig dagprogramma 4–20 juli
- 🗂 Filter op type dag (NL, Duitsland, actief, rust)
- 🗺 Google Maps link per bestemming
- ✨ AI-knop: vraagt extra info op per stad via Claude API
- ✏️ Zelf aanpassen: eigen titels en notities per dag
- 📴 Offline werking via Service Worker
- 📱 Installeerbaar op Android als PWA

## Kleuren & stijl

Cuba Libre retro thema:
- Geel `#F9E04B` — hoofdaccent
- Lichtblauw `#7EC8E3` — lucht en water
- Roze `#F4A7B9` — accenten
- Mint `#B5E8D0` — natuur
- Creme `#FFF8E7` — achtergrond
- Donkerblauw `#1A3A47` — hero en footer

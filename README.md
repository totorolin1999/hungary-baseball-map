# ⚾ Hungarian Baseball & Softball Map

> **Magyar Baseball és Softball Pályák Térképe**  
> An interactive web map showcasing baseball and softball clubs, ballparks, official coordinates, and club resources across Hungary.

---

## 🌟 Features

- **🗺️ Interactive Map (Leaflet.js)**: Explore all active baseball and softball fields throughout Hungary with custom markers, detailed popups, and direct Google Maps navigation links.
- **🔍 Real-Time Search & Filtering**: Filter teams by league tiers (NB I, NB II, Youth Academy, etc.) or search directly by club name and city.
- **📍 Nearest Ballpark Discovery**: GPS-based geolocation calculates real-time distances to every ballpark and sorts the list from nearest to farthest.
- **🌐 Bilingual UI**: Seamless one-click switching between Hungarian (Magyar) and English.
- **📱 Fully Responsive**: Optimized for desktop and mobile displays with an intuitive sliding drawer on smaller screens.

---

## 🚀 Quick Start & Local Development

Because team and stadium data are dynamically fetched from [`teams.json`](teams.json), modern browsers require a local web server (to bypass CORS file:// restrictions):

### Using Python 3:
```bash
python -m http.server 8000
```
Open in browser: `http://localhost:8000`

### Using Node.js (npx):
```bash
npx serve .
```

---

## 📦 Data Schema (`teams.json`)

All club and ballpark information is centralized in [`teams.json`](teams.json). Each record follows this structure:

```json
{
  "id": "budapest-red-wolves",
  "name": "Budapest Red Wolves",
  "league": "nbi",
  "tierLabelHU": "NB I Bajnok / Interleague",
  "tierLabelEN": "NB I Champion / Interleague",
  "cityHU": "Budapest (18. kerület)",
  "cityEN": "Budapest (District 18)",
  "ballparkHU": "Budapest RedWolves Park (Thököly út 11)",
  "ballparkEN": "Budapest RedWolves Park (Thököly út 11)",
  "coords": [47.4478, 19.1853],
  "socials": {
    "website": "https://redwolves.hu",
    "facebook": "https://www.facebook.com/BudapestRedWolvesBaseballSE",
    "instagram": "https://www.instagram.com/budapestredwolves"
  }
}
```

---

## 🤝 Contributing & Feedback

Contributions, corrections, and improvements from baseball enthusiasts and developers are always welcome:

- **Found incorrect ballpark coordinates, team info, or outdated links?** Feel free to open an [Issue](../../issues)!
- **Want to add missing clubs or improve map interactions?** Pull Requests are warmly welcome!

---

## 📄 License

This project is open-source and licensed under the [MIT License](LICENSE).

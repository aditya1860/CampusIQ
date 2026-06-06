# CampusIQ 🎓

> A modern, zero-dependency college discovery platform built for Indian students — search, filter, compare, and predict admission chances across top institutions.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/status-live-brightgreen?style=flat-square)

---

## 🌐 Live Demo

https://campus-iq-mu-nine.vercel.app/

---

## 📸 Preview

| Discover | Compare | Predictor |
|----------|---------|-----------|
| Browse & filter colleges | Side-by-side metrics | AI-powered admission chances |

---

## ✨ Features

- **🔍 Smart Search** — Instantly filter colleges by name, course, or city
- **🎛️ Multi-filter Sidebar** — Filter by state, institution type, fees range, and rating
- **📊 Side-by-Side Compare** — Compare up to 3 colleges with best-value highlights
- **🎯 College Predictor** — Enter your JEE / CAT / NEET / BITSAT rank and get admission probability
- **📋 College Detail View** — Deep-dive into placements, courses, and student reviews
- **⚡ Zero Dependencies** — Pure HTML + CSS + JS. No React, no Node, no build step
- **🌑 Premium Dark UI** — Amber/gold accent system with smooth micro-animations
- **📱 Responsive** — Works on mobile, tablet, and desktop

---

## 🏛️ Colleges Included

| College | Type | NIRF |
|---------|------|------|
| IIT Bombay | IIT | #1 |
| IIT Delhi | IIT | #2 |
| IIM Ahmedabad | IIM | #1 |
| AIIMS Delhi | Government | #1 |
| NIT Trichy | NIT | #8 |
| BITS Pilani | Private | #16 |
| VIT Vellore | Private | #22 |
| Manipal Institute | Private | #35 |

---

## 🚀 Getting Started

### Run Locally

No installation needed. Just open the file:

```bash
# Option 1 — Double-click
# Simply open index.html in any modern browser

# Option 2 — Local server (recommended)
python -m http.server 8000
# Then visit: http://localhost:8000
```

### Clone & Run

```bash
git clone https://github.com/aditya1860/CampusIQ.git
cd CampusIQ
# Open index.html in your browser
```

---

## 📁 Project Structure

```
CampusIQ/
│
├── index.html        # Entire application — single self-contained file
└── README.md         # You are here
```

> **Why a single file?** This project is intentionally kept as one file for maximum portability — no build tools, no package managers, no configuration. Drop it anywhere and it works.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 (semantic) |
| Styling | CSS3 (custom properties, grid, flexbox, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| Icons | Tabler Icons (CDN) |
| Fonts | Syne + DM Sans (Google Fonts) |
| Hosting | GitHub Pages |

---

## 🧭 How It Works

```
User opens app
      │
      ├── Discover Tab
      │     ├── Search bar filters in real-time
      │     ├── Sidebar filters (state / type / fees / rating)
      │     ├── Sort by rating, fees, or NIRF rank
      │     └── Click any card → College Detail View
      │
      ├── Compare Tab
      │     ├── Add up to 3 colleges via "+ Compare" button
      │     ├── Side-by-side table with 9 metrics
      │     └── Green highlight = best value per row
      │
      └── Predictor Tab
            ├── Select exam (JEE Adv / Main / CAT / NEET / BITSAT)
            ├── Enter rank or percentile
            ├── Select category (General / OBC / SC-ST)
            └── Returns probability % for all colleges
```

---

## 🔧 Customisation

### Add a New College

Open `index.html` and find the `COLLEGES` array. Add a new object:

```javascript
{
  id: 9,
  name: "Delhi Technological University",
  loc: "New Delhi, Delhi",
  type: "Government",
  fees: 175000,
  rating: 4.2,
  nirf: 36,
  courses: ["B.Tech", "M.Tech", "MBA"],
  placements: { avg: 900000, highest: 2500000, pct: 85 },
  reviews: [
    { author: "Rohit K.", text: "Great faculty and strong alumni network." }
  ],
  icon: "🏢"
}
```

### Change the Accent Color

Find the `:root` CSS block and update `--accent`:

```css
:root {
  --accent: #f5a623;      /* Current: amber */
  --accent-glow: rgba(245, 166, 35, 0.15);
}
```

---

## 📦 Deployment

### GitHub Pages (Free)

1. Push code to a public GitHub repository
2. Go to **Settings → Pages**
3. Source: `Deploy from branch` → `main` → `/ (root)`
4. Click **Save** — live in ~60 seconds


### Vercel (Free)

```bash
npm i -g vercel
vercel
```

---

## 🤝 Contributing

Contributions are welcome!

```bash
# 1. Fork the repo
# 2. Create your feature branch
git checkout -b feature/add-more-colleges

# 3. Commit your changes
git commit -m "feat: add 10 more colleges with placement data"

# 4. Push and open a Pull Request
git push origin feature/add-more-colleges
```

**Ideas for contribution:**
- Add more colleges (NIT Warangal, IIT Madras, etc.)
- Add a bookmarks / shortlist feature
- Add a dark/light mode toggle
- Improve predictor algorithm accuracy
- Add entrance exam cutoff data

---

## 📄 License

MIT License — free to use, modify, and distribute. See [LICENSE](LICENSE) for details.

---

## 👤 Author

**Aditya** — [@aditya1860](https://github.com/aditya1860)

Built as part of an internship OA task — Track B: College Discovery Platform.

---

<p align="center">
  Made with ❤️ and a lot of ☕
</p>

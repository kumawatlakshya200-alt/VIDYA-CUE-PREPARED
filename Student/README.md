# VIDYA-CUE — College Portal (Updated with Teacher Portal)

A comprehensive college portal with student dashboard and newly converted teacher portal.

## 🆕 NEW: Teacher Portal (Vanilla JavaScript)

The React-based teacher portal has been successfully converted to **pure HTML, CSS, and JavaScript**!

### ⚡ Quick Start
```
Open: teacher.html in any web browser
No installation needed • No build process • All features working
```

### 📋 Features
- ✅ Dashboard with statistics
- ✅ QR Code generation
- ✅ Assignment management
- ✅ Attendance tracking
- ✅ Grade management
- ✅ Schedule view
- ✅ Dark/Light theme
- ✅ Responsive design

### 📁 Files
```
teacher.html                  ← Main entry point
teacher/
├── styles.css              - CSS styling
├── main.js                 - App logic
├── pages.js                - Page renderers
├── components.js           - UI components
├── data.js                 - Mock data
└── utils.js                - Helpers
```

### 📚 Documentation
- **QUICK_START.md** - How to use the portal
- **TEACHER_PORTAL_GUIDE.md** - Integration & customization
- **CONVERSION_SUMMARY.md** - Technical details
- **teacher/README.md** - Full technical docs

---

## 📚 Student Portal

Original features maintained:
- Added a reusable header (`studentheader.html`) and created `include-html.js` to inject it into each page.
- Added `styles.css` for shared styling.
- Updated each page to include `header placeholder`, `styles.css` and the header injector script.
- Dashboard (`studentdashboard.html`) now displays a grid of card links to the major pages and has sidebar buttons linked to full pages.
- `login.html` now stores a mock user in `localStorage` and redirects to the dashboard; header shows logged in name.
- Header has a nav with links to all pages and a small active-link highlight.

How to run locally (recommended):
- The header is injected via `fetch`, so opening files with `file://` may cause network restrictions. Use a simple static server.

Using Python (3.x):
```
cd c:\Users\hp\Desktop\HImanshu\2.0
python -m http.server 8000
```

Using `http-server` (Node.js):
```
npm i -g http-server
cd c:\Users\hp\Desktop\HImanshu\2.0
http-server -p 8000
```

Then open http://localhost:8000/homepage.html (or any page) in your browser.

Notes & next steps:
- You might want to move header styles into a separate `styles.css` and reduce duplication.
- Add server-side session handling (if needed) and replace `localStorage`-based mock login with a real auth flow.
- The header HTML is kept in `studentheader.html` and is injected into all pages to keep things DRY.

Enjoy! 🎓

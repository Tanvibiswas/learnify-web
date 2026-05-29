# Learnify 📚 — Study Resource Organizer

> *"Save once. Find always. Learn better."*

A smart, browser-based study resource organizer built for **Neurathon** (PS1) by **Team Behind the UI**. Learnify helps students save, organize, search, and track all their study links in one clean, distraction-free workspace — no backend, no sign-up, no clutter.

---

## 👥 Team Members

- Tanvi Biswas(leader)
- Kaushika Goswami
- Sakshi Priya
- Sharmistha Buragohain

---

## 🧩 The Problem

Students today deal with information overload without any organization system:

- **Lost productivity** — Wasting time searching for resources already found once but forgotten
- **Bookmark chaos** — Browser bookmarks are unsorted, unsearchable, and cluttered with personal and academic links mixed together
- **No context retention** — A raw link saved in a notes app has no label, category, or priority, making it meaningless days later
- **Fragmented tools** — Students juggle browser tabs, note apps, and Google Docs with no unified system
- **Exam pressure** — During revision, quick access to the right resource at the right time directly impacts performance

---

## ✨ Features

### #1 — The Completed System
Mark any resource as done with a ✓ and it instantly disappears from your active grid — no clutter, no dimmed cards. It moves into a dedicated **Completed** view, grouped by subject. Changed your mind? Hit **Undo** and it's back instantly.

### #2 — Live Progress Tracker
A real-time progress bar that fills up green as you work. Displays your exact completion percentage, how many resources are done, pending, and overdue — all updating the moment you interact with anything.

### #3 — Ollie the Owl 🦉
Not just a decoration. Ollie is a reactive mascot who lives in your sidebar and responds to your actual progress:
- 🎉 Celebrates every 25% milestone
- ⚠️ Warns you when something goes overdue
- 📉 Calls out the exact percentage drop when you undo tasks
- 🎊 Goes wild with animations when you hit 100%

### #4 — Fully Inline Editable Cards
Edit any resource card directly — title, URL, tags, due date, notes — without opening a separate page or losing your place.

### #5 — Smart Search
Searches titles, tags, notes, and categories simultaneously. Uses word-boundary matching so searching "cs" finds "Computer Science" but won't incorrectly match "Physics."

### #6 — Due Date Ribbons
A colored ribbon sits at the top of every card:
- 🔴 Red — overdue
- 🟡 Yellow — due soon
- 🟢 Green — upcoming

You see urgency before you read anything.

### #7 — Clickable Tag System
Add multiple tags to any resource. Click a tag to instantly filter the entire workspace to only show resources with that tag. Click again to clear. No dropdowns, no menus.

### Additional Features
- **Custom Grids** — Organize resources into subject-specific grids with custom colors and emoji icons
- **Star/Priority Toggle** — Mark high-priority resources with a star
- **Color Picker** — Full HSV color picker for personalizing grid colors
- **Collapsible Sidebar** — Clean, minimal sidebar that collapses to icon-only mode with tooltip hints
- **Toast Notifications** — Subtle feedback messages for every action
- **Landing Page** — Smooth animated entry into the app

---

## 🛠️ Tech Stack

| Technology | Role |
|---|---|
| HTML5 | Structure & Semantics |
| CSS3 | Styling, Grid & Flexbox layouts |
| JavaScript (Vanilla) | Logic, DOM manipulation |
| LocalStorage | Persistent data (no server needed) |
| Google Fonts | Typography (Playfair Display, DM Sans) |

**Pure frontend — no backend, no database, no server required. Runs entirely in the browser.**

---

## ⚙️ Implementation Flow

1. **UI Layout** — Input form + category filter bar + resource card grid
2. **Data Layer** — Resources stored as JSON objects in `localStorage`
3. **Add Resource** — Capture title, URL, category → push to array → re-render
4. **Filter Logic** — Filter array by selected category → re-render cards
5. **Search** — Live filter on keyup across title, tags, notes, and categories
6. **Bonus** — Star toggle, tag chips, favicon via Google Favicon API, Ollie reactions, color picker, emoji picker

---

## 📁 Project Structure

```
PS1/
└── index.html      ← Entire app (HTML + CSS + JS in one file, no dependencies)
```

---

## 🚀 Running the App

No installation needed. Since the app is pure frontend:

**Option 1 — Just open the file:**
```
Double-click index.html in File Explorer
```

**Option 2 — Via local server (recommended):**
```bash
python -m http.server 8000
```
Then open `http://localhost:8000/index.html`

All data is saved automatically to your browser's `localStorage` and persists across sessions.

---

## 🔒 Data & Privacy

All data is stored **locally in your browser** using `localStorage`. Nothing is sent to any server. Clearing your browser data will erase saved resources.

---

## 🏆 Built for

**ECS Web Dev Hackathon — Study Resource Organizer**
Team: Behind the UI

# 📔 Monthly Habit Tracker

A **single-file, offline-first habit tracker** that looks and feels like a paper journal.
No build step, no install, no account, no server — just open `index.html` in any browser and start tracking.

## ✨ Features

- **Monthly grid** — tap a box to check off up to 10 custom habits for every day of the month
- **Custom section** — rename the whole section and its boxes to track anything (default: prayer)
- **Sleep tracker** — log fall-asleep / wake-up times; hours are calculated automatically, plus a "slept enough?" toggle
- **Water tracker** — 8 blocks × 250 ml (2 L goal per day)
- **Daily memories** — one line per day, expands into a bigger box when you focus it
- **Highlights of the month** — a space for lessons learned, milestones and wins
- **Best moments & goals** — a second spread with memorable moments and a goal list with a progress bar
- **Month summary** — live stats: habit boxes filled, most consistent habit, average sleep, water intake, goals done
- **Month navigation** — flip back and forth between months with `‹` / `›`; today's row is always highlighted
- **Light & dark themes** — follows your system preference, switchable with the ◐ button
- **Everything is editable** — rename habits, add/remove them, rename the custom section, all from the "Customize" panel

## 🚀 Getting started

**Option 1 — just open it**

Download `index.html` and double-click it. That's it.

**Option 2 — run it from this repo**

```bash
git clone https://github.com/parigalaprashanthkumarkvsr-code/monthly-habit-tracker.git
cd monthly-habit-tracker
# open index.html in your browser, or serve it:
python3 -m http.server 8000   # then visit http://localhost:8000
```

**Option 3 — GitHub Pages**

This repo can be served directly via GitHub Pages (Settings → Pages → deploy from branch → `index.html`).

## 💾 How your data is stored

All data is saved in your browser's **`localStorage`** under the key `habit-tracker-v1`.
Nothing ever leaves your device — there are no cookies, no analytics, and no network calls
(apart from loading two Google Fonts, and the page falls back to system fonts without them).

> ⚠️ Data is tied to the specific browser + device you use. Clearing browser data will erase it.
> Tip: use your browser's "Save page as…" to keep dated snapshots of a filled-in month.

## ⌨️ Usage tips

- **Tap / click** a habit box to toggle it. Tap again to untoggle.
- **Water blocks** fill up progressively — tap block 4 to log 1 L, block 8 for 2 L.
- **Sleep**: set the From/To times and the hours column updates instantly.
- **Memories**: click into a day's line and it expands into a full text area.
- **Rename habits** under *Customize habits & custom section* — the first letter becomes the column label automatically.
- Navigate months freely; each month keeps its own data.

## 🧰 Tech

- Pure **HTML + CSS + vanilla JavaScript** in one file (~20 KB)
- Handwritten-journal styling with *Patrick Hand* and *Caveat* fonts
- Sticky header row and sticky day column for easy scrolling
- Responsive with a zoomed "notebook spread" layout that fits any screen width
- Keyboard accessible: all cells and inputs have focus styles and ARIA labels

## 📄 License

MIT — do whatever you like with it.

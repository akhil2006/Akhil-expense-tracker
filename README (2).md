# AI-Assisted Expense Tracker

Program 05 · AI Assisted Software Development Lab (BASDLI507)

A React + localStorage expense tracker with categories, monthly analytics and CSV export.
It is a static site: nothing to install, and it needs no internet connection to run once loaded.

## Files
- `index.html`: page shell
- `bundle.js`: the compiled app (React included). This is what the browser runs.
- `style.css`: styling
- `app.jsx`: readable React source code, grouped by layer (data model, UI shell, state, persistence, analytics). Use it for your viva and lab record. It is not loaded by the site.

## Features
- Add expenses (amount > 0, category required, date defaults to today, note up to 120 characters)
- Expense table sorted by date (newest first), coloured category tags, delete with confirmation
- Category manager: add, rename/recolour, delete (affected expenses are reassigned first)
- `useLocalStorage` hook: JSON saved in the browser, loaded on mount, debounced writes
- Analytics: monthly total with % change vs last month, category donut chart, 6-month trend chart (SVG)
- CSV export of all expenses
- "Load sample data" button on the empty screen, useful for screenshots

## Upload to GitHub
1. Create a new repository (for example `expense-tracker`).
2. Add file > Upload files, then add `index.html`, `bundle.js`, `style.css`, `app.jsx`, `README.md`.
3. Commit changes.

## Deploy on Vercel
1. Sign in at vercel.com with GitHub.
2. Add New > Project, import the repository.
3. Framework Preset: **Other**. Leave build command and output directory empty.
4. Deploy.

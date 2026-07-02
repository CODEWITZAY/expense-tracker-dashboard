# Expense Tracker Dashboard

A personal finance dashboard for tracking monthly bills, income, and spending — all in a single self-contained HTML file with no backend or dependencies beyond Chart.js.

**Live site:** https://codewitzay.github.io/expense-tracker-dashboard/

## Features

- **Bill management** — add, edit, delete, and mark bills as Paid / Unpaid / Upcoming / AutoPay
- **Category filtering** — Housing, Utilities, Insurance, Subscriptions, Transportation, Health, Other
- **Income tracker** — enter two incomes (editable in place) and see your leftover budget after bills
- **Calendar view** — July 2026 calendar with color-coded bill chips per day; click any day to open a detail panel and manage bills for that date
- **Charts** — bar chart of spending by category and a donut chart of budget breakdown (powered by Chart.js)
- **Progress bars** — paid vs. total per category at a glance
- **Sortable table** — sort by name, category, amount, due date, or status; live search included
- **Persistent storage** — bills and income values are saved to `localStorage` so data survives page refreshes

## Usage

No installation needed. Open `index.html` directly in any modern browser, or visit the live GitHub Pages URL above.

```
index.html          # Open this in a browser
july_dashboard.html # Original source file (same content)
```

## How It Works

Everything runs client-side in a single HTML file:

- **State** is kept in a JavaScript `bills` array and synced to `localStorage` on every change
- **Charts** use [Chart.js 4.5.1](https://www.chartjs.org/) loaded from jsDelivr CDN
- **No frameworks** — plain HTML, CSS, and vanilla JavaScript
- **Responsive** — adapts to mobile screens via CSS Grid and media queries

## Tech Stack

| Layer | Details |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 — CSS custom properties, Grid, Flexbox |
| Logic | Vanilla JavaScript (ES6+) |
| Charts | Chart.js 4.5.1 via CDN |
| Persistence | Browser `localStorage` |
| Hosting | GitHub Pages |

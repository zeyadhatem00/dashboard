# مدبّر — Personal Finance Dashboard UI

An Arabic, right-to-left personal-finance dashboard presented as a static front-end interface. The page brings balances, activity, bills, budgets, transactions, account summaries, and payment-card visuals into one responsive dashboard.

## What is included

- **Overview cards** for current balance, income, and spending, with sample percentage changes.
- **Recent activity** and **monthly bills** panels with categories and due-date labels.
- **Budget overview** with total/remaining amounts and progress bars for several spending categories.
- **Recent transactions** table with sample income, spending, category, date, status, and amount data.
- **Income versus spending** visual with a four-week bar comparison.
- **Account summary** for current, savings, and credit accounts, plus illustrated Visa, Mastercard, and PayPal cards.
- **Responsive layout** that moves from a desktop sidebar/grid to a single-column mobile layout at widths up to 600px.

## Current scope

This repository is a visual demo, not a connected banking or budgeting application. The displayed figures, names, dates, balances, transactions, bills, account details, card details, and chart values are static HTML content in `index.html`. There is no persistence, authentication, backend, API integration, or user-specific data flow.

The page contains buttons for navigation, search, notifications, quick actions, details, analysis, and management, but no JavaScript event handlers or linked routes are implemented. These controls are therefore visual UI elements only.

## Tech stack

- HTML5 for the page structure and Arabic content.
- CSS3 for the layout, cards, tables, progress bars, hover states, and animations.
- [IBM Plex Sans Arabic](https://fonts.google.com/specimen/IBM+Plex+Sans+Arabic) loaded from Google Fonts.
- Local Font Awesome CSS and webfont files in `CSS/` and `webfonts/` for icons.

There is no `package.json`, lockfile, build tool, JavaScript bundle, environment file, or project-specific dependency installation step. The page is served as static files.

## Run locally

1. Clone the repository and enter it:

   ```bash
   git clone --depth 1 https://github.com/zeyadhatem00/personal-finance-dashboard.git
   cd dashboard
   ```

2. Open `index.html` in a browser. Because this is a static site, no build step or environment variables are required.

For a local static server, use any server that serves the repository root and then open its displayed local address. The repository does not define a preferred server command or a package-manager script.

## Project structure

```text
.
├── index.html                 # Complete dashboard markup and sample data
├── CSS/
│   ├── style.css              # Desktop layout and component styles
│   ├── media.css              # Mobile breakpoint styles
│   └── all.min.css             # Local Font Awesome CSS
├── Images/                    # Favicon and avatar artwork
├── webfonts/                  # Local Font Awesome webfonts
└── .github/workflows/
    └── static.yml             # GitHub Pages deployment workflow
```

## External services and configuration

The only external request declared by the page is the Google Fonts stylesheet for IBM Plex Sans Arabic. If it is unavailable, the CSS font stack falls back to a sans-serif font. No API keys, secrets, environment variables, or external application services are required.

The included GitHub Actions workflow deploys the complete repository to GitHub Pages on pushes to `main` and supports manual dispatch. A Pages deployment URL is not declared in the repository, so no live-demo URL is listed here.

## Repository

- Source: [zeyadhatem00/dashboard](https://github.com/zeyadhatem00/personal-finance-dashboard)
- Default branch: `main`

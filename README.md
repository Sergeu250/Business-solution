# BizFlow Rwanda 🇷🇼

An all-in-one business management web app built for Rwandan small and medium enterprises. Track inventory, manage customers, and monitor your stock value — all from a clean, fast, browser-based interface with no installation required.

---

## Live Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Landing page with features overview |
| Register | `register.html` | Create a new business account |
| Login | `login.html` | Log in to your account |
| Dashboard | `stock.html` | Manage your product inventory |
| Customers | `customers.html` | View and manage registered accounts |

---

## Features

- **Inventory Management** — Add products with name, quantity, and price. Grand total value is calculated automatically in RWF.
- **Customer Registry** — View all registered businesses with their TIN numbers. Search by name, email, or TIN.
- **Secure Accounts** — Each business account has its own private data. Products are stored per user, not shared.
- **Rwanda-ready** — TIN number field built in. Prices displayed in Rwandan Francs (RWF).
- **No backend needed** — All data is stored in the browser via `localStorage`. Works offline.

---

## Getting Started

### Option 1 — Open directly in a browser

Download the repo and open `index.html` in any modern browser. No server, no dependencies, no build step.

```bash
git clone https://github.com/Sergeu250/Business-solution.git
cd Business-solution
open index.html   # macOS
# or double-click index.html on Windows/Linux
```

### Option 2 — Serve locally (recommended)

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000` in your browser.

---

## How to Use

1. **Register** — Go to `register.html`, enter your email, business name, TIN, and a password.
2. **Log in** — Use your email and password on `login.html`.
3. **Add products** — On the Dashboard (`stock.html`), fill in a product name, quantity, and unit price, then click **Add**.
4. **View customers** — On the Customers page (`customers.html`), see all registered accounts. Use the search bar to filter.
5. **Log out** — Click **Log out** in the sidebar at any time.

---

## Project Structure

```
Business-solution/
├── index.html       # Homepage / landing page
├── register.html    # Account registration
├── login.html       # Login form
├── stock.html       # Inventory dashboard
├── customers.html   # Customer management
└── README.md
```

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 |
| Styling | CSS3 (custom, no frameworks) |
| Logic | Vanilla JavaScript |
| Storage | Browser `localStorage` |
| Fonts | Google Fonts — Inter |

No external libraries. No backend. No database. Runs entirely in the browser.

---

## Data & Privacy

All data is stored locally in the user's browser via `localStorage`. Nothing is sent to any server. Clearing browser storage or using a different browser/device will reset the data.

> **Note:** This is a frontend-only prototype. For production use, connect to a real backend (e.g. Node.js + PostgreSQL) and replace `localStorage` with authenticated API calls. Do not store passwords in plain text in production.

---

## Screenshots

| Page | Description |
|------|-------------|
| Homepage | Hero section with dashboard preview and feature cards |
| Register | Split-panel layout with business onboarding checklist |
| Login | Centered card with branded header |
| Dashboard | Sidebar nav, stats cards, add-product form, product table |
| Customers | Searchable table with avatar initials and TIN display |

---

## Roadmap

- [ ] Sales / POS module
- [ ] PDF invoice generation
- [ ] Bookkeeping and expense tracking
- [ ] CSV export for inventory and customers
- [ ] Backend integration (Node.js + PostgreSQL)
- [ ] Multi-language support (Kinyarwanda / French / English)

---

## Contributing

Pull requests are welcome. For major changes, open an issue first to discuss what you'd like to change.

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push: `git push origin feature/my-feature`
5. Open a Pull Request

---

## License

MIT — free to use, modify, and distribute.

---

*Built for businesses like yours in Rwanda.*

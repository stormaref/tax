# محاسبه‌گر مالیات بر حقوق | Iran Salary Tax Calculator

A free, open-source web tool for calculating Iranian payroll income tax using the official progressive (stepped) tax brackets. Supports tax years **1404** and **1405** (Iranian calendar).

**Live demo:** [stormaref.github.io/tax](https://stormaref.github.io/tax/)

---

## Features

- **Progressive tax calculation** — Applies the official multi-bracket tax rates automatically
- **Year selector** — Switch between 1404 and 1405 tax tables instantly
- **Social security insurance** — Calculates the employee's 7% share of social security contributions
- **Net salary output** — Shows the final take-home pay after tax and insurance deductions
- **Tax bracket table** — Expandable reference table showing all rate tiers for the selected year
- **Real-time results** — Calculations update live as you type
- **Persian formatting** — Currency values displayed with Persian digits and comma separators
- **Responsive design** — Works seamlessly on mobile, tablet, and desktop
- **Zero dependencies** — Pure HTML, CSS, and vanilla JavaScript; no build step required
- **SEO optimized** — Open Graph, Twitter Card, and JSON-LD structured data included

## Tax Brackets (1405)

| Bracket | From (Toman) | To (Toman) | Rate |
|---------|-------------|------------|------|
| 1 | 0 | 40,000,000 | Exempt |
| 2 | 40,000,000 | 80,000,000 | 10% |
| 3 | 80,000,000 | 100,000,000 | 15% |
| 4 | 100,000,000 | 120,000,000 | 20% |
| 5 | 120,000,000 | 140,000,000 | 25% |
| 6 | 140,000,000 | — | 30% |

## Getting Started

### Run locally

Clone the repository and open `index.html` in a browser — no server or build tools needed:

```bash
git clone https://github.com/stormaref/tax.git
cd tax
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

### Deploy

The project is a single HTML file with inline CSS and JS, so it can be deployed anywhere that serves static files — GitHub Pages, Netlify, Vercel, Cloudflare Pages, or a plain web server.

## Project Structure

```
tax/
├── index.html   # Complete application (markup, styles, and logic)
├── LICENSE      # Apache 2.0
└── README.md
```

## How It Works

1. The user enters their **taxable salary** in Toman
2. The calculator applies the **progressive tax brackets** for the selected year — each income tier is taxed at its own rate
3. A **7% social security insurance** deduction is computed on the gross salary
4. The **net salary** is calculated as: `gross - tax - insurance`

All computation happens client-side with no data sent to any server.

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

If you find this tool useful, please star the [GitHub repository](https://github.com/stormaref/tax) to help others discover it.

## License

This project is licensed under the [Apache License 2.0](LICENSE).

# Three Crises, One Economy 🇬🇧

A visual, interactive analysis comparing the economic impact of three major global crises on the United Kingdom: **COVID-19**, the **Ukraine War**, and the **Iran War**.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat&logo=chartdotjs&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## About

This single-page, self-contained website presents a clear financial breakdown of how each crisis affected the UK economy across key dimensions including GDP, inflation, energy prices, government spending, and national debt.

It was built to make complex economic data accessible, visual, and easy to understand, without requiring a degree in economics to follow along.

## Features

- **Fully interactive charts** powered by Chart.js with hover tooltips
- **Six data-driven sections** covering GDP, inflation, energy shocks, government spending, debt, and overall severity
- **Scroll-triggered animations** for a smooth, engaging reading experience
- **Dark editorial design** with a distinctive colour palette and typography
- **Radar chart** showing the comparative severity fingerprint of each crisis
- **Responsive layout** that works across desktop, tablet, and mobile
- **Zero dependencies at runtime**, just a single HTML file and a CDN link to Chart.js
- **No build step required**, open the file in any browser and it works

## Sections

| Section | What It Covers |
|---|---|
| Crisis Snapshot | At-a-glance summary cards with key metrics for each crisis |
| GDP Growth | Bar chart comparing annual GDP change during each event |
| Inflation | Bar chart of CPI at key moments plus a line chart showing the full trajectory |
| Energy Price Shocks | Side-by-side comparison of petrol and wholesale gas price changes |
| Government Spending & Debt | Fiscal response scale and debt-to-GDP ratios over time |
| Comparative Severity | Radar chart plotting relative impact across six dimensions |

## Getting Started

### Option 1: Just open it

Download `uk-crisis-comparison.html` and open it in any modern browser. That is genuinely it.

### Option 2: Clone the repo

```bash
git clone https://github.com/yourusername/uk-crisis-comparison.git
cd uk-crisis-comparison
open uk-crisis-comparison.html
```

### Option 3: Serve locally

If you prefer a local dev server:

```bash
npx serve .
```

Then visit `http://localhost:3000` in your browser.

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and content |
| CSS3 | Styling, animations, scroll-triggered reveals |
| Chart.js 4.4.1 | All interactive charts (bar, line, radar) |
| Google Fonts | DM Sans (body) and Playfair Display (headings) |

## Data Sources

All figures are drawn from publicly available, authoritative sources:

- IMF World Economic Outlook (April 2026)
- Office for National Statistics (ONS)
- Bank of England
- House of Commons Library
- Office for Budget Responsibility (OBR)
- OECD

Iran war figures are early estimates and forecasts, and are clearly labelled as such throughout.

## Customisation

Since it is a single HTML file, customisation is straightforward. The key design tokens are defined as CSS variables at the top of the `<style>` block:

```css
:root {
  --covid: #E63946;
  --ukraine: #457B9D;
  --iran: #E9C46A;
  --bg: #0B1120;
  --card: #111827;
  --text: #E2E8F0;
}
```

Chart data is defined in plain JavaScript objects within the `<script>` block at the bottom of the file, so updating figures as new data becomes available is simple.

## Browser Support

Tested and working in:

- Chrome 90+
- Firefox 90+
- Safari 15+
- Edge 90+

## Contributing

Contributions are welcome. If you spot an error in the data, have a design improvement, or want to add a new section, feel free to open an issue or submit a pull request.

## Licence

This project is licensed under the MIT Licence. See the `LICENCE` file for details.

## Acknowledgements

Built with care using data from the sources listed above. Inspired by a desire to make economic analysis accessible and visually engaging for everyone, not just economists.

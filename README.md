# Pricing Table — Flexbox Layout

A responsive three-tier pricing table built with CSS Flexbox, demonstrating a common SaaS-style product pricing layout. The cards adapt from a horizontal row on wide screens to a vertical stack on narrow viewports via a single media query.

## Overview

Three pricing plans — Basic ($11.99/mo), Standard ($19.99/mo), and Premium ($49.99/mo) — are displayed as horizontally distributed cards. Each card lists a plan name, price, feature checklist, and a sign-up button. Below 1250px, the layout switches to a single-column vertical stack.

## Tech Stack

| Technology | Role |
|---|---|
| HTML5 | Semantic structure |
| CSS3 + Flexbox | Card layout and responsive stacking |
| Google Fonts (Sono) | Typography |

## Project Structure

```
pricing-table-flexbox/
├── index.html      — All HTML and CSS in a single file
└── solution.html   — Reference implementation
```

## Getting Started

Open `index.html` in any browser. An internet connection is needed to load the Google Font.

## Key Concepts

- `display: flex` for horizontal card distribution
- `justify-content: center` and `gap` for spacing
- `flex: 1` combined with `max-width` for equal-width constrained cards
- `@media (max-width: 1250px)` to switch `flex-direction` to `column`

---
*Part of the Antigravity project collection — Saptarshi Sadhu*
"# pricing-table-flexbox" 

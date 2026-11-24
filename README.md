# Pulse — CRM Dashboard Demo

A SaaS-style CRM dashboard in one HTML file: KPI cards with animated counters, hand-rolled canvas charts (no chart library), a deals pipeline table and an activity feed. Zero dependencies.

![Stack](https://img.shields.io/badge/stack-vanilla%20JS-c8f542) ![Deps](https://img.shields.io/badge/dependencies-0-c8f542)

## Features

- **KPI cards** — revenue, active deals, new contacts, churn, with eased count-up animation and delta indicators
- **Revenue chart** — 12-week line chart with gradient fill and a comparison series, drawn on raw `<canvas>`
- **Pipeline chart** — deals-by-stage bars, also raw canvas (rounded bars via `roundRect`)
- **Deals table** — company marks, values, stage pills, owners
- **Activity feed** — timestamped team events
- **Responsive** — sidebar collapses behind a hamburger on mobile; charts redraw on resize at device pixel ratio

## Run it

```bash
open index.html
# or
npx serve .
```

## Notes

All numbers are sample data. The charts are written by hand on purpose — for a dashboard of this size a chart library is dead weight, and drawing directly keeps the bundle at zero bytes of JavaScript dependencies.

---

*Demo project by [Jameel Ali](https://github.com/jalidev).*

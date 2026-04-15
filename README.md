# Data: What It Is, What It Can Tell Us, and What It Can't

An interactive Reveal.js presentation for 8th grade data science, by Krista Herling and Nathan Layman.

**Live site:** [n8layman.github.io/data-thinking](https://n8layman.github.io/data-thinking)

## What's in the presentation

- **Why we need data** — the Birthday Problem, gut feelings, and why intuition fails
- **Four cognitive fallacies** — Association Fallacy, Survivorship Bias, Texas Sharpshooter, Gambler's Fallacy
- **Interactive games** — coin flip (Gambler's Fallacy), full Monty Hall simulator
- **Data concepts** — central tendency, spread, correlation vs. causation, falsifiability
- **Real weather data** — NOAA Wenatchee, WA station (1931–present): yearly high/low temperature, annual precipitation, and max snow depth — with discussion prompts

## Data

Weather data sourced from NOAA Climate Data Online, station USC00459074 (Wenatchee, WA). Processed into `docs/weather-data.js` for client-side rendering with Plotly.js.

## Running locally

```bash
python3 -m http.server 8080 --directory docs
```

Then open [http://localhost:8080](http://localhost:8080).

## Tech

- [Reveal.js](https://revealjs.com/) 5.1.0
- [Plotly.js](https://plotly.com/javascript/) 2.32.0
- No build step — single HTML file + static assets

# MalariaFore: Malaria Forecasting Web Application

MalariaFore is a browser-based public health analytics dashboard for malaria trend monitoring, forecast simulation, climate-risk visualization, and resource planning.

The application is designed around a dataset-first workflow:
1. Upload malaria CSV data.
2. Analyze trends and climate correlation.
3. Simulate forecast outputs.
4. Review district risk maps and resource allocation charts.

## Project Highlights

- Upload-first gated dashboard flow.
- CSV ingestion from user upload or bundled sample dataset.
- Trend analytics with historical and forecast views.
- Climate correlation visualization (rainfall vs malaria cases).
- District risk ranking and map-based forecast view.
- Resource planning charts for RDT kits, ACT doses, and bed nets.

## Tech Stack

- Vite
- HTML, Tailwind CSS (CDN mode), vanilla JavaScript
- Chart.js
- Leaflet

## Dataset Format

The CSV is expected to contain these columns:

- ds
- district
- cases
- RDT Kits
- ACT Doses
- Bed Nets
- Rainfall_mm
- Humidity_%
- Temperature_C

Sample file included in this repository:

- malaria_synthetic_dataset.csv

## Local Development

### Prerequisites

- Node.js 18+ (recommended)
- npm

### Install

```bash
npm install
```

### Run Development Server

```bash
npm run dev
```

Open the URL printed in the terminal (usually http://localhost:3000 or next available port).

### Build for Production

```bash
npm run build
```

### Preview Production Build

```bash
npm run preview
```

## End-to-End Usage Flow

1. Log in to the dashboard.
2. Start on Upload & Preview.
3. Upload your CSV or load the sample dataset.
4. Confirm summary and table preview.
5. Go to Train & Forecast and run model simulation.
6. Inspect Trend Analysis, District Map, and Resource Allocation pages.

## Notes

- This version uses a forecast simulation strategy from uploaded historical patterns and climate signals.
- Tailwind directives in inline style blocks are processed at runtime in browser CDN mode.

## Repository Structure

- index.html: Main single-page application.
- malaria_synthetic_dataset.csv: Sample input dataset.
- package.json: Scripts and dependencies.
- vite.config.ts: Vite configuration.

## License

For internal/demo use unless otherwise specified.

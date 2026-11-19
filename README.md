# Demand Forecaster

A browser-based demand forecasting tool. No install, no server, no build step.

## Features
- Upload an Excel (.xlsx/.xls) or CSV file, paste data, or type demand manually in the entry table (first sheet is read; last numeric column = demand, first column = period name)
- Methods: Simple average, Exponential smoothing, Trend-adjusted (Holt), Seasonal trend-adjusted (Holt-Winters, multiplicative or additive)
- Adjustable alpha (smoothness/responsiveness), beta (trend), gamma (seasonality) and season length
- Auto-optimise parameters (lowest MSE), error metrics (MAD, MAPE, MSE, bias, tracking signal), method comparison, chart, CSV download

## Run locally
Open `index.html` in any browser. Try `sample-data.csv`.

## Publish on GitHub Pages
1. Create a new repository on GitHub.
2. Upload `index.html`, `xlsx.full.min.js` (Excel reader), `README.md` and `sample-data.csv`.
3. Settings > Pages > Source: "Deploy from a branch", Branch: `main`, folder `/ (root)`, then Save.
4. Your app will be live at `https://<username>.github.io/<repo-name>/`.

# Forest Traceability Blockchain

Expo / React Native interface for the local forest timber traceability blockchain dataset.

## Features

- Demo login: `admin` / `admin`
- Overview of registered timber, blockchain blocks, total volume and transactions
- Timber registry with species/origin filters and record details
- Blockchain ledger with block hashes and transaction references
- **Stats & Analytics terminal** inspired by financial-market data interfaces, including:
  - Species composition (pie-style distribution)
  - Timber volume histogram
  - Volume by origin bar chart
  - Registration activity line chart
  - Species-by-origin heatmap
  - GPS coordinate plot of registered timber
  - Timber records data table
- **Forecasting terminal** with selectable 3-, 6- and 12-month horizons:
  - Monthly projected timber registrations (log counts)
  - Projected timber volume in cubic metres
  - Historical-versus-forecast chart and monthly forecast table
  - Linear-trend diagnostics and indicative error ranges
  - Forecasts are fitted to the latest 12 available harvest-date months; they are planning estimates, not guarantees, and do not model seasonality or external factors
- Statistics, registry data and forecast inputs are read directly from `data/forest-blockchain.json`.

## Run

```bash
npm install
npx expo start
```

For the web version:

```bash
npx expo start --web
```

The project includes `react-dom` and `react-native-web` dependencies for Expo web support.

> The `admin` / `admin` login is for demonstration only. Use a secure server-side authentication system before production deployment.

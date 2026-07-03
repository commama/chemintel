# CHEMINTEL

AI Powered Computational Drug Discovery Platform.

CHEMINTEL is a premium pharmaceutical SaaS-style web application for computational drug discovery, molecule exploration, disease intelligence, ADMET review, chemistry calculators, reaction simulation, and executive analytics.

## Stack

- React + Vite
- Tailwind CSS
- Framer Motion
- React Router
- Lucide React
- 3Dmol.js
- Chart.js
- Node.js + Express
- SQLite through Node's built-in `node:sqlite` module
- PubChem API
- OpenFDA API

## Run Locally

```bash
pnpm install
pnpm --dir frontend install
pnpm --dir backend install
pnpm run dev
```

Frontend: http://localhost:5173  
Backend: http://localhost:4000

## Useful Scripts

```bash
npm run client
npm run server
npm run build
npm start
```

## Project Structure

```text
chemintel/
  backend/
    src/
      data/
      routes/
      services/
      db.js
      server.js
  frontend/
    src/
      components/
      data/
      pages/
      services/
      App.jsx
      main.jsx
```

## Notes

Drug search uses PubChem first and enriches medical safety data from OpenFDA when available. The backend includes a realistic SQLite seed database so the platform remains useful even when external APIs rate-limit or return incomplete data. Use Node 22 or newer for the built-in SQLite module.

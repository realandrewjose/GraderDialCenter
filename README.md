# Symposium Research Grading App

This project is a React application bootstrapped with Vite and styled with Tailwind CSS. It provides a grading interface for public speaking assignments. On launch you'll see a dashboard with cards for the Symposium Research Assignment, Informative Speech, Persuasive Speech, and Introductory Speech; selecting a card opens the grader for that assignment.

## Available Scripts

Install dependencies:

```bash
npm install
```

Start development server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Preview production build:

```bash
npm run preview
```

## Tailwind CSS

Tailwind is configured via `tailwind.config.js` and `postcss.config.js`. The styles entry point is `src/style.css`.

## Notes

React and React DOM are included along with `@vitejs/plugin-react`. The main entry is `src/main.jsx` which renders the `App` component.

## Running as a Local Web App

This repository is a Vite‑powered React application that can run entirely in the browser.

### Development

1. Install dependencies (first time):
   ```bash
   npm install
   ```
2. Start the dev server:
   ```bash
   npm run dev
   ```
3. Open your browser at `http://localhost:5173/`.

   > **Do not** open `index.html` directly with the `file://` protocol – the app relies on
   > ES modules and will only work when served over HTTP.

The development server supports hot module reloading, so changes are reflected automatically.

### Production Build

Generate static assets with:

```bash
npm run build
```

This creates a `dist/` folder containing `index.html` and an `assets/` subdirectory.

You can serve it locally using any static file server, for example:

```bash
# using the `serve` package
npx serve dist

# or with Python
python -m http.server --directory dist 3000
```

Then visit `http://localhost:3000` (or the port you chose) to use the app.

### Deployment

The contents of the `dist/` directory are static and can be deployed to any
hosting provider that serves static files (GitHub Pages, Netlify, Vercel, etc.).

> Tip: Configure your host to redirect all 404s to `index.html` if you plan to add
> client‑side routing in the future.

This setup keeps the project simple and focused on the web; no Electron
dependencies are required anymore.


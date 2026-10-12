# PortfolioLens — React Portfolio Analyzer

A responsive React/Vite workspace built from the supplied webdevelopment project. It adds a sign-in screen, a profile dashboard, searchable analytics cards, a profile-visibility toggle, responsive navigation, and sign-out. Existing LeetCode, Codeforces, GitPulse, and Ask Gemini pages are preserved in `public/tools` and opened inside the React workspace to retain their current behavior while allowing incremental component-by-component migration.

## Run locally

1. Install Node.js (LTS).
2. Open this folder in VS Code.
3. In the terminal run:
   ```bash
   npm install
   npm run dev
   ```
4. Open the local URL Vite prints (normally `http://localhost:5173`).

To create a production build: `npm run build`.

## Important authentication note

The login page is a front-end demo only. It accepts any valid email and a non-empty password; it does not authenticate an account or securely protect data. For real users, connect an Express backend and database, hash passwords, validate sessions/tokens server-side, and protect API routes. Never store real passwords in local storage.

## Structure

- `src/main.jsx` — React login, navigation, profile dashboard and analytics workspace.
- `src/style.css` — responsive dark theme and login/dashboard styling.
- `public/tools/` — original analytics pages and profile images preserved for compatibility.

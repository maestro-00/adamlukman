# AGENTS.md

## Cursor Cloud specific instructions

This repository is a single-page React portfolio site built with Vite and Tailwind CSS. There is no backend or database — everything runs client-side.

### Services

- Frontend (Vite dev server): `npm run dev` serves the app at `http://localhost:5173`. Use `npm run dev -- --host` to expose it on the network interface.

### Common commands (see `package.json`)

- Dev server: `npm run dev`
- Lint: `npm run lint` (currently reports pre-existing errors/warnings in `src/`; do not treat a non-zero exit as an environment problem)
- Production build: `npm run build` (outputs to `dist/`)
- Preview production build: `npm run preview`

### Notes

- Node 22 works fine; dependencies are installed with plain `npm install` (lockfile is `package-lock.json`).
- The contact form uses EmailJS with hardcoded service/template/public keys in `src/components/Contact.jsx`. No environment variables are required to run the app. Actually submitting the form makes a live EmailJS API call, so avoid real submissions during testing.

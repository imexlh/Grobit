# grobit — grow habit

A responsive browser-based habit garden prototype using HTML, CSS, and JavaScript. The Grobit mascot is in `public/assets/grobit-mascot.png`.

## Run locally
1. Install Node.js LTS: https://nodejs.org/
2. Open a terminal in this folder.
3. Run `npm install`
4. Run `npm run dev`
5. Open the local URL printed by Vite (usually http://localhost:5173).

## Production build
Run `npm run build`. Vite writes the production site to `dist/`.

## Deploy to Vercel with GitHub
1. Create a repository on GitHub and upload the contents of this project.
2. In Vercel select **Add New → Project**, import the GitHub repository, and deploy.
3. Framework preset: **Vite**; build command `npm run build`; output directory `dist`.

## Working demo features
- Add and delete habits; mark each complete once per day.
- Points, seeds, level progression and visual plant stages.
- Demo shop with seed purchases and owned items.
- Edit profile name and reset demo data.
- Data persists in the current browser using `localStorage`.

## Not implemented yet
Real accounts, password authentication, cloud database/sync, payments, and ad integration. This is a front-end prototype, not a secure account system. Local data is not shared across devices.

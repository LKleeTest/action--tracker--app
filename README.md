# Meeting Action Tracker

A single-page app for tracking the actions agreed in meetings, so nothing gets forgotten.

- Add an action with an owner and a due date
- Actions are grouped by owner, with a tick box to mark each one done
- Open, done and overdue counts at the top; overdue actions are highlighted in red
- Data is saved in the browser's `localStorage` (each browser keeps its own list)

Everything lives in `index.html` with no build step and no external dependencies.

## Deploy to Vercel

1. Go to [vercel.com/new](https://vercel.com/new) and import this GitHub repository.
2. Leave the settings as they are:
   - **Framework Preset:** Other
   - **Build Command:** leave empty
   - **Output Directory:** leave empty (the repo root is served)
3. Click **Deploy**. Vercel serves `index.html` at your project URL.

Every push to `main` redeploys automatically. `vercel.json` adds clean URLs and a few security and caching headers.

### Or with the Vercel CLI

```bash
npm i -g vercel
vercel        # preview deploy
vercel --prod # production deploy
```

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

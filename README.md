# Focus Grove

**A little space to do what matters.**

Focus Grove is a calm, accessible focus companion for adults, children, and grandparents. Each mode adjusts the language, suggested session lengths, and reading comfort while keeping the core experience familiar.

## Features

- Three modes: Adults, Kids, and Grandparents
- Focus timer with start, pause, resume, and reset
- Mode-specific timer presets and encouraging messages
- Separate task lists for each mode
- Daily focus totals and a seven-day progress overview
- Optional completion chime (off by default)
- Responsive layout, keyboard focus states, semantic controls, and reduced-motion support
- Local-first storage: tasks and session history stay in the current browser
- No account, analytics, server, third-party JavaScript, external fonts, or dependencies required

## Run locally

Open `index.html` in a modern browser. For a local server, run:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Checks

With Node.js 18 or newer:

```bash
npm run check
npm test
```

These smoke checks cover essential structure and project behavior; they are not a substitute for comprehensive browser end-to-end testing.

## Deploy with GitHub Pages

The repository includes a GitHub Actions workflow that publishes the static website to GitHub Pages whenever changes are pushed to `main`. In the repository, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions** if it is not already selected. Once the workflow finishes, the public site should be available at:

https://ngaurav951.github.io/focus-grove/

## Privacy and limitations

All tasks and session history are saved in the browser's local storage; they are not uploaded to a server. Clearing browser data clears those records. The timer uses browser timing and is intended for everyday focus sessions, not precision timing. Kids mode is a supportive focus aid, not parental-control software. Focus Grove is a productivity tool, not a medical or diagnostic application.

## Project files

- `index.html` — accessible page structure
- `styles.css` — visual system and responsive layouts
- `app.js` — timer, tasks, progress, and local persistence
- `favicon.svg` — matching leaf mark
- `tests/smoke-check.mjs` — dependency-free structural smoke checks
- `.github/workflows/pages.yml` — GitHub Pages deployment

## License

MIT. See [LICENSE](LICENSE).

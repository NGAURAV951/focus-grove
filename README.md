# Focus Grove

**A little space to do what matters.**

Focus Grove is a calm, accessible focus companion made for adults, children, and grandparents. It adapts session lengths, language, and reading comfort for each mode without asking people to learn a different app.

## What it does

- **Three modes:** Adults, Kids, and Grandparents, each with its own suggested timer lengths and language.
- **Focus timer:** Start, pause, resume, and reset sessions.
- **Personal task lists:** Add, finish, and remove tasks. Lists are separate for each mode.
- **Progress overview:** Today’s completed focus minutes, finished sessions, and a rolling seven-day chart.
- **Optional completion chime:** Off until enabled.
- **Accessible by design:** Responsive layout, keyboard focus states, clear labels, and reduced-motion support.
- **Local-first privacy:** Task lists and completed sessions stay in the browser's local storage. No account, analytics, database, or third-party scripts.

## Run locally

Open `index.html` in any modern browser. No installation or build step is needed.

For a local server, run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

This repository includes a GitHub Actions workflow at `.github/workflows/pages.yml`. It deploys the static app whenever a commit is pushed to `main`.

If the workflow reports that Pages is not enabled, open **Settings → Pages** and select **GitHub Actions** under **Build and deployment → Source**. The site URL is:

**https://ngaurav951.github.io/focus-grove/**

Monitor deployment progress in the [Actions tab](https://github.com/NGAURAV951/focus-grove/actions).

## Project structure

```text
focus-grove/
├── index.html                 # Complete app (HTML, CSS, and JavaScript)
├── README.md                  # Setup and project documentation
├── LICENSE                    # MIT license
└── .github/workflows/pages.yml # Automatic Pages deployment
```

Keeping the first version in a single HTML file makes it easy to host, inspect, and modify without a package manager or framework.

## Privacy and limitations

Tasks and session history are stored in the current browser only; they are not synced between devices. Clearing browser data removes those records. Browser timers may be throttled when a tab is in the background, so this is intended for everyday focus sessions, not precision timing. Kids mode is a supportive focus aid, not parental-control software. Focus Grove is a productivity tool, not a medical or diagnostic application.

## License

MIT. See [LICENSE](LICENSE).

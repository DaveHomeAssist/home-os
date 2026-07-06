# Home OS

The family-facing front door for the Robertson household's Notion workspace, live at **[davehomeassist.github.io/home-os](https://davehomeassist.github.io/home-os/)**. It's a static single-page dashboard that routes family members to the right Notion page — it doesn't hold any data itself.

## What it is

Home OS is a **navigation facade, not a system of record**. The household's real data (tasks, projects, recipes, maintenance, budgets, etc.) lives in Notion databases. This site exists so that a family member can open one calm, searchable page and get pointed to the right destination without needing to understand the Notion workspace's back-end structure.

## What's here

| Path | What it is |
|---|---|
| `index.html` | The entire app — markup, styling, and vanilla JS in one file. No build step, no dependencies. |
| `favicon.svg` | Browser tab icon. |

### What the page does

- **Route directory** — primary routes, family hubs, reference indexes, and admin surfaces are rendered from small JS arrays (`primaryRoutes`, `hubs`, `references`, `adminLinks`), each linking out to a Notion page.
- **Search + filter** — a search box and kind filters (`All` / `Routes` / `Hubs` / `Refs` / `Admin`) narrow the visible cards client-side.
- **Anticipatory UX** — a `localStorage`-backed store (`homeos` key) tracks visit frecency, recent searches, and last-used filter/search, and drives a time-of-day greeting with a suggested next action.
- **Operating model section** — documents which layer owns what (Home OS vs. `05 | Home & Family` vs. the Notion databases vs. REF pages) so ownership boundaries stay explicit as the workspace grows.

## How to run it

There's no build step or dependencies — it's a static HTML file.

- **Locally:** open `index.html` directly in a browser, or serve the folder with any static file server (e.g. `npx serve .`).
- **Live:** the `main` branch is published via GitHub Pages at [davehomeassist.github.io/home-os](https://davehomeassist.github.io/home-os/).

## Conventions

- All content lives inline in `index.html` as plain JS data arrays — to add or change a route/hub/reference/admin link, edit the corresponding array in the `<script>` block rather than the DOM.
- Home OS should stay a **pointer layer**. Don't let it grow into a duplicate of the canonical Notion databases it links to — see the "Operating model and ownership" section on the page itself for the current ownership boundaries.

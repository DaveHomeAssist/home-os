# Home OS — User Guide

Home OS is the front door to the household's Notion setup: **[davehomeassist.github.io/home-os](https://davehomeassist.github.io/home-os/)**. Use it when you know roughly what you need but not which Notion page it lives on.

## Getting around

- **Greeting bar** — at the top, a time-of-day greeting suggests one thing to open next (your Family Inbox in the morning, the Dashboard midday, Food & Cooking in the evening). Once you've used the site a few times, it switches to suggesting whatever you actually visit most.
- **Quick resume** — below the greeting, your most-visited links show up as chips so you can jump straight back to them.
- **Search** — type in the search box to filter every route, hub, reference, and admin surface by title/description. Your last few searches are remembered as quick-pick chips.
- **Filters** — use the `All / Routes / Hubs / Refs / Admin` buttons to narrow the page to one category.
- **Jump links** — use the nav row to skip straight to a section (Front door, Family hubs, Reference index, Operating model, Roadmap).

## The four sections

| Section | What it's for |
|---|---|
| **The front door** | Everyday entry points — Start, Dashboard, Mom Home, Family Inbox, Family Projects, Food & Cooking. |
| **The household atlas** | All family hubs (Calendar, Finance, Health, Vehicles, Yard, etc.) — pick a domain to jump into. |
| **Pointers, not duplicates** | Reference index pages (Books, Games, Places, Services, etc.) that point into the canonical Notion systems. |
| **Operating model** | Explains what Home OS owns vs. what lives deeper in Notion, plus admin-only links (Systems, Templates, Config, Archive). |

## Things to know

- Every card opens the underlying **Notion page** in a new tab — Home OS itself doesn't store any household data.
- Your recent searches, visit history, and last-used filter are saved **only in your own browser** (`localStorage`), not shared across devices or family members.
- If a link looks wrong or a hub is missing, it should be added/fixed in `DB | 103 | Fam Hubs` in Notion (the source of truth) and then mirrored here — see the main `README.md` for where that lives in the code.

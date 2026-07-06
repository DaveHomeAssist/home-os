# Changelog

All notable changes to Home OS, grouped by date.

## 2026-07-06
- Added an explicit all-rights-reserved LICENSE.

## 2026-06-20
- Added a site favicon and linked it from the page `<head>`.

## 2026-04-18
- Fixed `saveStore` to dispatch a `homeos:storage-error` event on `localStorage` quota failure instead of silently swallowing the exception.

## 2026-03-31
- **Initial commit** — Home OS family operations dashboard: route/hub/reference/admin directory, search, kind filters, and the operating-model/ownership documentation section.
- Added tactile microinteraction feedback across interactive surfaces (counter pulse on visible-count change, staggered card reveal on filter/search).
- Added anticipatory UX: `localStorage`-backed frecency tracking of visited links, a time-of-day contextual greeting with a suggested next action, a "quick resume" recent-links row, search-term recollection, persisted filter/search state across sessions, and a time-and-day-aware search placeholder hint.

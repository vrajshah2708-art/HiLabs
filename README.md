# MCheck® Handoff: working prototype

A clickable, single-file prototype of the case management workbench MVP from the HiLabs APM product case (2026–27). Open `index.html` in any modern browser. It has no build step and needs no server. Fonts load from Google Fonts; without a connection it falls back to system fonts.

All members, numbers, providers and the health plan are fictional. The data is taken from the annex workbook (Queue (48), Patient cards, Data inventory, Recipes, Clocks, Imperfections log, Assessment (40 fields), Time model).

## What's inside

| Screen | Deck slide | What you can do |
|---|---|---|
| Queue | 7 | Live ED timer for Dwayne in the NOW lane; scheduled lane for Rosa; ranked queue of the 48-member caseload with "Why" score breakdowns (U × I/5 × A); filter and search; clock-load spike with supervisor rebalance |
| Member handoff | 8 | I-PASS layout for all 5 annex members: severity (Maria only), AI-read facts to confirm, timeline, labs with arrival lag, med-list diff, ordered actions, situation awareness, identity split (Rosa), Part 2 gating (Andre) |
| Call & confirm | 9 | Rosa's 15:42 call: 5 bundled items, all 40 assessment fields (31 pre-filled with source, 9 judgment), note draft whose brackets fill as you answer, write-back on save |
| Flag review | 10 | Gloria's "right member, wrong problem": accept (adds 3 tasks) or keep the flag (override reason captured) |
| Data & trust | 4–5, 10 | 28 datasets by decision, 16 recipes, expectation clocks, trust model, AI responsibility matrix, 27 planted imperfections |
| Impact & pilot | 2, 11–12 | Live time model: drag the inputs to recompute the 48 blocks, conversations per day, overhead per conversation and value ÷ price |

The guided tour runs through Maria's Monday in 23 steps. Each step is mapped to a slide and callout pin.

Every confirmation lands in the **write-back record** (database icon, bottom left of the sidebar). Hover any trust chip to see its source, freshness and rule.

## Shortcuts

`1`–`6` switch screens · `Ctrl/⌘ K` search · `T` tour · `←/→` tour steps · `J/K` move in the queue · `D` dark mode · `?` help

Add `?tour=1` to the URL to start the tour directly, or `?welcome=1` to show the welcome screen again.

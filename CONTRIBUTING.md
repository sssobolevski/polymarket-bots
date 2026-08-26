# Contributing

Additions are welcome. This list is curated the same way the [POLBOTS](https://polbots.com) catalog is: every entry is checked by hand before it appears, and entries that fail the checks are declined with the evidence.

## What qualifies

- **A working product** — a bot, platform or tool for trading on Polymarket that can actually be run or used today. Waitlists, concepts and pricing pages with nothing behind them do not qualify yet; resubmit when it ships.
- **A real website, repo or Telegram bot** that you control.
- **An honest one-line description** of what it does — no "guaranteed profit", no invented performance or rating numbers.

## How to add a bot

Open a PR adding one line to the section matching the bot's primary strategy, keeping the alphabetical order:

```
- [Name](https://example.com) — What it does, in one sentence.
```

Note that `README.md` is generated from the POLBOTS catalog data. Before merging, we port your entry into the catalog — which runs it through the checks below and also gives the bot its own review page — and the next regeneration includes it. Your PR is the submission; you'll get either a merge or the evidence for a decline.

## The checks we run

All from the outside — no account or purchase needed, so you can repeat them yourself:

1. **CTA targets.** Every link behind "Launch / Choose plan / Docs / Dashboard" must lead to a real page, not an in-page anchor like `/#how`.
2. **Paths and subdomains.** `/login`, `/docs`, `app.`, `api.` — something must answer that looks like the product, not a wildcard stub.
3. **Structured data vs reality.** An `aggregateRating` requires a review mechanism that actually exists; `og:image` must resolve; numbers duplicated across sister sites are fabricated.
4. **Wayback + whois.** Registration date, first snapshot and the story on the page must agree; a template whose title names a different brand is a decline.
5. **Socials.** Linked Telegram / X accounts must be alive and actually belong to the project.
6. **Press releases.** Paid PR-wire "launch" posts that have since been withdrawn count against, not for.
7. **Open-source repos.** The repo must contain the bot, not a scaffold with an inflated README — real strategy code, real API calls, a commit history that matches the claims.

## Removals

If a listed bot dies, rugs, or turns out to fail these checks, open an issue with what you found — removals are as welcome as additions.

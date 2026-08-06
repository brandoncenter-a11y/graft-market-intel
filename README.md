# Graft — Market Intelligence

The living map of Graft's ecosystem: competitors, adjacent companies, infrastructure,
nonprofits, and investors in the US kidney-transplant market. Kept in its own repo (out of
the product code) and **refreshed weekly by an automated cloud agent**.

## What's here

- **[`ecosystem-players.md`](ecosystem-players.md)** — the canonical roster. Read the
  **Change Log at the top first**: each weekly refresh logs new entrants, funding rounds,
  M&A, and material changes there, then updates the roster below.

## How the weekly refresh works

A scheduled Claude Code cloud agent runs every **Monday 08:00 America/Chicago**. It:

1. Clones this repo.
2. Re-runs the tracked search queries in `ecosystem-players.md` → *Watchlist & weekly-refresh queries*.
3. Diffs what it finds against the current roster.
4. Adds a dated block to the **Change Log** for anything new/changed (tagged `[NEW]`,
   `[FUNDING]`, `[M&A]`, `[CHANGE]`) and updates the relevant roster rows.
5. Opens a **pull request** titled `Weekly ecosystem refresh — <date>` for review. If nothing
   material changed that week, it says so in the PR body rather than inventing churn.

Review the PR diff to see exactly who's new. Merge to accept.

## Standing tags

🔴 Direct competitor · 🟠 Partial overlap / could encroach · 🟡 Adjacent (channel / partner /
acquirer) · 🟢 Infrastructure / nonprofit · 💰 Investor / capital.

## Sources & confidence

Claims are sourced in the roster. Figures marked *(unverified)* are third-party estimates or
undated — don't cite an unverified funding round without a fresh press release. A browsable
version of this map is published as a private Claude artifact.

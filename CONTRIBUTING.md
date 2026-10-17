# Contributing

Thanks for helping. This list stays useful only if every entry is real, current and honestly described.

## What gets in

1. The repo is **public** and **not archived**.
2. It has **a license**.
3. It has had **a commit in the last 12 months**.
4. It fits this list: open-source libraries, bots, backtesters, data tools and AI agents for trading stocks, futures, forex and crypto.
5. It does something you can show in the README. No empty shells, no "coming soon".
6. It is **not a copy** of another repo on the list.
7. No affiliate or tracking links.

Owners may add their own project. It is judged by the same rules. Mark it with "(by the author)" in the description.

## How to add a repo

1. Fork this repo.
2. Add **one** object to `data/entries.json`:
   ```json
   {
     "repo": "owner/name",
     "category": "framework",
     "description": "One plain sentence. What it does. Say if it needs paid keys.",
     "license": "MIT",
     "verified": "YYYY-MM-DD",
     "last_commit": "YYYY-MM-DD"
   }
   ```
   Categories: `framework`, `backtest`, `exchange`, `data`, `ta`, `portfolio`, `ml`, `platform`, `defi`.
3. Run `python scripts/build_readme.py`. Do not edit `README.md` by hand.
4. Open a pull request using the template. One entry per PR.

## Writing the description

- Plain words. Short. One sentence, two at most.
- Say what it does, not how great it is. No "best", "powerful", "revolutionary".
- If it needs paid keys or a paid plan, say so.
- If the claims are unproven, do not repeat them as facts.

## Removing or fixing entries

A weekly check (GitHub Action) opens an issue when a listed repo is archived, renamed, missing or has no commits for a year. Maintainers remove or fix those. You can also open a PR to remove a dead entry.

## Changelog

Add a line to `CHANGELOG.md` under "Unreleased" for each change.

# STATUS — jarrenchang

**Last updated:** 2026-11-11

## One-line description
Jarren Chang's personal site — a placeholder front page plus a beginner's guide (`/howto`) so he can run the site himself.

## Scope / positioning
- Per README: "The point of this repo isn't the site — it's that Jarren can run it himself."
- Front page is a placeholder: a list of ideas for what to add, links to other family sites, and a promise to transfer the domain and hosting to him.
- `/howto` is an operator's manual written for someone who has never used a terminal.

## Stack & hosting
- Static HTML + one stylesheet (`assets/site.css`); no build step, no `package.json`.
- Light/dark theme toggle saved in localStorage.
- GitHub Pages branch deploy from `thirstypig/jarrenchang`; push to `main` publishes.
- DNS at Squarespace: apex A/AAAA records to GitHub Pages, `www` CNAME to `thirstypig.github.io`.
- No CI workflows, tests or CLAUDE.md in repo.

## URLs
- https://jarrenchang.com
- https://jarrenchang.com/howto/

## Shipped (last 60 days)
- Nothing in the window. Last commit: 2026-07-31 (all 6 commits are from that day).

## In progress
- None recorded.

## Open bugs / known issues
- None recorded.
- Warning in README: when the site moves to a GitHub Actions build, `CNAME` must end up in the build output, or each deploy silently drops the custom domain.

## Next phases (in order)
- README mentions a planned move to Astro (dev server on port 3140). No date or order recorded.
- Content is up to Jarren; the front page lists ideas, not a plan.

## Decisions changed recently
- 2026-07-31: switched to UW colours and modern type, alongside adding the operator's manual.
- No changes since.

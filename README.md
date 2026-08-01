# jarrenchang.com

Jarren Chang's personal site. Static, hosted free on GitHub Pages.

The point of this repo isn't the site — it's that Jarren can run it himself.
`/howto` is the guide that teaches him how, written for someone who has never
used a terminal.

## Where things are

| Path | What it is |
|------|------------|
| `index.html` | The front page. Placeholder for now. |
| `CNAME` | Tells GitHub which domain to serve. **Don't delete this.** |

## How it gets published

Push to `main` → GitHub Pages publishes it → live at https://jarrenchang.com
within a minute or so. There is no build step yet.

## Local preview

No install needed — open `index.html` in a browser.

Once this moves to Astro, the dev server runs on **port 3140** (assigned in the
workspace port registry; don't pick a different one).

## Domain

| | |
|---|---|
| Registrar / DNS | Squarespace |
| Host | GitHub Pages, `thirstypig/jarrenchang` |
| Apex records | 4× `A` → `185.199.108–111.153`, 4× `AAAA` → `2606:50c0:8000–8003::153` |
| `www` | `CNAME` → `thirstypig.github.io` |

⚠️ When this repo moves to a GitHub Actions build, `CNAME` must end up in the
build output or **every deploy silently drops the custom domain** and the site
reverts to `thirstypig.github.io/jarrenchang`. Actions-based deploys don't
restore it the way branch deploys do.

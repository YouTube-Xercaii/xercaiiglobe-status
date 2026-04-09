# XercaiiGlobe — status & incident updates

Public notices when **XercaiiGlobe** (website or API) is down, degraded, or undergoing maintenance.  
This repo has **no application code** — only **[GitHub Releases](https://github.com/YouTube-Xercaii/xercaiiglobe-status/releases)** used as a simple, CDN-friendly feed.

## Who this is for

- **Players / developers** on the site: during deploys or outages, the **“Server is restarting”** screen can load updates from here even when Render is unavailable.
- **Xercaii/Isaiah (operator):** post a release in a minute — no need for the main API or web app to be up.

## How to post an update

1. Open **[Releases](https://github.com/YouTube-Xercaii/xercaiiglobe-status/releases)** → **Draft a new release**.
2. **Choose a tag** — any unique name is fine, e.g. `2026-04-09-outage`, `deploy-api`, `incident-001`. Create the tag on `main` (or your default branch) when prompted.
3. **Release title** — short headline users see in the list (e.g. *“API maintenance — ~30 min”*).
4. **Describe this release** — use **Markdown**: what happened, ETA, workarounds, links. Tables and lists render on the site.
5. **Publish release**.

The newest release appears first. The live site polls this feed periodically while someone has **Notifications & updates** expanded.

## Tips

- Prefer **clear ETAs** and **what still works** (e.g. “Globe read-only”, “Auth down”).
- You can publish **pre-releases** for drafts; the public API usually returns them too — if you want something hidden from the default list, use a private note elsewhere until you’re ready to publish.
- Very old entries fall off the **latest five** in the UI; older posts remain on GitHub under **Releases**.

## Related repos

- **Website / API changelog** (deploy & product notes) may live in another public repo — see your main **XercaiiGlobe** web project env (`NEXT_PUBLIC_WEBSITE_API_CHANGELOG_*`).
- **Source code** for the app is **not** in this repository.

---

*Repository: [YouTube-Xercaii/xercaiiglobe-status](https://github.com/YouTube-Xercaii/xercaiiglobe-status)*

# XercaiiGlobe — status & incident updates

Public notices when **XercaiiGlobe** (website or API) is down, degraded, or undergoing maintenance.  
This repo has **no application code** — only **[GitHub Releases](https://github.com/YouTube-Xercaii/xercaiiglobe-status/releases)** used as a simple, CDN-friendly feed.

## For developers

Releases are fetched via the **public GitHub REST API** (no auth required for this repo). The **XercaiiGlobe** web app reads them during the service-health / outage overlay (**Notifications & updates**) so users can see incident copy even when your own hosting or API is unreachable.

- Default API URL pattern: `https://api.github.com/repos/YouTube-Xercaii/xercaiiglobe-status/releases?per_page=5`
- Override in the web app with `NEXT_PUBLIC_STATUS_NOTIFICATIONS_RELEASES_URL` if the feed moves (see `githubChangelog.ts` / `.env.example` in **xercaiiglobe-web**).
- Human-facing Releases page: same repo’s GitHub **Releases** tab (`NEXT_PUBLIC_STATUS_NOTIFICATIONS_GITHUB_URL` if overridden).
- The UI typically shows the **latest five** releases; ordering follows GitHub’s API (newest first). Markdown in release bodies is rendered on the client.

## Related

- **Website / API changelog** (product / deploy notes) is a **separate** public repo and env keys (`NEXT_PUBLIC_WEBSITE_API_CHANGELOG_*` in **xercaiiglobe-web**).
- Application **source code** lives in the main monorepo / web project — not here.

---

*Repository: [YouTube-Xercaii/xercaiiglobe-status](https://github.com/YouTube-Xercaii/xercaiiglobe-status)*

# FFC-EX-facinggiantsnc.org

Facing Giants Inc — FFC-supported charity website (static, GitHub Pages).

This repository holds a fully localized static capture of the former WordPress site at
`facinggiantsnc.org` (previously hosted on Hostinger), migrated as part of the FFC
Wave-1 WordPress-to-Pages program
([FFC-Cloudflare-Automation#702](https://github.com/FreeForCharity/FFC-Cloudflare-Automation/issues/702)).

## Hosting

- Deployed to GitHub Pages on the default URL:
  <https://freeforcharity.github.io/FFC-EX-facinggiantsnc.org/>
- Deployment runs from `.github/workflows/static.yml` on every push to `main`.
- No custom domain and no DNS changes are configured at this stage.

## Structure

Plain static HTML capture — no build step. Pages:

| Path | Page |
| --- | --- |
| `/` | Home |
| `/aboutus/` | About Us |
| `/community-focus-areas/` | Community Focus Areas |
| `/fg-intiatives/` | FG Initiatives |
| `/get-involved/` | Get Involved |

All CSS/JS/fonts/images are served from this repository (external font and analytics
hosts were localized or stripped during migration). Third-party iframe embeds
(YouTube, Facebook video, Google Forms) are retained intentionally.

## Maintenance

- Edit the HTML in place; every push to `main` redeploys.
- `linkcheck.yml` runs lychee weekly and on pushes/PRs to catch link rot.
- See the migration tracking issue in this repo for what was captured, stripped,
  and flagged during the WordPress-to-static conversion.

---

Supported by [Free For Charity](https://freeforcharity.org).

# security-toolkit

Two small security tools, live on blurxy.net:

- **OSINT Field Kit**: https://blurxy.net/osint/ (a curated, searchable launchpad of OSINT tools with a case notebook and report export)
- **KEV Watch**: https://blurxy.net/kev/ (CISA's Known Exploited Vulnerabilities catalog as an ops board, with EPSS scores)

Built by Rafiul Bari ([blurxy.net](https://blurxy.net)). Split out of [`blurxy/blurxy.net`](https://github.com/blurxy/blurxy.net) (then named `blurxy-worldcup26`) on 2026-11-15 with each tool's history. A merged single app is planned at blurxy.net/toolkit/.

Deploy: a Cloudflare Worker serving `public/` on the `blurxy.net/osint*` and `blurxy.net/kev*` routes (`wrangler.jsonc`). Every push to `main` deploys automatically through Cloudflare Workers Builds (`npx wrangler deploy`).

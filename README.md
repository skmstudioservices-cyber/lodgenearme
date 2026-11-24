# lodgenearme

Static near-me site — **Lodges Near Me — Find Nearby, Free Map**.

- Live: https://lodgenearme.pages.dev
- Cloudflare Pages project: `lodgenearme`
- Sitemap: https://lodgenearme.pages.dev/sitemap.xml

## Deploy

Static files at the repo root. Two paths:

1. `.github/workflows/deploy.yml` — on push to `main`, needs
   `CLOUDFLARE_API_TOKEN` + `CLOUDFLARE_ACCOUNT_ID` as repo secrets.
2. **Network bridge** — `net-deploy-queue.yml` in `digipincode-india`
   deploys this repo to the `lodgenearme` Pages project using that repo's
   secrets. Push `deploy-queue/lodgenearme.json` there to trigger it.

## Rules

- One repo per site. This repo owns only `lodgenearme`.
- Never copy another site's data or branding here.
- Keep the host in `sitemap.xml` and `robots.txt` correct.

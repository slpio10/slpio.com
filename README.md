# Sleep Calculator — slpio10.github.io


A free, single-page sleep cycle calculator (plus BMI, calorie, water intake, and age calculators), built with plain HTML/CSS/JS — no build step, no dependencies, no backend.

## Deploy to GitHub Pages with your domain (slpio10.github.io)


1. Push all these files to a GitHub repo (root of the repo, not a subfolder).
2. Go to **Settings → Pages** in the repo.
3. Under "Build and deployment", set **Source: Deploy from a branch**, branch: `main`, folder: `/ (root)`. Save.
4. Under "Custom domain", enter `slpio10.github.io
` and save (GitHub will detect the `CNAME` file already included here).
5. At your domain registrar (wherever you bought slpio10.github.io), add these DNS records:
   - **A records** pointing `@` to GitHub Pages' IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - **CNAME record**: `www` → `YOUR-GITHUB-USERNAME.github.io`
6. Back in GitHub Pages settings, check **Enforce HTTPS** once it becomes available (can take up to 24 hours for DNS + certificate).

Once DNS propagates, your site will be live at `https://slpio10.github.io/slpio.com`.

## Files

- `index.html` — the entire site (calculator + about/contact/privacy/terms/disclaimer content, all self-contained)
- `CNAME` — tells GitHub Pages to serve this repo at slpio10.github.io
- `robots.txt` — search engine crawling rules
- `sitemap.xml` — sitemap for search engines

## Notes

- No API keys, no environment variables, no server — it's 100% static.
- All canonical URLs, Open Graph tags, and schema markup already point to `https://slpio10.github.io/slpio.com`.
- Nothing is sent to a server — all calculators run entirely in the browser.

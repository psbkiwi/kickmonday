# Kick Monday site

Static site. No build step. Edit the HTML, push, done.

- `index.html`  the one page
- `privacy.html`  linked from the footer and cookie notice; fill in [DATE] and [LEGAL ENTITY NAME]
- `config.js`  the three booking URLs; replace the placeholders and nothing else changes
- `styles.css`, `assets/`

## Deploy (first time, about 20 minutes)

1. Create a GitHub repo named `kickmonday`, push this folder to it.
2. vercel.com, New Project, import the repo, Framework preset "Other", deploy. You get a `*.vercel.app` URL.
3. Vercel, Project Settings, Domains, add `kickmonday.com` and `www.kickmonday.com`. Vercel shows the records to add.
4. In your DNS (Cloudflare or GoDaddy), add the A record for `kickmonday.com` and the CNAME for `www`. Wait a few minutes. https is automatic.

Every later change: edit, commit, push. Live in about a minute.

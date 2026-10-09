# SEND & SCHNITZEL — website (static, Cloudflare Pages)

Files: index.html (landing) · privacy.html · terms.html (TikTok audit needs both publicly)
       media-kit.html (for sponsors) · style shared inline (no build step)

> ⚠️ SUPERSEDED: the original GitHub Pages plan below is replaced by Cloudflare Pages.
> The live instructions are in ../DOMAIN-AND-EMAIL-SETUP.md (§3 Hosting).

## Deploy now (Cloudflare)
```bash
cd site
npx wrangler login          # one time — browser → Allow
npx wrangler pages deploy . # goes live at sendandschnitzel-site.pages.dev
```

## Auto-deploy from GitHub (recommended, one-time setup)
1. Push this folder to a GitHub repo (see ../DOMAIN-AND-EMAIL-SETUP.md §3A)
2. Cloudflare dash → Workers & Pages → Pages → Connect to Git → pick the repo
   (framework: None, build command: empty, output dir: /)
3. Custom domains → add sendandschnitzel.com + www
4. Every `git push` after this updates the site automatically.

---

# OLD PLAN (GitHub Pages — obsolete, kept for reference)
1. github.com → new account/user **sendandschnitzel** (or your existing one)
2. Create a new repository named exactly: `sendandschnitzel.github.io`
   → tick "Public" → Create
3. git init && git add . && git commit -m "site live" && git push
4. Site goes live at https://sendandschnitzel.github.io within ~1 min
5. Put that URL into the TikTok developer app (privacy policy + TOS fields)

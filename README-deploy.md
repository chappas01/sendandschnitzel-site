# SEND & SCHNITZEL — website (static, GitHub Pages ready)

Files: index.html (landing) · privacy.html · terms.html (TikTok audit needs both publicly)
       media-kit.html (for sponsors) · style shared inline (no build step)

## Deploy (Ashley, ~3 min, once)
1. github.com → new account/user **sendandschnitzel** (or your existing one)
2. Create a new repository named exactly: `sendandschnitzel.github.io`
   → tick "Public" → Create
3. On this PC:
   cd site
   git init && git add . && git commit -m "site live"
   git branch -M main
   git remote add origin https://github.com/sendandschnitzel/sendandschnitzel.github.io.git
   git push -u origin main
   (GitHub will ask you to log in in the browser once — that's your click)
4. Site goes live at https://sendandschnitzel.github.io within ~1 min
5. Put that URL into the TikTok developer app (privacy policy + TOS fields)

After that the AI updates the site freely (evidence packs, media kit numbers) and you
just approve pushes.

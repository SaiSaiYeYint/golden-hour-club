# Golden Hour Club

One-file site (`index.html`): the movement explainer, plus a full-screen app mode
(Ritual, Prep, Focus, Wrap) that opens from the "Start today's Golden Hour" button.
No build step. Vercel serves `index.html` as is.

## Files
- `index.html`   the whole site (edit this)
- `vercel.json`  clean URLs and no stale caching
- `.gitignore`

## First-time setup
1. On github.com create an empty repository (e.g. `golden-hour-club`). Do not add a README.
2. In this folder:
   ```
   git remote add origin https://github.com/<your-username>/golden-hour-club.git
   git push -u origin main
   ```
3. In Vercel open the existing `golden-hour-club` project:
   Settings > Git > Connect Git Repository > pick the repo. Production branch: `main`.

From then on every push to `main` deploys to production, and every other branch gets a preview URL.

## Everyday flow
Edit `index.html`, then:
```
git add index.html
git commit -m "what changed"
git push
```
Vercel deploys in under a minute.

## Notes
- App mode opens at `/#app`, so the phone's back button leaves it.
- Progress is saved in the browser (localStorage), per device.

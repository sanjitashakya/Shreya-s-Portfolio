# Shreya Shrestha — portfolio

A one-page portfolio. Plain HTML/CSS/JS, no build step.

## Files
- `index.html` — the page (design + layout)
- `assets/stories.js` — every story (12 from Nepal Connect, 99 from The Annapurna Express). Generated, don't edit by hand.
- `assets/images/shreya.jpg` — her photo
- `scripts/update_stories.py` — re-collects her stories from both sites

## Add new stories
When Shreya publishes something new, run this from the project folder:
```bash
python scripts/update_stories.py
git add . && git commit -m "Update stories" && git push
```
Vercel updates the live site after the push.

## Things to fill in
- Email, LinkedIn and Instagram links: search `TODO` in `index.html`
- Colours: the `:root { ... }` block at the top of `index.html`
- Archive topics: the `TOPICS` list in the script at the bottom of `index.html`

## Push to GitHub
```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/<username>/shreya-portfolio.git
git push -u origin main
```

## Go live on Vercel
1. vercel.com → **Add New… → Project**
2. Import the `shreya-portfolio` repo
3. Framework preset: **Other** (no build command, output directory blank)
4. **Deploy**

## The CV
- Download file: `assets/Shreya-Shrestha-CV.pdf` (linked from the menu, top section and contact box)
- To edit it: change `cv/cv.html`, open it in Chrome, press Ctrl+P → Save as PDF (A4, margins None, background graphics on), and save over `assets/Shreya-Shrestha-CV.pdf`.

## Best work
The three "Best work" stories are set by `BEST` near the bottom of `index.html`: paste each story's link there.

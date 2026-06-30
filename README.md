# Ashwin Badamikar — Portfolio

A static HTML/CSS/JS portfolio site. No build step, no frameworks — just `index.html`, `style.css`, and `script.js`.

## Before you publish — 3 things to check

1. **Add your résumé PDF.** Drop a file named `Ashwin_Badamikar_Resume.pdf` into this same folder (same level as `index.html`). The "Résumé" buttons in the nav and Contact section already link to that exact filename.

2. **One link still needs verifying.** *Chronic Care AI*, *Diabetes Treatment AI*, *Nutrition Tutor Bot*, *Advanced Research Assistant*, and the *Web Scraping & Document Intelligence Tool* all link to confirmed real repos. *Financial Statement Data Pipeline* still points to your GitHub profile rather than a specific repo since I don't have that exact URL — swap it in once you have it.

3. **Skim the copy.** I pulled your experience, project, and skills details from our past conversations about your résumé. Double-check dates, numbers, and bullet wording against whatever you consider your most current résumé version, since you've iterated on a lot of variants.

## How to host this on GitHub Pages (free, your own URL)

**Option A — brand-new repo, using GitHub's website (no terminal needed)**

1. Go to [github.com/new](https://github.com/new).
2. Repository name: `ashwin-badamikar.github.io` (using *exactly* this pattern — `your-username.github.io` — gives you the cleanest URL, `https://ashwin-badamikar.github.io`, with zero extra config). If you'd rather keep it as a project page under a different name, see Option B's note below.
3. Make it **Public**, then click **Create repository**.
4. On the new repo's page, click **uploading an existing file**.
5. Drag in `index.html`, `style.css`, `script.js`, and your résumé PDF.
6. Click **Commit changes**.
7. Go to the repo's **Settings → Pages**. Under "Build and deployment," set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
8. Wait 1–2 minutes, then visit `https://ashwin-badamikar.github.io`. That's it — live.

**Option B — using git from your terminal**

```bash
cd path/to/this/folder
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/ashwin-badamikar/ashwin-badamikar.github.io.git
git push -u origin main
```

Then enable Pages the same way as step 7 above (Settings → Pages → Deploy from branch → `main` → `/root`).

> If you use a repo name *other* than `your-username.github.io` (e.g. `portfolio`), GitHub Pages will publish it at `https://ashwin-badamikar.github.io/portfolio/` instead — still free, just a slightly longer URL.

## Making future edits

Everything is plain HTML/CSS — no compiling. Edit `index.html` for content, `style.css` for design, `script.js` for behavior (nav toggle, scroll-reveal, project filters), then commit and push. GitHub Pages redeploys automatically within a minute or two of every push to `main`.

## Structure

- `index.html` — all page content and sections (Hero, About, Experience, Projects, Skills, Contact)
- `style.css` — design system (colors, type, layout) — see the CSS variables at the top of the file to retheme quickly
- `script.js` — nav scroll/mobile-menu behavior, scroll-triggered reveal animations, project category filters

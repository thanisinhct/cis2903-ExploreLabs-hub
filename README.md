# CIS 2903 Operating Systems – Lab Practice Hub

Interactive animations and practice terminals for the CIS 2903 labs (HCT).
**Practice only. The lab exam is done on a real Linux / Windows VM.**

```
index.html     ← home page listing every lab
.nojekyll      ← tells GitHub Pages to serve the files exactly as they are
README.md      ← this file (not shown on the website)
labs/          ← one page per lab (13 pages)
```

## Put it online with GitHub Pages (free, about 10 minutes)

1. Sign in at **https://github.com** or create a free account.
2. Click **+ → New repository**.
   - Repository name: `cis2903` (this becomes part of the web address)
   - Set it to **Public**, then click **Create repository**.
3. On the new repository page, click **uploading an existing file**.
4. Unzip `cis2903-practice-hub.zip`, open the folder and select **everything inside it**: `index.html`, `README.md`, `.nojekyll` and the `labs` folder. Drag them into the upload area.
   - `.nojekyll` is a hidden file. On Windows, turn on **View → Show → Hidden items**. On a Mac, press **Cmd + Shift + .** in Finder. If you can't see it the site still works, so don't worry.
5. Click **Commit changes** and wait for the upload to finish.
6. Go to **Settings → Pages**. Under **Build and deployment** choose:
   - Source: **Deploy from a branch**
   - Branch: **main** and folder **/ (root)**, then click **Save**.
7. Wait 1–2 minutes and refresh the page. A message appears: **"Your site is live at https://YOUR-USERNAME.github.io/cis2903/"**.
8. Share that link with students on your LMS or Teams.

> Check that `index.html` is at the **top level** of the repository, not inside another `cis2903-practice-hub` folder. If you see that extra folder, open it and upload its *contents* instead.

## Updating the site later

- **Change one lab:** open the `labs` folder in the repository, click **Add file → Upload files**, drop in the new `.html` with the **same file name**, then click **Commit changes**. The site updates within 1–2 minutes.
- **Add a new lab:**
  1. Upload the new page into `labs/`.
  2. Open `index.html` on GitHub, click the ✏️ pencil, find the `LABS` list near the bottom and add a line, for example:
     ```js
     { f: 'lab10-new-page.html', ico: '🧪', t: 'Lab 10 Title', d: 'One-line description.', k: 'hands' },
     ```
     (`k: 'hands'` gives the green **Hands-on** label. Leave it out for a **Walkthrough**.)
  3. Click **Commit changes**.

If students still see an old version, ask them to refresh with **Ctrl + F5** (Windows) or **Cmd + Shift + R** (Mac).

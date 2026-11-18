# CIS 2903 Lab Practice Hub – How to host it

The folder holds a complete static website. There is nothing to install and no server to run.

```
cis2903-practice-hub/
├── index.html          ← home page (lists every lab)
├── HOW-TO-HOST.md      ← this guide (not shown to students)
└── labs/               ← one page per animation (13 pages)
```

To preview it, unzip the folder and double-click `index.html`.

---

## Option A – Netlify Drop (easiest, about 2 minutes)

1. Unzip `cis2903-practice-hub.zip`.
2. Go to **https://app.netlify.com/drop** and sign up for free (email or GitHub).
3. Drag the **`cis2903-practice-hub` folder** onto the page.
4. You get a link like `https://random-name-123.netlify.app`.
   Go to **Site configuration → Change site name** to choose something like `cis2903-hct.netlify.app`.
5. Share the link with students on your LMS or Teams.

**To update later:** open the site in Netlify, go to **Deploys**, and drag the updated folder in. The link stays the same.

---

## Option B – GitHub Pages (permanent and free)

1. Create a free account at **https://github.com**.
2. Click **New repository**, name it `cis2903`, set it to **Public**, then click **Create**.
3. Click **uploading an existing file**, drag in **everything inside** the unzipped folder (`index.html` and the `labs` folder), then click **Commit changes**.
4. Go to **Settings → Pages → Build and deployment**. Set Source to **Deploy from a branch** and Branch to **main / (root)**, then click **Save**.
5. After 1–2 minutes your site is live at `https://YOUR-USERNAME.github.io/cis2903/`.

**To update later:** upload the changed files to the repository again. The site refreshes within a minute or two.

---

## Adding a new lab later

1. Put the new page's `.html` file in the `labs/` folder.
2. In `index.html`, find the `LABS` list near the bottom and copy one line, for example:
   ```js
   { f: 'lab10-new-page.html', ico: '🧪', t: 'Lab 10 Title', d: 'One-line description.' },
   ```
   Add `k: 'hands'` if the page lets students type commands.
3. Upload again with Option A or B.

(Or ask Claude to add it for you.)

---

## Notes
- Every page shows an **"← All labs"** button and a **"Practice only · Exam is on a real VM"** note in the bottom-left corner.
- The pages load fonts from Google Fonts. If a network blocks that, they still work with system fonts.
- Before putting course material on a public site, check HCT's IT and academic policy.

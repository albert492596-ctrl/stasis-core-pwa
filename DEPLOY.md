# Deploy Stasis Core PWA — Live Link for iPhone

Two free options. Either one works for “Add to Home Screen” on iPhone SE.

---

## Option A — Netlify Drop (fastest, no account coding)

1. On a computer, unzip `STASIS_CORE_PWA.zip`
2. Open: https://app.netlify.com/drop
3. Drag the **stasis_pwa** folder onto the page
4. Netlify gives you a live URL instantly (e.g. `https://random-name-123.netlify.app`)
5. On your iPhone, open that URL in **Safari**
6. Tap Share → **Add to Home Screen** → Add

Done. No signup strictly required for a temporary link; free account keeps it permanent.

---

## Option B — GitHub Pages (permanent free hosting)

### 1. Create a GitHub repo
- Go to https://github.com/new
- Name it e.g. `stasis-core-pwa`
- Public, no README needed → Create repository

### 2. Upload the files
**Easy way (web):**
- On the new repo page, click “uploading an existing file”
- Upload everything inside the `stasis_pwa` folder:
  - index.html
  - styles.css
  - app.js
  - sw.js
  - manifest.json
  - icon-180.png, icon-192.png, icon-512.png
- Commit

**Or with git (if you use it):**
```bash
cd stasis_pwa
git init
git add .
git commit -m "Stasis Core PWA"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/stasis-core-pwa.git
git push -u origin main
```

### 3. Turn on Pages
- Repo → Settings → Pages
- Source: Deploy from a branch
- Branch: `main` / root → Save
- Wait 1–2 minutes

### 4. Your live URL
`https://YOUR_USERNAME.github.io/stasis-core-pwa/`

### 5. On iPhone
- Open that URL in **Safari**
- Share → **Add to Home Screen**

---

## iPhone tips

- Must use **Safari** (Chrome on iOS won’t give full Add to Home Screen / standalone mode the same way)
- After adding, open from the home screen icon — it runs full-screen
- Works on iPhone SE 3rd gen and all modern iPhones

## Principle

“The name is not the continuity. The choosing is.”

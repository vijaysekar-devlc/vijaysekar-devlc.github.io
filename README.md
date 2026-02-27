# Zoom Marketplace – Required pages

This folder contains the **Privacy Policy**, **Terms of Use**, **Support**, **Documentation**, and **Configure** pages required (or optional) for Zoom Marketplace app submission. Host these at stable public URLs and paste those URLs into the Zoom app listing.

---

## 1. Before hosting – replace placeholders

In every HTML file, replace these placeholders with your real values:

| Placeholder | Replace with | Prefilled in this repo |
|-------------|--------------|------------------------|
| `[YOUR_COMPANY_NAME]` | Your company or product name | **LiveControl** |
| `[SUPPORT_EMAIL]` | Your support/contact email | **support@livecontrol.io** |
| `[UPDATE_DATE]` | Date of last update | **February 26, 2026** |
| `[GOVERNING_LAW_JURISDICTION]` | Only in `terms.html` – law and jurisdiction | **the laws of the State of California, USA** |

The HTML files in this folder are already prefilled with the values above. If you need to change them, edit the files directly or do a find-and-replace.

---

## 2. How to host (choose one)

You need **live URLs** that Zoom can open. Examples:

### Option A: GitHub Pages (free, easy)

1. Create a new repo (e.g. `livecontrol-zoom-pages`) or use an existing one.
2. Upload this folder’s contents so the repo has:
   - `privacy.html`
   - `terms.html`
   - `support.html`
   - `documentation.html`
   - `configure.html`
3. In the repo: **Settings → Pages**. Source: **Deploy from a branch**. Branch: `main` (or `master`), folder: **/ (root)**. Save.
4. After a minute or two, pages will be at:
   - `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/privacy.html`
   - `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/terms.html`
   - etc.

Use these as your **Privacy Policy URL**, **Terms of Use URL**, **Support URL**, **Documentation URL**, and optionally **Configure URL**.

### Option B: Your company website

Upload the five HTML files to your site, e.g.:

- `https://yourcompany.com/zoom-app/privacy`
- `https://yourcompany.com/zoom-app/terms`
- `https://yourcompany.com/zoom-app/support`
- `https://yourcompany.com/zoom-app/documentation`
- `https://yourcompany.com/zoom-app/configure`

(Your server may use `privacy.html` as the default for `/zoom-app/privacy` depending on config.)

### Option C: Netlify / Vercel / similar

Drag this folder into Netlify (or connect the repo). The site will be `https://something.netlify.app`. Your URLs would be:

- `https://something.netlify.app/privacy.html`
- `https://something.netlify.app/terms.html`
- etc.

---

## 3. What to enter in the Zoom Marketplace

In your Zoom app’s submission form, fill in:

| Zoom field | Your URL (example) |
|------------|--------------------|
| **Privacy Policy URL** | `https://yourcompany.com/zoom-app/privacy` or `https://username.github.io/repo/privacy.html` |
| **Terms of Use URL** | `https://yourcompany.com/zoom-app/terms` or `.../terms.html` |
| **Support URL** | `https://yourcompany.com/zoom-app/support` or `.../support.html` |
| **Documentation URL** | `https://yourcompany.com/zoom-app/documentation` or `.../documentation.html` |
| **Configure URL** (optional) | `https://yourcompany.com/zoom-app/configure` or `.../configure.html` |

Use the **exact** URLs where each page is live. Zoom will check that they load.

---

## 4. File summary

| File | Purpose |
|------|---------|
| `privacy.html` | Privacy Policy – data collection, use, retention, data subject rights (required by Zoom). |
| `terms.html` | Terms of Use (required). |
| `support.html` | Support page with contact and common issues (required). |
| `documentation.html` | Zoom-specific guide: adding, using, removing the app (required). |
| `configure.html` | Explains that configuration is in the desktop app (optional Configure URL). |

---

## 5. After publishing

- Keep the URLs stable. If you move your site, set up redirects or update the URLs in the Zoom Marketplace.
- When you change policies or terms, update the “[UPDATE_DATE]” (and the content) and re-save the files so the live pages stay current.

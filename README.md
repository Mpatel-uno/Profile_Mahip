# Mahip Patel — Portfolio Website

A polished, mobile-friendly personal portfolio site built as a single React component with a classic professional palette (navy + warm grey, gold accents, serif headings).

## What's in this folder

- **`index.html`** — open this in a browser to preview the site instantly. No build step required (uses React + Babel via CDN).
- **`Portfolio.jsx`** — the React component as a single file. Drop into any React app (Vite, CRA, Next.js).
- **`README.md`** — this file.

## Quick start (preview locally)

1. Save your photo as **`profile.jpg`** in this folder.
2. Save your résumé PDF as **`Mahip_Resume.pdf`** in this folder (the original `Mahip_Resume_new.pdf` works too — just update the filename in the code or rename the file).
3. Double-click `index.html`. That's it.

> Tip: if you double-click and the page is blank, right-click → *Open with* → your browser. Some browsers require `http://` rather than `file://` to load Babel — in that case run a quick local server: `python3 -m http.server` from this folder, then visit `http://localhost:8000`.

## Using the React component (`Portfolio.jsx`)

```bash
# In a fresh Vite app:
npm create vite@latest my-portfolio -- --template react
cd my-portfolio
# Drop Portfolio.jsx into src/, plus profile.jpg and Mahip_Resume.pdf into public/
# In src/App.jsx:
import Portfolio from "./Portfolio.jsx";
export default function App() { return <Portfolio />; }
npm install && npm run dev
```

## Editing your content

Open `Portfolio.jsx` (or `index.html`) and look for the `data = { ... }` object near the top. Everything is there:

- `name`, `tagline`, `location`, `email`, `phone`
- `github`, `linkedin` — update the LinkedIn URL once you confirm the slug
- `about` — your bio paragraph
- `experience[]` — work history
- `education[]` — schools
- `skills[]` — grouped skill chips
- `projects[]` — featured projects

Change values, save, refresh.

## Free hosting options

| Host | How |
| --- | --- |
| **GitHub Pages** | Push `index.html` + `profile.jpg` + `Mahip_Resume.pdf` to a repo, enable Pages on the main branch. |
| **Netlify Drop** | Drag this folder onto https://app.netlify.com/drop — instant URL. |
| **Vercel** | `vercel` from this folder, follow prompts. |
| **Cloudflare Pages** | Connect to a GitHub repo, no build command needed. |

## Custom domain

Once hosted, point your domain (e.g., `mahippatel.com`) at the host's DNS. All four hosts above include free TLS.

## What to verify before sharing

- Replace `https://www.linkedin.com/in/mahip-patel` with your actual LinkedIn URL if the slug differs.
- Confirm `github.com/mahip-patel` is correct.
- Add real project links (`tech` array can be extended with a `link` field).
- Drop in a higher-resolution profile photo if you have one (4:5 portrait works best).

— Built May 2026.

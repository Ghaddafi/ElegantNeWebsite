# Elegant Designs — Architecture & Construction

A single-page website for Elegant Designs, built for GitHub Pages.

---

## Deploying to GitHub Pages

1. Create a new repository on GitHub (e.g. `elegant-designs`)
2. Upload all files maintaining this folder structure:
   ```
   /
   ├── index.html
   ├── README.md
   └── images/
       ├── intro-bg.jpg
       ├── hero-0.jpg
       ├── hero-1.jpg
       ├── hero-2.jpg
       ├── proj-1.jpg
       ├── proj-2.jpg
       ├── proj-3.jpg
       ├── proj-4.jpg
       ├── proj-5.jpg
       ├── proj-6.jpg
       ├── proj-7.jpg
       ├── spot.jpg
       ├── insight-1.jpg
       ├── insight-2.jpg
       └── insight-3.jpg
   ```
3. Go to **Settings → Pages → Branch: main → / (root)** and click Save
4. Your site will be live at `https://yourusername.github.io/elegant-designs`

---

## Replacing Images

### Method 1 — Direct file replacement (recommended for production)
Replace any file in the `images/` folder with your own photo using the same filename.  
Commit and push — the site updates automatically.

Image size guidelines:
| File | Dimensions | Notes |
|---|---|---|
| `intro-bg.jpg` | 1920×1080 | Intro splash screen |
| `hero-0/1/2.jpg` | 1920×1080 | Hero slideshow |
| `proj-1.jpg` | 800×1100 | Portrait — main feature card |
| `proj-2.jpg` | 800×600 | Landscape |
| `proj-3/4.jpg` | 800×440 | Landscape |
| `proj-5/6/7.jpg` | 600×360 | Secondary row |
| `spot.jpg` | 720×600 | Studio section |
| `insight-1/2/3.jpg` | 560×352 | Blog cards |

### Method 2 — In-browser admin panel
The site has a hidden admin image manager. To access it:

- **Keyboard shortcut:** Press `A` then `D` then `M` in sequence
- **URL param:** Add `?admin` to the end of your URL, e.g. `https://yoursite.github.io/?admin`
- **Password:** `12345`

Once unlocked, you can upload, preview, and replace images directly in the browser. Images are saved locally (browser storage) and will persist on that device.  
Use **Export HTML ↓** to download a self-contained `index.html` with all images embedded — useful for sending to a client or keeping an offline backup.

> **Note:** To permanently update the live site, always replace the files in `images/` and push to GitHub.  
> The admin panel only updates images locally in your browser.

---

## Customisation

All content (text, project names, contact details, awards) is in `index.html`.  
Search for the following to find what to edit:

- `hello@elegantdesigns.com` — contact email
- `+255 000 000 000` — phone number
- `Est. Dar es Salaam — 2019` — tagline in intro
- `© 2025 Elegant Designs` — footer copyright

---

## Tech Stack

- Pure HTML/CSS/JS — no build tools, no dependencies
- Google Fonts (Libre Baskerville, Barlow, Barlow Condensed)
- Fully responsive (mobile, tablet, desktop)
- GitHub Pages compatible (static, no server required)

# GDN Group Website

**GDN Enterprise Pty Ltd** | ACN 666 495 263 | Southport QLD 4215

A fully static, GitHub Pages-ready website for GDN Group covering Commodity Trading, Strategic Advisory, and CrossLedger (CLXT) blockchain trade infrastructure.

---

## File Structure

```
gdn-website/
├── index.html              ← Homepage
├── css/style.css           ← Design system
├── js/main.js              ← Animations and interactions
├── README.md               ← This file
└── pages/
    ├── trading.html        ← Commodity products
    ├── advisory.html       ← Advisory practice
    └── crossledger.html    ← CrossLedger / CLXT
```

---

## Deploy to GitHub Pages

### Step 1 — Create a GitHub repository

1. Go to github.com and sign in (create a free account if needed)
2. Click "New repository"
3. Name it: gdngroup-website
4. Set to Public
5. Click "Create repository"

### Step 2 — Upload the files

6. On the empty repo page, click "uploading an existing file"
7. Drag all files from the gdn-website folder into the upload box
8. Click "Commit changes"

### Step 3 — Enable GitHub Pages

9. Go to Settings then Pages
10. Under Source, select "Deploy from a branch"
11. Branch: main, Folder: / (root)
12. Click Save

Your site will be live at: https://yourusername.github.io/gdngroup-website/

---

## Connect Your Custom Domain (gdngroup.com.au)

1. In Settings then Pages, enter your custom domain: gdngroup.com.au
2. Tick "Enforce HTTPS"
3. At your domain registrar, add these DNS records:
   - CNAME: www pointing to yourusername.github.io
   - A records for apex domain:
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153

DNS changes take up to 48 hours to propagate.

---

## How to Update Content

All content is in plain HTML. No CMS or build tools needed.

| What to change        | Where                          |
|-----------------------|--------------------------------|
| Hero headline         | index.html - hero-content      |
| Trading products      | pages/trading.html             |
| Advisory engagements  | pages/advisory.html            |
| CrossLedger data      | pages/crossledger.html         |
| Contact details       | index.html - contact-item      |
| Colours and fonts     | css/style.css - :root section  |

---

## Design System

Fonts (Google Fonts - no install needed):
- Cormorant Garamond - headings
- DM Sans - body text
- DM Mono - labels and tags

Key colours (edit in css/style.css):
- Navy background: #07091A
- Gold accent: #C9A84C
- CrossLedger blue: #2A6FDB
- Body text: #EDE9DF

---

## Contact Form

The form shows a success animation but does not send emails by default. To wire it up, use Formspree (free, no backend needed): replace the form submit handler in js/main.js with a fetch POST to https://formspree.io/f/YOUR_ID

---

## Legal

2026 GDN Enterprise Pty Ltd. All rights reserved.
ACN 666 495 263 | ABN 65 666 495 263
This website does not constitute financial, legal, or investment advice.

# Hillside Stays Website

Full marketing website for Hillside Stays — Western North Carolina short-term rental co-hosting company.

## Files
- `index.html` — Main website (all sections)
- `style.css` — All styles
- `script.js` — Interactivity (nav, FAQ, form, animations)
- `owner-portal.html` — Owner portal placeholder page

---

## Deploying to GitHub Pages (Free Hosting)

### Step 1: Get a GitHub account
Go to github.com and create a free account if you don't have one.

### Step 2: Create a new repository
1. Click the green "New" button on your GitHub dashboard
2. Name it exactly: `hillsidestays` (or your preferred name)
3. Set it to **Public**
4. Click "Create repository"

### Step 3: Upload your files
1. On the new repository page, click "uploading an existing file"
2. Drag all 4 files (index.html, style.css, script.js, owner-portal.html) into the upload area
3. Click "Commit changes"

### Step 4: Enable GitHub Pages
1. Go to your repository's **Settings** tab
2. Click **Pages** in the left sidebar
3. Under "Source", select **Deploy from a branch**
4. Select branch: **main**, folder: **/ (root)**
5. Click **Save**

Your site will be live at: `https://YOUR-USERNAME.github.io/hillsidestays`
(takes 1-2 minutes to go live after saving)

---

## Setting Up Your Contact Form (Formspree)

1. Go to **formspree.io** and create a free account
2. Click "New Form" and name it "Hillside Stays Contact"
3. Copy your unique Form ID (looks like: `xpzgkwqr`)
4. Open `index.html` and find this line:
   ```
   action="https://formspree.io/f/YOUR_FORM_ID"
   ```
5. Replace `YOUR_FORM_ID` with your actual ID
6. Re-upload `index.html` to GitHub

Free Formspree tier allows **50 submissions/month** — plenty to start.

---

## Connecting a Custom Domain

1. Buy your domain at **Namecheap.com** (~$12/year for .com)
   - Search for: hillsidestays.com
2. In Namecheap DNS settings, add these records:
   ```
   Type: A      Host: @    Value: 185.199.108.153
   Type: A      Host: @    Value: 185.199.109.153
   Type: A      Host: @    Value: 185.199.110.153
   Type: A      Host: @    Value: 185.199.111.153
   Type: CNAME  Host: www  Value: YOUR-USERNAME.github.io
   ```
3. In GitHub Pages settings, enter your custom domain
4. Check "Enforce HTTPS" once it propagates (24-48 hours)

---

## What to Update Before Going Live

1. **Contact form** — Replace `YOUR_FORM_ID` with Formspree ID (see above)
2. **Email address** — Search for `hello@hillsidestays.com` and replace with your actual email
3. **Revenue stats** — Verify the nightly rate and occupancy figures against current AirDNA data
4. **Footer phone** — Add your phone number if desired
5. **Social links** — Replace `href="#"` on Instagram/Facebook icons with your actual profile URLs
6. **Privacy Policy / Terms** — Add actual pages or link to a simple terms generator

---

## Monthly Cost Summary

| Item | Cost |
|------|------|
| GitHub Pages hosting | **Free** |
| Formspree (contact form) | **Free** (50/mo) |
| Domain name | ~$12/year (~$1/mo) |
| **Total** | **~$1/month** |

Upgrade paths:
- Formspree paid ($10/mo) when you exceed 50 leads/month — a good problem to have
- Move to Webflow ($14/mo) if you want a visual drag-and-drop editor for updates

# Lebancho — Official Website

Streetwear landing page for **Lebancho** — embroidered streetwear brand based in Jaipur.

---

## 🚀 How to Deploy on GitHub Pages + Custom Domain

### Step 1 — Create a GitHub Account
Go to [github.com](https://github.com) and sign up for a free account if you don't have one.

---

### Step 2 — Create a New Repository
1. Click the **"+"** button (top right) → **New repository**
2. Name it exactly: `lebancho-website` (or any name you like)
3. Set it to **Public**
4. Click **Create repository**

---

### Step 3 — Upload Your Files
You have two options:

**Option A — Upload via GitHub website (easiest):**
1. Open your new repository
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop ALL files from this folder:
   - `index.html`
   - `CNAME`
   - `images/` folder (add your product photos here later)
4. Click **"Commit changes"**

**Option B — Using Git (for developers):**
```bash
git init
git add .
git commit -m "Initial Lebancho website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/lebancho-website.git
git push -u origin main
```

---

### Step 4 — Enable GitHub Pages
1. Go to your repository → click **Settings** (top tab)
2. Scroll down to **"Pages"** in the left sidebar
3. Under **"Source"** → select **"Deploy from a branch"**
4. Branch: **main** / folder: **/ (root)**
5. Click **Save**
6. Wait 2–3 minutes — your site will be live at:
   `https://YOUR_USERNAME.github.io/lebancho-website`

---

### Step 5 — Connect Your Custom Domain

#### A) Edit the CNAME file
Open `CNAME` in this folder and replace `www.yourdomain.com` with your actual domain, e.g.:
```
www.lebancho.com
```

#### B) Add DNS records at your domain registrar
Log in to wherever you bought your domain (GoDaddy, Namecheap, BigRock, etc.) and add these DNS records:

**For www subdomain (recommended):**
| Type  | Name | Value                              |
|-------|------|------------------------------------|
| CNAME | www  | YOUR_USERNAME.github.io            |

**For root/apex domain (e.g. lebancho.com without www):**
| Type | Name | Value          |
|------|------|----------------|
| A    | @    | 185.199.108.153 |
| A    | @    | 185.199.109.153 |
| A    | @    | 185.199.110.153 |
| A    | @    | 185.199.111.153 |

#### C) Set the domain in GitHub Pages settings
1. Go to **Settings → Pages**
2. Under **"Custom domain"** enter: `www.yourdomain.com`
3. Click **Save**
4. Wait for DNS to propagate (can take up to 24 hours, usually under 1 hour)
5. Check **"Enforce HTTPS"** once it appears ✅

---

### Step 6 — Add Your Product Images
1. Go to the `images/` folder in your repository
2. Upload product photos named like:
   - `hoodie-1.jpg`
   - `cap-1.jpg`
   - `tee-1.jpg`
   - `shoes-1.jpg`
3. In `index.html`, replace placeholder blocks like:
   ```html
   <div class="product-placeholder" style="...">
   ```
   With:
   ```html
   <img src="images/hoodie-1.jpg" class="product-img" alt="Signature Embroidery Hoodie">
   ```

---

## 📁 File Structure
```
lebancho-website/
├── index.html        ← Main landing page (this is your website)
├── CNAME             ← Your custom domain goes here
├── images/           ← Add product photos here
│   └── (your product images)
└── README.md         ← This guide
```

---

## ✏️ How to Edit Content

Open `index.html` in any text editor (Notepad, VS Code, etc.) and search for:

- **Brand name / tagline** → Search `WEAR YOUR CRAFT`
- **Product names & prices** → Search `₹` to find all prices
- **Nav links** → Search `<nav`
- **Newsletter text** → Search `GET FIRST ACCESS`
- **Footer links** → Search `<footer`
- **WhatsApp / Instagram links** → Search `social-links`

---

## 🌐 Free Tools Used (No Cost)
- **GitHub Pages** — Free hosting
- **Google Fonts** — Free fonts (Bebas Neue, DM Sans, Dancing Script)
- Your custom domain — Only paid part (~₹800–1500/year from GoDaddy or Namecheap)

---

Made with ❤️ for Lebancho — Embroidered in Jaipur.

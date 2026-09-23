# Dynamic Trilateral Leadership - Deployment Guide

## Domain
**dynamictrilateral.org**

## Registrar
**Namecheap** (same account as Clarity House)

---

## Step 1: Register the Domain

1. Log into Namecheap (same account as clarityhouse.consulting)
2. Search: `dynamictrateral.org`
3. Purchase (should be ~€12-15/year)
4. Wait for domain to activate (usually instant, up to 1 hour)

---

## Step 2: Add DNS Records in Namecheap

1. Go to **Domain List** → Click **Manage** next to dynamictrilateral.org
2. Click **Advanced DNS** tab
3. Add these records:

| Type | Host | Value | TTL |
|------|------|-------|-----|
| A Record | @ | 185.199.108.153 | Automatic |
| A Record | @ | 185.199.109.153 | Automatic |
| A Record | @ | 185.199.110.153 | Automatic |
| A Record | @ | 185.199.111.153 | Automatic |
| CNAME Record | www | mbeyst.github.io | Automatic |

**Note:** These are GitHub Pages IP addresses — same as Clarity House.

---

## Step 3: Create GitHub Repository

1. Go to: github.com/new
2. Repository name: `dynamic-trilateral`
3. Public repository
4. **Do NOT** initialize with README
5. Click **Create repository**

---

## Step 4: Upload Files

Upload these files to the repository:

- `index.html` (the journey site — index-journey.html, renamed to index.html)
- `CNAME` (contains: dynamictrilateral.org)
- `.gitignore` (optional, for future development)

**Method A: Web Upload (Easiest)**
1. Click **uploading an existing file**
2. Drag files from `C:\Users\martinb\dynamic-trilateral\`
3. Commit changes

**Method B: Git Command Line**
```bash
cd C:\Users\martinb\dynamic-trilateral
git init
git add .
git commit -m "Initial DTL site"
git branch -M main
git remote add origin https://github.com/mbeyst/dynamic-trilateral.git
git push -u origin main
```

---

## Step 5: Configure GitHub Pages

1. Go to: github.com/mbeyst/dynamic-trilateral/settings/pages
2. **Source:** Deploy from branch
3. **Branch:** main (or master) → Folder: / (root)
4. Click **Save**
5. Wait ~2 minutes for deployment

---

## Step 6: Connect Custom Domain

1. In GitHub Pages settings, scroll to **Custom domain**
2. Enter: `dynamictrilateral.org`
3. Click **Save**
4. Check **Enforce HTTPS** (wait for certificate to provision, ~5 minutes)

---

## Step 7: Verify DNS Propagation

1. Go to: https://dnschecker.org/
2. Search: `dynamictrilateral.org`
3. Wait until all regions show GitHub Pages IPs

**Propagation time:** Usually 5-30 minutes, can take up to 24 hours.

---

## Step 8: Test the Site

Once DNS propagates:
- https://dynamictrilateral.org — should load
- https://www.dynamictrilateral.org — should redirect to root

---

## Step 9: Set Up Email Forwarding (Optional)

If you want `martin@dynamictrilateral.org` to forward to your main email:

1. In Namecheap, go to **Advanced DNS**
2. Add MX records for email forwarding service (e.g., ImprovMX, ForwardEmail)
3. Or use **Email Forwarding** section in Namecheap dashboard

**Recommended:** ImprovMX (free tier)
- Add MX records as specified
- Create forward: `martin@dynamictrilateral.org` → your main email

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Domain not resolving | Wait 24 hours for DNS propagation |
| GitHub Pages 404 | Check CNAME file exists and matches domain exactly |
| HTTPS not working | Wait longer for certificate, then re-check "Enforce HTTPS" |
| www not redirecting | Check CNAME record for www subdomain |

---

## Files Needed

From `C:\Users\martinb\dynamic-trilateral\`:

1. **index-journey.html** → Rename to **index.html** before uploading
2. **CNAME** → Contains exactly: `dynamictrilateral.org` (no trailing spaces)

---

## Post-Launch Checklist

- [ ] Update LinkedIn profile with new website URL
- [ ] Update video script CTAs to use the live URL
- [ ] Test contact forms (set up Formspree)
- [ ] Add Google Analytics (optional)
- [ ] Set up email forwarding

---

*Created: July 2026*
*For: Martin Beyst - Dynamic Trilateral Leadership*

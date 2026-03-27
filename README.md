# Career Cafe + R.O.O.T.E.D. Journals — Wix Store Scaffold

Static HTML demo and Wix configuration spec for two digital product brands.

---

## Files in This Repo

| File | Purpose |
|------|---------|
| `career-cafe-product.html` | Product page visual spec — Career Cafe brand |
| `rooted-product.html` | Product page visual spec — R.O.O.T.E.D. Journals brand |
| `store-config.md` | Wix setup guide: slugs, digital delivery, automations, variants |
| `README.md` | This file — overview and Wix Contributor invite workflow |

---

## How to View the Demos

Open either HTML file directly in a browser — no server required:

```
open career-cafe-product.html
open rooted-product.html
```

These are **visual spec files only**. Buttons and links are non-functional. They represent the exact layout and styling intent to be built inside Wix.

---

## Wix Contributor Invite Workflow

### Overview

Wix uses a **role-based Contributor system**. To give a developer, designer, or agency access to the store without sharing the account owner's credentials, follow the steps below.

---

### Step 1 — Access Dashboard Roles

1. Log in to [manage.wix.com](https://manage.wix.com)
2. Select your site
3. Go to **Dashboard → Settings → Roles & Permissions**

---

### Step 2 — Invite a Contributor

1. Click **"Invite People"**
2. Enter the contributor's email address
3. Select their role:

| Role | Access Level | When to Use |
|------|-------------|-------------|
| **Owner** | Full access | Never share — keep for account holder only |
| **Admin** | Full dashboard access, no billing | Trusted team leads |
| **Store Manager** | Manage products, orders, coupons | eCommerce VA or assistant |
| **Designer** | Edit site visuals in Editor | Web designer or agency |
| **Blog Writer** | Blog content only | Content team |
| **SEO Specialist** | SEO panel + content | SEO contractor |
| **Developer** | Editor + code access (Velo/Corvid) | Technical developer |

4. Click **Send Invite**

The contributor receives an email. They must accept via **their own Wix account** (free account works). They do not need a paid plan.

---

### Step 3 — Developer Access (Wix Dev Mode)

If the developer needs to write custom code (Velo by Wix):

1. In the site Editor, go to **Dev Mode → Enable Dev Mode**
2. Ensure the contributor has **Developer** or **Admin** role
3. Share the **site URL** from **Dashboard → Settings → Site URL**

> Warning: Enabling Dev Mode activates Wix Velo (JavaScript). This cannot be disabled after enabling without potential loss of custom code.

---

### Step 4 — Handing Off This Spec

When sharing this visual spec with the Wix developer or Designer contributor:

1. Send both HTML files for visual reference
2. Send `store-config.md` for technical setup steps
3. Key things to point out:
   - **Color palettes** are in CSS `:root` variables at the top of each HTML file
   - **Product names, prices, and descriptions** are ready to copy-paste into Wix product editor
   - **Email templates** are in `store-config.md` — paste into Wix Automations
   - **Image placeholders** indicate required dimensions and aspect ratios

---

### Step 5 — Removing Access

When the project is complete:
1. **Dashboard → Settings → Roles & Permissions**
2. Find the contributor → click **"..."** → **Remove**

Access is revoked immediately. The contributor's Wix account is not deleted.

---

## Brand Quick Reference

### Career Cafe
- **Palette:** Teal `#2A8C94` / Black `#1A1A1A` / White `#FFFFFF`
- **Feel:** Clean, professional, academic
- **Product:** Career Cafe Journal — Daily Planning Edition — $24.99 digital PDF
- **CTA Color:** `#2A8C94` background, white text

### R.O.O.T.E.D. Journals
- **Full Name:** Rooted Opportunities & Organized Thoughts for Everyday Direction
- **Palette:** Black `#0D0D0D` / Gold `#C9A84C` / Cream `#F5F0E8`
- **Feel:** Bold, campaign-style, launch energy
- **Product:** R.O.O.T.E.D. Journal — Volume 1 — $29.99 digital PDF
- **CTA Color:** `#C9A84C` background, black text
- **Founder:** Nicole (personal note section included in product page)

---

## Wix Plan Requirements

| Feature Used | Minimum Wix Plan |
|-------------|-----------------|
| Wix eCommerce / Store | **Core** or higher |
| Digital product delivery | **Core** or higher |
| Automations (post-purchase email) | **Core** or higher |
| Custom domain | Any paid plan |
| Wix Velo (custom code) | Any paid plan |
| Remove Wix branding | Any paid plan |

> The free Wix plan does **not** support eCommerce or digital file delivery.

---

## Next Steps Checklist

- [ ] Client accepts Wix Contributor invite
- [ ] Developer reviews HTML spec files
- [ ] Products created in Wix Store with correct pricing and digital files
- [ ] Collections created: `career-cafe` and `rooted-journals`
- [ ] Product variants configured (PDF format options)
- [ ] Post-purchase email automations built in Wix Automations
- [ ] CTA button colors updated to match brand palettes
- [ ] Store URL slugs set per `store-config.md`
- [ ] Test purchase completed end-to-end (use Wix test payment mode)
- [ ] Custom domain connected

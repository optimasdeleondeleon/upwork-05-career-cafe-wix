# Wix Store Configuration Guide
## Career Cafe + R.O.O.T.E.D. Journals — Digital Product Setup

---

## 1. Store URL Slug

Both brands share one Wix site. Configure the store path under:

**Wix Dashboard → Pages & Menu → Store Pages**

| Page | Recommended Slug |
|------|-----------------|
| Main shop | `/shop` |
| Career Cafe collection | `/shop/career-cafe` |
| R.O.O.T.E.D. collection | `/shop/rooted-journals` |

> **Note:** Wix auto-generates product page URLs as `/shop/product-page/{product-name}`. To customize individual product slugs, go to the product editor → SEO tab → Edit URL.

---

## 2. Digital Delivery Configuration

### Enable Digital Products
1. **Wix Dashboard → Store → Products → + Add Product**
2. Select **"Digital File"** as product type (not Physical)
3. Upload your PDF under **"Manage Digital Files"** — files upload to Wix's secure delivery server
4. Wix auto-sends a time-limited download link via post-purchase email (valid 30 days / 3 download attempts by default)

### Digital File Settings (per product)
- **File type:** PDF
- **Download attempts:** Set to `5` (recommended — avoids support tickets)
- **Link expiry:** `30 days` after purchase
- **Re-download:** Customer can re-download from "My Orders" in their Wix account

### Wix Pricing Plans (optional upgrade path)
If bundling journals into a membership or subscription, use **Wix Pricing Plans** app. Not required for one-time digital downloads.

---

## 3. Product Page Variants Feature

Wix eCommerce supports **Product Options** (variants) on each product. Use this for:

### Career Cafe Journal — Daily Planning Edition
| Option Name | Values |
|-------------|--------|
| Format | PDF (Letter), PDF (A4), A5 Print-Ready |

**Setup:**
1. Product Editor → **Options & Variants**
2. Add option: **Format** (Dropdown or Button layout)
3. Each variant can have a separate SKU — keep price the same across formats or adjust if needed

### R.O.O.T.E.D. Journal — Volume 1
| Option Name | Values |
|-------------|--------|
| Edition | Digital PDF, Bundle (Vol 1 + Workbook) |

> Wix does not currently support different digital files per variant on the same product. If each format needs a different file, create separate products and use a collection to group them.

---

## 4. HTML Embed Button — Link Update Instructions

The HTML demo files (`career-cafe-product.html`, `rooted-product.html`) use static buttons for visual reference. To wire up real purchase buttons in Wix:

### Option A: Use Wix's Native Buy Button (Recommended)
- In Wix Editor: **Add → Store → Buy Button**
- Connect to the correct product via "Connect to Data"
- Style to match brand palette (see color values below)

### Option B: Custom HTML Embed with Wix Product Link
If using a custom-coded section via **Wix Dev Mode / Corvid**:

```html
<!-- Replace href with your Wix product page URL -->
<a href="/shop/product-page/career-cafe-journal-daily-planning-edition"
   class="btn-add-to-cart">
  Add to Cart — $24.99
</a>
```

For R.O.O.T.E.D.:
```html
<a href="/shop/product-page/rooted-journal-volume-1"
   class="btn-cta-gold">
  Get Your Copy — $29.99
</a>
```

### Button Color Reference
| Brand | CTA Button BG | CTA Button Text |
|-------|--------------|-----------------|
| Career Cafe | `#2A8C94` | `#FFFFFF` |
| R.O.O.T.E.D. | `#C9A84C` | `#0D0D0D` |

---

## 5. Post-Purchase Automation Email Templates

Configure both under:
**Wix Dashboard → Automations → + New Automation → "Order is placed" trigger**

---

### EMAIL TEMPLATE 1 — Career Cafe

**Trigger:** Order placed → Product contains "Career Cafe Journal"
**Send delay:** Immediately

---

**Subject:** Your Career Cafe Journal is ready — download inside

**Preview text:** Your PDF is waiting. Let's get to work.

---

Hi {{contact.firstName}},

Thank you for your purchase! Your **Career Cafe Journal — Daily Planning Edition** is ready to download right now.

**[Download Your Journal →]** *(Wix auto-inserts secure download button here)*

Your download link is valid for **30 days** and can be used up to 5 times. You can also access it anytime from your account under **My Orders**.

---

**Getting Started Tips:**

- Print at 100% scale on Letter or A4 paper (duplex recommended)
- Or import directly into GoodNotes / Notability for digital use
- Start with the **Monthly Intention** page before diving into daily spreads

---

Have questions? Reply to this email or reach us at **hello@careercafe.co**

We can't wait to see what you build.

— The Career Cafe Team

*You're receiving this because you made a purchase at careercafe.co. [Manage preferences]*

---

### EMAIL TEMPLATE 2 — R.O.O.T.E.D. Journals

**Trigger:** Order placed → Product contains "R.O.O.T.E.D. Journal"
**Send delay:** Immediately

---

**Subject:** You're rooted. Your journal is here.

**Preview text:** Volume 1 is in your hands. Your story starts now.

---

{{contact.firstName}},

You made a move. Now let's build on it.

Your **R.O.O.T.E.D. Journal — Volume 1** is ready to download.

**[Get Your Journal →]** *(Wix auto-inserts secure download button here)*

---

**This journal was made for you. Here's how to start:**

1. Open the **"Before You Begin"** intro page first — read it slowly
2. Complete the **Root Check-In** on page 3 before anything else
3. Don't skip the weekly reflection spreads — that's where the real work happens

Your link is active for **30 days**. Download it now and save it somewhere you'll find it.

---

You joined something real. Welcome to the R.O.O.T.E.D. community.

With purpose,

**Nicole**
Founder, R.O.O.T.E.D. Journals

*Questions? Email us at hello@rootedjournals.co*

*[Unsubscribe] | [Manage Preferences]*

---

## 6. Collection Setup

Create two Wix Store Collections:

| Collection Name | URL Slug | Products |
|----------------|----------|---------|
| Career Cafe | `career-cafe` | Career Cafe Journal, Resume Workbook, Interview Prep Toolkit |
| R.O.O.T.E.D. Journals | `rooted-journals` | R.O.O.T.E.D. Vol 1, future volumes |

**Wix Dashboard → Store → Collections → + New Collection**

---

## 7. Tax & Payment Notes

- **Digital products** are taxable in some US states (NY, TX, WA, etc.) — enable **Wix Tax** or connect **Avalara** for automatic calculation
- Recommended payment methods: **Wix Payments** (default) + **PayPal** for trust signals
- For international buyers: enable **Currency Converter** app from Wix App Market

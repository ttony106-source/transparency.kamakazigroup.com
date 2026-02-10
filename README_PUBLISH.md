# Governance Transparency Registry - Publish Guide

## Repository: `transparency.kamakazigroup.com`

**Owner:** Kamakazi Group LLC 
**Target URL:** `https://transparency.kamakazigroup.com`

---

## Files in This Bundle

| File | Purpose |
|------|---------|  
| `index.html` | Public-safe governance transparency registry page |
| `CNAME` | Custom domain binding for GitHub Pages |
| `robots.txt` | Search engine crawler directives |
| `README_PUBLISH.md` | This file - publish instructions |

---

## Quick Publish Steps

### 1. GitHub Pages Activation

1. Go to **Settings** > **Pages** in this repository
2. Under **Build and deployment**, select:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/ (root)**
3. Click **Save**

### 2. DNS Configuration

At your DNS provider for `kamakazigroup.com`, create:

```
Type:   CNAME
Name:   transparency
Target: ttony106-source.github.io
TTL:    300 (or default)
```

### 3. Verify & Secure

1. In **Settings** > **Pages**, confirm the custom domain shows `transparency.kamakazigroup.com`
2. Wait for DNS check to pass (green checkmark)
3. Enable **Enforce HTTPS**

### 4. Confirm Live

Once DNS propagates (typically 5-30 minutes):

```
https://transparency.kamakazigroup.com
```

Should display the Governance Transparency Registry page.

---

## Troubleshooting

- **404 error:** Ensure GitHub Pages is enabled and deploying from `main` / root
- **DNS not resolving:** Verify CNAME record points to `ttony106-source.github.io`
- **HTTPS not available:** Wait for GitHub to provision the TLS certificate (can take up to 24h)
- **Domain mismatch:** Confirm the `CNAME` file contains exactly `transparency.kamakazigroup.com`

---

*Maintained by Kamakazi Group governance operations.*

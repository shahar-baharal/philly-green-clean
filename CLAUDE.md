# Philly Green Clean — AI Agent Guide

Live at https://phillygreenclean.com. HugoBlox site, English. Phase and open items: `docs/status.md`.

## Business

**Philly Green Clean LLC**: air duct, dryer vent and chimney cleaning in Philadelphia, Montgomery, Delaware and Bucks Counties and South Jersey. A service-area business: no street address on the site.

## Key facts

- **Based on `sites/eztechrepair/`** (workspace `docs/sites/NEW-SITE-GUIDE.md`). **Theme**: `baharal-hugoblox`, the HugoBlox fork (`../../themes/baharal-hugoblox/MENASHE-FORGE.md`). No theme overrides.
- **Hosting is the exception**: Netlify, not Cloudflare, because the DNS is at Wix (`docs/status.md`). `netlify.toml` copies the Hugo and Node versions from `mise.toml`: change both together. No `.github/` workflow and no `wrangler.jsonc`, so `workflows/scripts/bump.sh` doesn't fit: bump the theme with `hugo mod get <module>@<version> && hugo mod vendor`, then push.
- **Colors**: `data/themes/philly-green-clean.toml`, from the logo (green, darkened to pass AA, and navy). **Fonts**: `data/fonts/philly-green-clean.yaml` (Playfair Display + Source Sans 3, the old site's pair).
- **Logo**: `assets/media/logo-src.svg` is the source; `logo.png` and `logo-dark.png` (navy text recolored white) are rendered from it with `magick -background none -density 400 logo-src.svg -resize x80 logo.png`. `icon.png` is the old favicon.
- **Homepage**: `data/pages/home.yaml` → `hero`, `cta-image-paragraph` (`#services`), `faq` (`#faq`), `contact-info` (`#contact`). Copy in `data/blocks/<ref>.yaml`, images in `assets/media/`.
- **Contact**: `data/contact.yaml` (phone, email). Its comment lists the static copies to update with it.
- **Local dev**: `pnpm install` (once), then `hugo server` → http://localhost:1313/.

## Documentation index

See `docs/INDEX.md`.

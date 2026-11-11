# Project Status — Philly Green Clean

Live at https://phillygreenclean.com, served by Netlify (`netlify.toml`) on every push to `main`. The domain and its DNS are at Wix, so it isn't on Cloudflare like the other sites; moving it would start with the nameservers (the private repo's `business/PHILLY-GREEN-CLEAN-DNS-TRANSFER.md`).

Moved from `hugo-local-biz` to the HugoBlox fork on 2026-11-11, with the same copy, images, hours and FAQ. Based on `sites/eztechrepair/` (workspace `docs/sites/NEW-SITE-GUIDE.md`).

## Open items

| Item | Status |
|---|---|
| Sveltia CMS at `/admin/` | Configured for hero, services, FAQ, contact and hours; uploads go into the repo (`assets/media/uploads`). Not tested in production. The domain must be in the OAuth Worker's allow-list (workspace `docs/cms/AUTH-SETUP.md`) |
| Service illustrations | 284px PNGs, shown at up to ~560px by `cta-image-paragraph`: larger originals would look sharper |
| Analytics | GTM container `GTM-NSV6FQWB` (from the old site); no GA4 property of its own |
| Contact form | None — the contact block shows phone and email only |
| French | Dropped in the move: the old `i18n/fr.yaml` was incomplete |

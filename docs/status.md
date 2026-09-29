# Project Status — Philly Green Clean

Served by Netlify from `netlify.toml` on every push to `main`. The AWS migration is parked: the domain is at Wix, which can't point the apex at CloudFront. The plan for resuming lives in the private repo's `business/PHILLY-GREEN-CLEAN-DNS-TRANSFER.md`.

## Open items

| Item | Status |
|---|---|
| Sveltia CMS at `/admin/` | Configured (migrated from Decap + DecapBridge), not yet tested in production |
| French translation | `i18n/fr.yaml` exists but is incomplete |
| Contact form | None — contact page shows phone/email only; add Netlify Forms if one is needed |

## Content decisions

- Homepage has no testimonials (removed). `data/features.json` exists but isn't in the homepage `sections` list.

# Home OS — v2

A single-file household tracker that ends in real orders: the morning digest
builds a per-vendor **order basket** — one tap shares a formatted order message
(WhatsApp/copy) respecting each vendor's payment quirks, and "Mark ordered"
updates stock and the log. Rapid "stock check" mode (tap how full each jar is),
4-field quick add, and a who-are-you picker for attribution.

**Live:** https://srijanarya.github.io/home-os-app/

Sharing across devices runs on Supabase (plain PostgREST fetch, no client lib);
until credentials are wired the app runs in local-only mode per device. The
household link (`#h=<uuid>`) is the access secret — same trust model as a
private doc link.

Planning docs (PRD + design brief) live in the private `home-os` repo; this repo
is just the deployable app. No real household data is stored in this repo.

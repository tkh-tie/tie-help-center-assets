# Assets: Install the Tie Pixel

Rendered from `visuals/*.html` by `kb_visual_render.py`; synced to github.com/tkh-tie/tie-help-center-assets by `kb_assets_sync.sh`. Re-render, never edit the PNG.

| File | Captured | Shows | Used by |
|---|---|---|---|
| shopify--01-two-pieces.png | 2026-09-28 | Diagram: loader in the theme, Customer Events pixel in settings | install-on-shopify |
| headless-shopify--01-event-split.png | 2026-09-28 | Diagram: your app vs Shopify checkout, who produces which event | install-on-headless-shopify |
| verify--01-network-200.png | 2026-09-28 | Real DevTools Network tab on a live Tie-tracked store, filter `domain:ss3.zone.* -id=G- -iframe -tp2`, loader + Tie scripts + enrich all 200 | verify-your-installation |
| verify--02-network-error.png | 2026-09-28 | Real DevTools Network tab on a local test page (127.0.0.1:8765/e404) requesting a nonexistent file on a tracking subdomain: 400 beside a 200 | verify-your-installation, no-data-after-install |
| verify--03-console-syntaxerror.png | 2026-09-28 | Real DevTools Console on a local test page with a line break inside the loader: Uncaught SyntaxError, window.dataLayer undefined | verify-your-installation, no-data-after-install |
| verify--04-tie-user-attributes.png | 2026-09-28 | Real DevTools Console on a live store: tie_user_attributes_status returns 'empty' for a fresh visitor | verify-your-installation |
| verify--06-console-events.png | 2026-09-28 | Real DevTools Console on a live store product page: rr_bot_validation, tie_user_attributes, rr_view_item | verify-your-installation |

Captured with `kb_devtools_shot.py` (scratch Chrome, undocked DevTools, CDP screenshot). Filters are chosen so no customer domain or vendor name appears. Not captured yet: the enrich CORS error on a theme preview (needs a real preview URL).

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
| shopify-custom-app--01-installed-app.png | 2026-10-21 | Settings → Apps, Installed list, Tie Integration App row highlighted | shopify-custom-app (16139668) Step 1 |
| shopify-custom-app--02-build-in-dev-dashboard.png | 2026-10-21 | App development page cropped to the Dev Dashboard card (legacy section left out), Build apps in Dev Dashboard highlighted | 16139668 2a |
| shopify-custom-app--03-create-app-fields.png | 2026-10-21 | Create an app form column, App name / App URL / Scopes highlighted with 2b / 2c / 2d badges | 16139668 2b to 2d |
| shopify-custom-app--04-scope-error.png | 2026-10-21 | Couldn't create app banner (invalid scopes: read_all_orders) above the App name card | 16139668 read_all_orders callout |
| shopify-custom-app--05-release-popup.png | 2026-10-21 | Release version popup only, Release highlighted | 16139668 2e |
| shopify-custom-app--06-install.png | 2026-10-21 | Store-side install window access list, Install highlighted | 16139668 2f |
| shopify-custom-app--07-one-install.png | 2026-10-21 | Dev Dashboard Installs card showing 1 | 16139668 2g |
| shopify-custom-app--08-copy-credentials.png | 2026-10-21 | Settings → Credentials card, both copy buttons highlighted (Client ID belongs to the deleted throwaway app) | 16139668 Step 3 |
| shopify-custom-app--09-custom-distribution.png | 2026-10-21 | Select a distribution method, Custom distribution and Select highlighted (Partners page) | 16139668 distribution |
| shopify-custom-app--10-generate-link.png | 2026-10-21 | Custom distribution form, placeholder your-store.myshopify.com, multi-store box and Generate link highlighted | 16139668 distribution |

Captured 2026-10-21 on a throwaway "Tie Integration App" created in the Revenue Roll Dev Dashboard and installed on Design Team Sandbox (Tim's go), then uninstalled and deleted. The Dev Dashboard renders dark only. Raw captures and the crop/annotation spec live in `visuals/captures/shopify-custom-app/` (not published); re-render with `kb_annotate.py`, never edit these PNGs.

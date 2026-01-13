# How to install and use this Shopify theme in any store — Step‑by‑step

Prerequisites
1. Shopify store admin access (or collaborator access with theme permissions).
2. Local copy of this theme folder.
3. Optional: Shopify CLI installed (recommended for development) or ability to upload a zip via Shopify admin.

Method A — Quick install via Shopify admin (no CLI)
1. Compress the theme folder into a single ZIP file.
2. In the target store admin go to Online Store → Themes.
3. Click “Upload theme” (top right) and select the ZIP file.
4. When upload completes, click Actions → Preview to test, Actions → Duplicate to keep a backup, and Actions → Publish when ready.
5. Open Online Store → Themes → Customize to configure settings, sections, and content.

Method B — Install and develop using Shopify CLI (recommended for iterative work)
1. Install Shopify CLI and authenticate:
    - shopify login --store your-store.myshopify.com
2. From the theme folder, preview locally:
    - shopify theme dev
3. To push the theme to the store (create or update a theme):
    - shopify theme push --store=your-store.myshopify.com
    - Or follow prompts from the CLI to choose/create a theme target.
4. In admin, verify under Online Store → Themes and publish when ready.

Post‑install checklist
1. Copy/verify content: pages, blog posts, products, collections, menus.
2. Upload images/assets that aren’t part of the theme.
3. Install any required apps and configure app settings.
4. Migrate custom data: metafields, translations, and config/settings_data.json if applicable.
5. Test responsive layout, checkout flow, and performance.
6. Set primary domain and SSL (Online Store → Domains).

Tips
- Keep a backup (duplicate) of the live theme before publishing.
- Use the CLI for faster iterative changes and live reload.
- If theme uses Shopify Functions, custom apps, or API keys, provision those in the new store first.


# Evergreen Coffee Co. website

A one-page website for Evergreen Coffee Co. on Evergreen Village Square, San Jose. Plain HTML and CSS with a little JavaScript, no build step, ready for GitHub Pages.

## What's in the folder

| File | What it is |
| --- | --- |
| `index.html` | The whole site: storefront drawing, story, favorites, full menu, the square, reviews, hours and map. The header hides while you scroll down and comes back when you scroll up. |
| `404.html` | Friendly "page not found" page (GitHub Pages uses it automatically) |
| `robots.txt`, `sitemap.xml` | Help search engines find and index the site |
| `assets/` | Logo, favicons and the image shown when the link is shared |

## Put it online with GitHub Pages

1. Create a new **public** repository on GitHub, for example `evergreen-coffee`.
2. Upload everything in this folder (keep the `assets` folder as a folder) to the repository's main branch.
3. In the repository, open **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. After a minute or two the site is live at `https://YOUR-USERNAME.github.io/evergreen-coffee/`.

## One find-and-replace before (or right after) you publish

The text `https://YOUR-SITE-URL/` appears in `index.html`, `robots.txt` and `sitemap.xml`. Replace it everywhere with your real address, ending in a slash, for example:

```
https://YOUR-USERNAME.github.io/evergreen-coffee/
```

This makes the search-engine tags and link previews (Facebook, iMessage, etc.) point at the right page.

## Updating prices or hours

- **Prices:** each price appears twice on its line in `index.html`, once as `data-p="5.95"` and once as the visible `5.95`. Change both. The search-engine menu data is built from the page automatically.
- **Hours:** update the hours table in the "Come say hi" section (the `data-open` / `data-close` times drive the "Open now" message), the footer line, and the `openingHoursSpecification` block near the top of the file.

## Accessibility (keep it ADA-friendly)

The site was built and checked against WCAG 2.1 level AA, the standard used for ADA website compliance:
every text color passes contrast, the whole page works with a keyboard (with a visible focus ring), the menu tabs work with arrow keys and screen readers, the page reflows on phones down to 320px wide and at 200% zoom, motion stops after a few seconds and is off for people who turn on "reduce motion", and there's an accessibility contact note in the footer.

When you change things later:
- Give every new photo a short `alt` description (what's in it), or `alt=""` if it's decoration.
- Stick to the colors already in the file for text and backgrounds; they're the ones that passed the contrast check.
- Keep link text meaningful ("See the menu", not "click here").

## Help Google show the shop

- Claim the shop's **Google Business Profile** and add this website address to it. That does more for local search than anything on the page itself.
- In **Google Search Console**, add the site and submit `sitemap.xml`.
- If you use a custom domain, add it under Settings → Pages and update `YOUR-SITE-URL` to match.

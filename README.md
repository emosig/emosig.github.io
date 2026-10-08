# Personal website of Eloy Mosig García

Plain HTML/CSS, no build step. GitHub Pages serves the files as they are.

## Files
- `index.html`: the whole site. Edit text and publications here.
- `style.css`: layout, colors, light/dark mode.
- `cv.pdf`: the CV linked from the page. Replace it with a new version under the same name.
- `favicon.svg`, `robots.txt`, `sitemap.xml`, `.nojekyll` (tells GitHub not to run Jekyll).

## Publish
1. On GitHub, create a public repository named exactly `emosig.github.io`.
2. Upload all the files (including `.nojekyll`) to the repository root.
3. Settings > Pages: source "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute or two the site is live at https://emosig.github.io

## Get it into Google
1. Open Google Search Console, add a "URL prefix" property for https://emosig.github.io/
2. Choose the "HTML tag" verification method, paste the tag into the marked spot in `index.html`, push, then click Verify.
3. In Search Console, submit `sitemap.xml` and use "URL inspection" > "Request indexing" on the home page.
4. Link to the site from places Google already crawls: your Google Scholar profile, ORCID, the Pisa department page, GitHub profile, LinkedIn. This matters more than anything else.
5. Unpublish the old Google Site (or replace its content with a link here) so the two don't compete.

## Adding a paper
Copy one `<li>...</li>` block inside the "Published" or "Preprints" list in `index.html`, edit it, and update `lastmod` in `sitemap.xml`.

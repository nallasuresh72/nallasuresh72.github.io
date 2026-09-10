# Blogging Guide

## One-time setup
The homepage is configured to read the public `blog/` folder from GitHub automatically.

## Every future blog
1. Create one HTML article file, for example `blog/sap-transport-management.html`.
2. Include these optional metadata tags in the `<head>`:
   - `blog-title`
   - `blog-category`
   - `blog-date`
   - `blog-description`
3. Upload **only that HTML file** into the repository's `blog/` folder.
4. Commit the change.
5. Wait for GitHub Pages to publish, then refresh the website.

The homepage discovers `.html` files in `blog/` automatically. You do not need to edit `index.html` or `site-data.js` for each new article.

## Recommended article structure
- Strong title
- Personal signature-style introduction
- Clear sections and practical explanations
- Examples where useful
- Final takeaways
- Follow/visit CTA
- Signature: `— Suresh Nalla` and your tagline

Never include client-confidential information, credentials, internal hostnames, screenshots containing sensitive data, or proprietary documents.

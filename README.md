# getbilldash.in – deployment notes

Upload the **contents** of this folder to your web root (public_html, or the repo root for static hosts).

## Files
- index.html – the landing page (CSS/JS inline, no frameworks)
- privacy-policy.html – privacy policy (review before going live; update the contact email if needed)
- 404.html – not-found page
- robots.txt, sitemap.xml – search engine files
- site.webmanifest, favicon.ico, favicon-*.png, apple-touch-icon.png – icons and web app metadata
- assets/ – logo (WebP + PNG), app icons, og-image.png for social sharing

## Hosting (Cloudflare Workers)
This folder is set up for Cloudflare. Redirect www to the apex domain with a Cloudflare Redirect Rule (dashboard > your domain > Rules > Redirect Rules > "Redirect from WWW to root"), not with a _redirects file.

## After launch
1. Submit https://getbilldash.in/sitemap.xml in Google Search Console.
2. Test structured data at https://search.google.com/test/rich-results
3. Check the social preview with a link-preview tool.

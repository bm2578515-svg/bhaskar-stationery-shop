# Bhaskar Stationery Shop — Google-ready package

## Phone testing
Keep `index.html`, `style.css`, and `manifest.webmanifest` together. Extract the ZIP and open `index.html` in Chrome.

## Customer use
Customers open the public website URL, choose Hindi or English, search/filter products, and see price, details, and In Stock / Out of Stock / Coming Soon status.

## Why Google cannot find the phone version
A page opened from a phone with a `content://` address is only a local file. It is not a public website that Google can crawl.

## How to make it searchable on Google
1. Publish the files on web hosting and get a public HTTPS URL.
2. Add and verify that website in Google Search Console.
3. Submit the site's sitemap.
4. Use URL Inspection to request indexing.
5. Later test with `site:YOUR-DOMAIN`.

Google says it automatically discovers many sites, but some can be missed; indexing is not instant and ranking is not guaranteed.

## Important admin limitation
The current demo dashboard is a front-end prototype and stores changes in browser localStorage. A real shop needs a secure backend/database so that your product and stock changes are visible to every visitor. Never put a real admin password directly in JavaScript.

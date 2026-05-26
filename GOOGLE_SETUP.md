# Google Search Setup

This page is now prepared for search engines with:

- Clear page title and description
- Indexing-friendly robots directives
- Open Graph and Twitter preview metadata
- Schema.org `ProfilePage` structured data for Shend Zhjeqi
- A `robots.txt` file allowing search crawlers

To appear in Google Search, the site still needs a public web address. Google cannot index `localhost` or files that live only on your computer.

## Recommended launch steps

1. Publish the folder to a public host, such as GitHub Pages, Netlify, Cloudflare Pages, or a University of Michigan web space.
2. Use a stable URL that includes the name, if possible, for example `https://shendzhjeqi.github.io/` or a university profile URL.
3. After the public URL exists, add this line inside the `<head>` of `index.html`, replacing the example URL:

```html
<link rel="canonical" href="https://your-public-url.example/">
```

4. Create `sitemap.xml` with the final public URLs:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://your-public-url.example/</loc>
    <lastmod>2026-05-26</lastmod>
  </url>
  <url>
    <loc>https://your-public-url.example/research.html</loc>
    <lastmod>2026-05-26</lastmod>
  </url>
  <url>
    <loc>https://your-public-url.example/talks.html</loc>
    <lastmod>2026-05-26</lastmod>
  </url>
  <url>
    <loc>https://your-public-url.example/teaching.html</loc>
    <lastmod>2026-05-26</lastmod>
  </url>
  <url>
    <loc>https://your-public-url.example/notes.html</loc>
    <lastmod>2026-05-26</lastmod>
  </url>
</urlset>
```

5. Add the public site to Google Search Console.
6. Submit the sitemap in Search Console.
7. Use URL Inspection in Search Console to request indexing for the homepage.
8. Link to the site from trusted public pages, such as a university profile, Google Scholar, arXiv author page, GitHub profile, or seminar pages.

Google can index a new page quickly, but ranking for a name search may take days or weeks and is not guaranteed.

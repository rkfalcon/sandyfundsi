# SI Sandy Relief Fund static site

This is a static capture of `http://www.sandyfundsi.org/` prepared for Vercel.

## What is included

- Public pages from the source sitemap.
- Blog posts, archive pages, category pages, and feed files discovered during the crawl.
- Same-site uploaded images and Weebly theme/script files that were still available from the source.
- Vercel static hosting config with clean URLs enabled.

## Notes

The original site was built on Weebly. Static pages and images are preserved, but hosted services such as comments, social widgets, PayPal donation flows, old analytics scripts, and third-party embeds still point to their original external providers.

The crawl reported missing obsolete Weebly theme image files that already returned `404 Not Found` from the source site. Those missing files are listed in `.crawl/manifest.json`, which is ignored from deployment.

## Local preview

```sh
npx serve public
```

## Deploy to Vercel

Import this folder into Vercel as a static project. The deploy output is the `public` directory.

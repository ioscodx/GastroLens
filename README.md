# GastroLens Official Website

Static public website for GastroLens, an AI-powered mobile app that turns dish photos into structured culinary guidance.

This repository contains the website used for:

- Landing page
- Privacy Policy
- Terms of Service
- Support page

## Overview

GastroLens helps users:

- Scan a dish
- Understand its structure and components
- Get preparation guidance
- Learn chef techniques
- Improve plating and presentation
- Share dishes through links or community/trending features

The site is built as a simple static website with no framework or build pipeline.

## Tech Stack

- HTML
- CSS
- Vanilla JavaScript

No framework dependencies.
No package manager.
No build step required.

## Search Engine Blocking

The site is configured to remain accessible by direct link while staying out of search engine results.

Current protections:

- Global `<meta name="robots">` tag on all public pages
- Root `robots.txt` blocking all crawlers
- Global `X-Robots-Tag` response header configured in `render.yaml`

Applied directives:

- `noindex`
- `nofollow`
- `noarchive`
- `nosnippet`

## Project Structure

```text
/
|-- .well-known/
|   `-- apple-app-site-association  # Universal Links association file
|-- app-ads.txt         # App-ads declaration
|-- favicon.ico         # Browser/site icon
|-- gastrolens.png      # Footer/logo asset
|-- index.html         # Landing page
|-- iphone-mockup-2.png # Current landing page preview image
|-- iphone-mockup.png   # Alternate landing preview image asset
|-- privacy.html       # Privacy Policy
|-- terms.html         # Terms of Service
|-- support.html       # Support page
|-- styles.css         # Shared site styles
|-- site.js            # Mobile navigation behavior
|-- robots.txt         # Blocks all crawlers
`-- render.yaml        # Render static-site config and headers
```

## Deployment

This site is intended for static hosting on Render with a custom domain.

Key deployment details:

- Publish directory: repository root
- Static site runtime
- Global `X-Robots-Tag` header defined in `render.yaml`
- Custom domain supported
- HTTPS enabled by the hosting platform

If you deploy this repository on Render, make sure the service uses the included `render.yaml` or replicate the same header rule in the Render dashboard.

## Legal and Support

Public pages included in this repository:

- Home: `/index.html`
- Privacy Policy: `/privacy.html`
- Terms of Service: `/terms.html`
- Support: `/support.html`

These pages include current disclosures covering:

- Privacy, subscriptions, and advertising
- Shared links, community visibility, and trending/import features

Contact:

- `contact@gastrolens.app`

## Notes

- The website is separate from the GastroLens mobile app codebase.
- If data practices, subscription behavior, or legal information change, update the legal pages in this repository.
- If sharing, community, or trending behavior changes in the app, update the Privacy Policy, Terms of Service, and Support pages in this repository.

Copyright 2026 GastroLens. All rights reserved.

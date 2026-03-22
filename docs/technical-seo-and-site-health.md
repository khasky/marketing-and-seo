[← SEO — FAQ, keywords, and tools](seo-tools-and-faq.md) · [Measurement →](measurement-attribution-and-experimentation.md)

# Technical SEO and site health

Crawlability, indexing, performance, and structured data — the layer that lets content and links work. Use with [keyword strategy](seo-tools-and-faq.md), [content](content-seo-and-blog.md), and [landing structure](landing-pages.md).

Official references change; verify on [Google Search Central](https://developers.google.com/search/docs).

## How this fits “best practice”

Technical SEO lines up with Search Essentials (helpful, reliable, people-first content), Page Experience signals, and clear implementation — not tricks.

## Crawling and indexing

- Discoverable links — important URLs reachable by `<a href>` from known pages; avoid orphans.
- Indexability — `noindex` only where it belongs (thin faceted URLs, staging); avoid accidental noindex on money pages.
- Google Search Console — Coverage / Pages report, URL Inspection, Sitemaps submission, removals for emergencies.

## `robots.txt` and robots meta

- **`robots.txt`** — crawl hints; do not rely on it alone for secrets.
- **Meta robots** — `noindex` for pages that should not appear in search results.
- **Google-specific** — confirm `googlebot` can render critical content (avoid hiding main text behind interactions without testing).

## Canonical URLs and duplicates

- One preferred URL per conceptual page; use `rel=canonical` for near-duplicates (tracking params, print views, HTTP/HTTPS variants).
- Parameter strategy — strip or consolidate UTM-only variants; avoid infinite faceted URL spaces ([Marketing II — duplicate caution](marketing-pages-and-attribution.md)).
- Redirects — 301 permanent moves; fix chains and loops.

## HTTPS and security

- HTTPS everywhere; mixed content undermines trust and can break features.
- HSTS when you are ready operationally.
- Match security copy to [Legal](legal-compliance.md) and what you actually do.

## Mobile and responsive design

- Mobile-first indexing — Google predominantly uses the mobile version.
- Viewport and tap targets — readable text without horizontal scroll; buttons spaced for touch.
- Interstitials — aggressive app-install or email gates can hurt UX and SEO on mobile ([Content — overlays](content-seo-and-blog.md)).

## Core Web Vitals (field metrics)

User-centric performance signals (check current docs):

- **Largest Contentful Paint (LCP)** — loading performance.
- **Interaction to Next Paint (INP)** — responsiveness (successor focus to older FID-style thinking).
- **Cumulative Layout Shift (CLS)** — visual stability.

Measure with CrUX, PageSpeed Insights, or GSC experience reports; fix templates that carry the most traffic first.

## Site architecture and internal linking

- Depth — key pages within a few clicks of home; breadcrumbs where they help.
- Hub and spoke — pillar plus supporting articles with descriptive anchors ([internal linking](content-seo-and-blog.md)).
- Faceted navigation — manage crawl budget on large sites (parameter handling, sitemap discipline).

## XML sitemaps

- Submit sitemaps in GSC; include `lastmod` where it is accurate.
- Split large sites by section or type; priority tags are weak signals — focus on coverage and freshness.

## Structured data (schema.org)

Markup can qualify you for rich results (not guaranteed):

- `Organization` / `WebSite` — site-level; optional sitelinks searchbox where valid.
- `Product` / `SoftwareApplication` — SaaS-friendly patterns when truthful.
- `FAQPage` — only if FAQs are visible on-page.
- `BreadcrumbList` — mirrors visible breadcrumbs.

Validate with Rich Results Test; avoid spammy or misleading schema.

## International and multilingual

- **`hreflang`** — tie language/region variants; `x-default` where appropriate.
- URL strategy — subdomains vs subfolders vs ccTLDs is an SEO plus ops tradeoff; pick one model and stay consistent.

## Local SEO (when relevant)

If geography matters (services, retail, regional SaaS):

- Google Business Profile accuracy; NAP consistency (name, address, phone) across listings.
- Local landing pages — unique copy per location; avoid duplicate city pages.

## Handy Search Central entry points

- [How Google Search works — overview](https://developers.google.com/search/docs/fundamentals/how-search-works)
- [Technical SEO](https://developers.google.com/search/docs/technical)
- [Page Experience](https://developers.google.com/search/docs/appearance/page-experience)

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [SEO — FAQ, keywords, and tools](seo-tools-and-faq.md) | [Home](index.md) | [Measurement](measurement-attribution-and-experimentation.md) |

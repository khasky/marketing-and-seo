[← Technical SEO](technical-seo-and-site-health.md) · [Paid remarketing →](paid-media-remarketing.md)

# Measurement, attribution, and experimentation

What to measure, how channels get credit, and how to run tests without fooling yourself. Links [product analytics](product-and-ux.md), [UTMs](marketing-pages-and-attribution.md), [paid tagging](paid-media-remarketing.md), and [legal consent](legal-compliance.md).

## Principles

- Metrics you can act on beat vanity dashboards — tie reports to weekly or monthly decisions.
- Leading vs lagging — activation and engagement often lead revenue; still check cohort revenue eventually.
- Consistency — same event definitions in product, site, and ads where possible.

## North Star and OMTM

- **North Star** — one outcome that reflects real value (e.g. weekly active teams finishing a core workflow).
- **One Metric That Matters (OMTM)** — for a given quarter, the single number the team optimizes (may differ from North Star during a phase).

Do not optimize pageviews or raw signups without quality and retention guardrails ([Frameworks](frameworks-and-retention.md)).

## Google Analytics 4 (GA4) — marketing essentials

- **Events** — implement key funnel steps (`sign_up`, `begin_trial`, `purchase`, `generate_lead`) with stable names.
- **Conversions** — mark a few primaries; too many dilutes reporting.
- **Audiences** — build segments for remarketing export to Google Ads ([Paid](paid-media-remarketing.md)).
- **Reports** — Traffic acquisition (channel grouping), Landing page, Path exploration for journeys.

Link GA4 and Google Ads; use Google signals only where privacy settings allow.

## Search Console + Analytics together

- **GSC** — queries, impressions, clicks, positions per page ([Technical SEO](technical-seo-and-site-health.md)).
- **GA4** — on-site behavior after the click.
- Together: high-impression / low-CTR titles vs high-CTR / low-conversion landings.

## UTM hygiene

Use one convention across teams ([example](marketing-pages-and-attribution.md)):

- Required: `utm_source`, `utm_medium`, `utm_campaign`; add `utm_content` for creative variants.
- Lowercase, hyphenated slugs reduce fragmentation.
- Document active campaigns so reports stay readable.

## Attribution models (limitations)

- **Last-click** — simple; undervalues assist channels.
- **Data-driven** (where available) — modeled credit; still not ground truth.
- **Incrementality** — geo holdouts, lift studies, PSA tests for brand/paid when budget allows ([Remarketing — incrementality](paid-media-remarketing.md)).

Report multiple views: channel performance, campaign ROI, cohort LTV.

## Experimentation

- **A/B tests** — change one main factor; run until power is adequate (watch peeking bias).
- **Feature flags** — ship safely; split release risk from experiment readout ([Product](product-and-ux.md)).
- **Holdout groups** — long-term no-email or no-discount cells for incremental proof.

## Consent, cookies, and data quality

- In regulated regions, consent mode affects observed vs modeled conversions — align tagging with [Cookie / CMP](legal-compliance.md).
- iOS ATT and browser limits shrink retargeting pools; first-party lists and CRM reconciliation matter more.

## Stack hygiene

- **Naming** — GA4 events, tag manager containers, and ad pixels labeled by owner and date.
- **QA** — staging GTM preview, Tag Assistant, Meta Test Events before launches.
- **Retention** — analytics data retention settings vs business needs.

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [Technical SEO](technical-seo-and-site-health.md) | [Home](index.md) | [Paid remarketing](paid-media-remarketing.md) |

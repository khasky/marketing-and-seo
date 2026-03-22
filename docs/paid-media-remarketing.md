[← Measurement](measurement-attribution-and-experimentation.md) · [Frameworks →](frameworks-and-retention.md)

# Paid media — remarketing and retargeting

How retargeting works on major ad platforms. For search ads that catch existing demand, see [Marketing I — Paid search (SEM)](marketing-acquisition-and-channels.md). Check consent, cookie banners, and platform policies with counsel before you ship tags.

## Definitions

- **Remarketing** — Google’s label for ads to people who already visited your site or app (people often say “retargeting” instead).
- **Retargeting** — the same idea on Meta, LinkedIn, and elsewhere: bring back people who already touched your brand.

## Why it works

People who visited, started signup, or looked at pricing often convert better than cold traffic, if you manage creative, frequency, and exclusions.

## Audience ladder (example)

Build nested audiences from broad to narrow:

1. All site visitors (7–30 days) — light brand reminder.
2. Engaged — two or more pages, sessions over about a minute, or scroll-depth events.
3. Feature or pricing viewers — objection handling, comparison, ROI proof.
4. Cart, checkout, or trial abandoners — reminder plus support or a limited offer.
5. Customers — upsell, referral, new feature (exclude recent purchasers so you do not waste discount ads).

## Platform building blocks

### Google Ads + GA4

- **Tag:** Google tag (gtag) or GTM; link Google Ads and GA4.
- **Audiences:** build in GA4 (e.g. segment on `begin_checkout`) and share to Google Ads.
- **RLSA (Search):** bid adjustments for past visitors searching Google — usually high intent.
- **Display / YouTube:** remarketing lists for website and YouTube engagement.
- **Dynamic remarketing:** feed products or services into creative — [Google Ads dynamic remarketing](https://support.google.com/google-ads/answer/3103357).

### Meta (Facebook / Instagram)

- Meta Pixel plus Conversions API (CAPI) for resilience as ATT and privacy rules tighten.
- Custom audiences: site, app, customer list (hashed email), engagement (video, lead form).
- Watch frequency and rotate creative; social feeds burn out fast.

### LinkedIn

- Insight Tag and matched audiences (retarget site, upload lists).
- Works when your ICP lines up with LinkedIn’s graph.

### Others

- TikTok Pixel, X, Pinterest — same pattern: pixel, list, suppression rules.

## Pixels and tagging

Common paths:

- **Tag Manager** — one place for Meta, Google Ads, LinkedIn, TikTok pixels.
- **Native integrations** (Shopify, Webflow) — fastest, less flexible.
- **Hard-coded** header — fine for small sites only.
- **Server-side / CAPI** — Meta CAPI, Google enhanced conversions — helps as third-party cookies weaken.

Put base tags early in `<head>` per vendor docs; test with Tag Assistant or Meta Test Events.

## Consent and privacy

- In the EEA, UK, and CH, consent mode and CMP choices affect whether ad tags fire for measurement — see [Legal — Cookie consent](legal-compliance.md).
- iOS ATT and browser tracking limits mean smaller retargeting pools; first-party data and CRM sync matter more.

## Creative and frequency

- Rotate ads to limit fatigue; use frequency caps (e.g. 5–7 per week on social as a starting band — measure your own).
- Sequential storytelling: education, then demo, then offer.
- Exclude recent converters from “signup” campaigns so you do not pay twice.

## Measurement

- Put UTMs on every destination URL — [Marketing II — UTMs](marketing-pages-and-attribution.md).
- Link GA4 and Google Ads; use consent mode diagnostics where relevant.
- Incrementality: geo or holdout tests when budget allows; retargeting often assists conversions also credited to search or brand.

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [Measurement](measurement-attribution-and-experimentation.md) | [Home](index.md) | [Frameworks](frameworks-and-retention.md) |

[← Marketing I](marketing-acquisition-and-channels.md) · [Content, blog, and link building →](content-seo-and-blog.md)

# Marketing II — Pages, attribution, and programs

Audience-specific pages, competitive landing matrices, UTMs, referrals, influencers, and feedback loops.

## FOR promo pages (audience-specific landing pages)

**Goal:** traffic plus segmented messaging.

### Duplicate content caution

Google tries to canonicalize or demote near-duplicate pages. If you spin many URLs with tiny swaps, add real differentiation:

- Unique headlines, proof, use cases, FAQs, schema where valid.
- Internal linking from hub to spoke.
- Avoid thin permutations; merge or 301 true duplicates.

Implementation: `rel=canonical`, redirects, and parameter handling — [Technical SEO](technical-seo-and-site-health.md).

Ahrefs “SEO for X vertical” pages are templated but substantively varied: [ahrefs.com/seo](https://ahrefs.com/seo) and `/seo/for/...` routes.

### Persona / vertical ideas

Bloggers, streamers, entrepreneurs, freelancers, teams, e-commerce, agencies, startups, B2B, SMB, enterprise, nonprofits, influencers, etc. — pick segments where you have proof.

## Comparison with competitors

**Goal:** capture solution-aware searchers.

**Matrix idea:** with ~N competitors, you can build alternatives, vs, pricing, review, and migration pages — some teams plan dozens of URLs for deep competitive SEO (illustrative math).

**Content**

- Honest feature comparison; update quarterly.
- Switching steps; importer links.
- Testimonials from switchers per competitor when possible.

Examples: [Klenty vs Reply](https://www.klenty.com/compare/reply), [Postoplan alternative](https://postoplan.contenive.com/free_alternative_to_sprout), [Kontentino vs Buffer](https://www.kontentino.com/kontentino-vs-buffer/), [Agorapulse Hootsuite alternatives](https://www.agorapulse.com/hootsuite-alternatives/), [Social Champ Buffer alternatives](https://www.socialchamp.io/buffer-alternatives/).

## Competitor migration pages

Example pattern: [Sociality migration guides](https://sociality.io/migration-guides) — step-by-step export/import, checklists, and support CTA.

## FREE tools section

**Goal:** programmatic traffic via micro-tools.

Examples unrelated to a single product: TikTok hashtag generator, WhatsApp link generator, social ROI calculator, Instagram utilities, UTM builder.

Starters: [CoSchedule headline analyzer](https://coschedule.com/blog-title-analyzer), [Learn with Hasan tools](https://learnwithhasan.com/tools/).

**SEO:** one tool per URL, fast LCP, clear primary CTA to your core product.

## Referral programs

- Referrals can convert roughly 4× vs cold traffic in some studies; margins can improve with lower CAC.
- Dropbox-style double-sided rewards are the classic SaaS pattern.
- At scale, use FirstPromoter, PartnerStack, or similar to track payouts and fraud.

## Influencer marketing

Further reading:

- [Sociality — find influencers](https://sociality.io/blog/how-to-find-social-media-influencers/)
- [Buffer — micro-influencers](https://buffer.com/resources/micro-influencers/)
- [Quuu — connect with influencers](https://blog.quuu.co/how-to-connect-with-influencers/)

Tools: BuzzSumo, Socialbakers (verify current product names).

Micro-influencers often deliver better CPE than celebrities for niche B2B.

## Competitors traffic investigation

Use Similarweb (or similar) Referrals tab to see who sends traffic to competitors — prospect those sites and partnerships.

## Newsjacking

Often stronger for social than long blog cycles.

Definition: attach a timely, credible angle to breaking news for media or feed pickup.

Rules:

- Speed — news decays in hours.
- Original insight, not rewritten wire copy.
- Monitor keywords and hashtags; verify facts.

## UTM meta for social sharing

**Why:** share buttons and copy-paste links often strip analytics context unless you tag them.

Guidance:

- Put UTMs on every share URL; optionally run through a shortener that still preserves or logs parameters.

Parameters:

| Parameter | Typical use |
|-----------|-------------|
| `utm_source` | `twitter`, `newsletter`, `linkedin` |
| `utm_medium` | `social`, `email`, `referral` |
| `utm_campaign` | launch or content slug |
| `utm_content` | which button or creative variant |
| `utm_term` | paid keywords (optional) |

Example: `?utm_source=gitlab&utm_medium=referral&utm_campaign=readme-badge&utm_content=screenshot-gallery`

Align with [GA4 custom channel rules](https://support.google.com/analytics) in your analytics admin.

## Browser extensions

**Only if applicable** — extensions can be high-retention distribution for workflow products (e.g. SEO, writing, social). Plan Chrome Web Store compliance, privacy manifest, and update overhead.

## Feedback / survey for reward

**Template** (edit heavily — comply with platform review policies and local marketing law):

> We would love to hear from you!
> As a valued user, please share your experience on [G2 / Capterra / Trustpilot]. We appreciate your time — [incentive disclosure].
> [Submit review]

**Requirements**

- Disclose incentives; many review sites ban compensated reviews or require specific disclosure flows.
- Never buy fake reviews.

## Customer satisfaction measurement

CSAT via email or phone, plus surveys.

- NPS — relationship pulse; follow with driver questions.
- CES — ease of key flows (upgrade, onboarding).
- In-product micro-polls after successful actions.
- Close the loop: tag feedback in CRM and reply when you ship fixes.

## LinkedIn outreach and sponsored messaging

Product promo in DMs is a known pattern — verify current LinkedIn rules and frequency limits before scaling creative that pushes offers in inbox threads.

### Organic (free) private messages

- Personalize with role, company trigger, or mutual context; short messages (under ~100 words often cited) outperform essays.
- Value first — insight, template, or intro — not an instant demo ask.
- Multi-touch sequences across email and LinkedIn over 2–3 weeks; many replies arrive on follow-ups.
- Timing — business hours in the recipient timezone; test Tuesdays–Thursdays.
- Respect LinkedIn limits and anti-spam policies; automation tools carry account risk.

### Paid: Message Ads and Conversation Ads

LinkedIn’s Sponsored Messaging products reach members in their inbox with controlled frequency (platform rules limit how often someone sees sponsored messages). Conversation Ads support branching CTAs and longer copy; specs and limits change — use LinkedIn’s official help:

- [Sponsored Messaging — overview](https://www.linkedin.com/help/lms/answer/a421723)
- [Conversation ads](https://www.linkedin.com/help/lms/answer/a425071)
- [Conversation ads specifications](https://www.linkedin.com/help/lms/answer/a426057)

**Practice:** align paid inbox creative with organic voice; avoid duplicate outreach to the same people from sales and ads.

## Global landing banners (design flag)

Optional site-wide strip (sometimes disabled in favor of in-page CTAs) — a thin top-of-site bar (fixed height, single message) keeps CLS low if you reserve layout space.

### When to use

- Time-bound promos (webinar, launch week, conference).
- Segmented offers (e.g. “For agencies — book a demo”) with a single CTA.
- Dismissible strip so returning users are not trapped.

### Implementation

- Do not hurt CLS — reserve height in layout; avoid layout shift.
- Contrast and focus order for accessibility (keyboard plus screen readers).
- One primary message; rotate creative rather than stacking multiple banners.
- Cookie / consent: if the banner loads tracking, tie it to your CMP (see [Legal — Cookie consent](legal-compliance.md)).

### When to skip

- Always-on marketing chrome can train users to ignore the whole site chrome — prefer in-page CTAs for evergreen conversion.

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [Marketing I](marketing-acquisition-and-channels.md) | [Home](index.md) | [Content](content-seo-and-blog.md) |

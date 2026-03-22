[← Brand, positioning, and messaging](brand-positioning-and-messaging.md) · [Landing pages →](landing-pages.md)

# Legal, privacy, and trust

**Disclaimer:** This chapter summarizes operational patterns from public compliance guidance. It is not legal advice. Use qualified counsel for Terms, Privacy, cookies, refunds, and cross-border data rules.

## NDA and partner agreements

**Templates and generators** as starting points:

- Prefer counsel-reviewed document templates.
- Generator example: [Policymaker — NDA](https://policymaker.io/non-disclosure-agreement/) — treat as a starting point only; replace with your counsel’s jurisdiction-specific MNDA.

**Practice**

- Match NDA scope to jurisdiction and mutuality (one-way vs mutual).
- For partnerships, separate commercial terms from confidentiality.

## Legal pages — ToS, Privacy Policy, Cookies, GDPR alignment

### Generators and checklists

- [Policymaker.io](https://policymaker.io/) — generator starting point.
- Cookie / compliance context: [Cookie Law / OneTrust resource area](https://www.cookielaw.org/) (verify current product naming).

### Why these pages matter for marketing and SEO

Terms of Service and Privacy Policy show that a site is run by a real organization; they support trust signals that quality raters look for alongside other E-E-A-T signals (experience, expertise, authoritativeness, trust).

### GDPR-flavored rights (summary)

European users’ rights commonly highlighted in policies include:

- Confirmation of whether personal data is processed, and access to categories, purposes, recipients, retention.
- Rectification and, in many cases, erasure (“right to be forgotten”) and restriction of processing.
- Data portability in a machine-readable form.
- Objection to certain processing (including marketing).
- Withdraw consent as easily as it was given.

**Consent UX:** avoid pre-ticked boxes; silence or inactivity is not valid consent; document how to withdraw consent clearly.

Further reading: [AIN.UA — why a privacy policy matters under GDPR](https://ain.ua/ru/2018/05/07/zachem-nuzhna-privacy-policy-i-chto-v-nej-menyaet-gdpr/).

### Example policy pages (style references)

SaaS and marketing tools’ policies as structural examples — compare sections, not copy/paste:

- [Thrive Health privacy notice](https://www.thrive.health/privacy-notice)
- [Kontentino privacy](https://www.kontentino.com/privacy-policy/)
- [Sitecore privacy](https://www.sitecore.com/legal/privacy-policy)
- [HeyOrca privacy](https://www.heyorca.com/privacy-policy)
- [MailerLite privacy](https://www.mailerlite.com/legal/privacy-policy)
- [SocialPilot privacy](https://www.socialpilot.co/privacy-policy)
- [Quuu privacy](https://quuu.co/privacy)

**Terms of service examples:** [Kontentino ToS](https://www.kontentino.com/terms-of-service/), [MailerLite legal](https://www.mailerlite.com/legal), [HeyOrca ToS](https://www.heyorca.com/terms-of-service), [SocialPilot terms](https://www.socialpilot.co/terms), [Quuu terms](https://quuu.co/terms).

**GDPR / security program pages:** [MailerLite GDPR](https://www.mailerlite.com/gdpr-compliance), [HeyOrca GDPR](https://www.heyorca.com/gdpr), [HeyOrca subprocessors](https://www.heyorca.com/gdpr/subprocessors), [ActiveCampaign GDPR overview](https://www.activecampaign.com/legal/gdpr-updates/gdpr-overview), [HeyOrca data security](https://www.heyorca.com/data-security).

### Cookie policy copy references

- [Quuu cookies](https://quuu.co/cookies)
- [Kontentino cookies policy](https://www.kontentino.com/cookies-policy/)

## Cookie consent / cookie banner

Major SaaS and publisher sites (Cloudflare, Sitecore, Atlassian, and many others) show common patterns: Accept / Reject / Manage, preference centers, and granular toggles — use them as UX references, not copy/paste legal text.

### When you need a banner

If you use non-essential cookies or similar tech (many analytics, ads, heatmaps, A/B tools, embedded social pixels), you typically need prior consent in EU/EEA/UK-style regimes — strictly necessary cookies (session, security, load balancing in many cases) are narrower.

### Valid consent properties

- Freely given — avoid cookie walls that force accept for basic access where regulators disallow it.
- Specific / granular — per purpose (analytics vs ads), not only “accept all.”
- Informed — link to cookie policy; explain purposes and third parties at a useful level.
- Unambiguous affirmative action — no pre-checked non-essential toggles.
- Easy withdrawal — reopen preferences anytime.

### Consent Management Platforms (CMPs)

CMPs help store consent strings, integrate with Google Consent Mode (including v2 requirements for ads personalization and measurement in the EEA/UK where applicable), Tag Manager, and keep logs for audits.

- **Google’s CMP partner program** — filter certified vendors by tier, region, and integrations: [Google CMP Partner Program](https://cmppartnerprogram.withgoogle.com/).
- **GA4** — how consent mode interacts with tagging: [GA4 consent banner guidance](https://support.google.com/analytics/answer/14546213).
- **AdSense / publishers** — consent requirements for ads in EEA/UK/CH: [Google AdSense consent requirements](https://support.google.com/adsense/answer/13554116).

Pick a CMP that matches your ad stack and jurisdictions; legal review still matters.

## GDPR implementation (product checklist)

- Cookies — consent and granular controls where required; preference center.
- Logging — document processing activities where required (ROPA) with counsel.
- Privacy Policy — what you collect, why, retention, legal bases, subprocessors.
- User control
  - Edit profile data in product.
  - Delete account and data — including backup mirrors where feasible (process plus timelines).
  - Export data in common formats (CSV, JSON) on request or self-serve.

Cross-link: [Product UX — settings](product-and-ux.md).

## Refund and credit policy (REP)

A common SaaS-style policy pattern (examples: [Dowize refund](https://site.dowize.co/refund-policy/), [Drumup refund](https://drumup.io/refund-policy)).

### Philosophy

- Refunds — when the service failed obligations.
- Credits — good-will for non-use, performance issues, or missed expectations short of a hard refund obligation.
- No refund — subjective “didn’t get results” when the service worked as contracted.

### Example triggers (illustrative — adapt legally)

**Refunds**

- Double charge, billing after documented cancellation, unused product in a short window (partial 1–2 months max in some policies), cancellation within 1–3 days of renewal (if you choose to offer).

**Credits**

- Forgotten subscription (time-boxed), promised feature delays, performance issues, missed non-renewal notice if you want to preserve LTV.

**No refund**

- “Did not get desired results” if SLA met, purchase by former employee, subjective value disputes without defect.

Always align copy with card network, App Store, and local consumer rules.

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [Brand, positioning, and messaging](brand-positioning-and-messaging.md) | [Home](index.md) | [Landing](landing-pages.md) |

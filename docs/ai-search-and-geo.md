[← Technical SEO](technical-seo-and-site-health.md) · [Measurement →](measurement-attribution-and-experimentation.md)

# AI search and GEO

How to stay visible when answers come from AI Overviews, ChatGPT, Perplexity, and Claude instead of ten blue links. Builds on [Technical SEO](technical-seo-and-site-health.md) and [content](content-seo-and-blog.md); measurement caveats connect to [Measurement](measurement-attribution-and-experimentation.md).

This area moves fast; verify bot names and vendor policies against current documentation.

## Why AI search matters now

- AI Overviews answer more queries directly on the results page — zero-click intensifies, especially for informational intent.
- ChatGPT, Perplexity, and Claude are referral surfaces in their own right: cited sources get clicks, everyone else gets paraphrased.
- Brand mentions in training and retrieval corpora are becoming an acquisition asset — a model that "knows" your product recommends it unprompted.
- The practical shift: optimize to be cited and recommended, not only ranked.

## GEO — be the citable source

Generative engines quote sources that are easy to quote:

- **Clear claims** — one verifiable statement per sentence beats hedged paragraphs; engines lift sentences, not essays.
- **Original data** — benchmarks, surveys, and numbers you produced; summaries of other people's data rarely earn citations.
- **Named entities** — use product, company, and category names consistently; ambiguity breaks retrieval.
- **Consistent facts across pages** — pricing, feature claims, and positioning should not contradict between landing pages, docs, and blog ([Brand](brand-positioning-and-messaging.md)).
- **Structured data still pays** — the schema work from [Technical SEO](technical-seo-and-site-health.md) feeds the same pipelines.
- **Quotable summary blocks** — a short factual answer near the top of key pages (what it is, who it is for, what it costs) gives engines something safe to lift with attribution.

## llms.txt

A plain Markdown file at `/llms.txt` that points AI systems at your most important pages with short descriptions — a sitemap for reading rather than indexing.

- **When to bother** — docs-heavy products and content sites benefit; a five-page brochure site does not need one.
- **Keep it honest and small** — a curated list of pages that actually answer questions; padding it with every URL defeats the purpose.
- Adoption by engines is uneven; treat it as cheap insurance, not a ranking lever.

## AI crawler policy

Decide deliberately which AI bots may read your site. The common user agents:

| Bot               | Operator  | Blocking mostly affects                |
| ----------------- | --------- | -------------------------------------- |
| `GPTBot`          | OpenAI    | training corpora                       |
| `ClaudeBot`       | Anthropic | training corpora                       |
| `PerplexityBot`   | Perplexity | retrieval and citations               |
| `Google-Extended` | Google    | Gemini training (not Search ranking)   |

- Blocking in `robots.txt` is a business decision — training exposure versus referral and recommendation traffic — not a security default.
- Publishers selling content have a real case to block; most SaaS and content-marketing sites benefit from being read.
- Whatever you choose, document the choice and the reasoning, and revisit it yearly as the bots and their behavior change.

## Measuring AI referrals

- **Referral segments** — group `chatgpt.com`, `perplexity.ai`, `claude.ai`, `gemini.google.com`, and copilot referrers into one "AI surfaces" channel in GA4.
- **Branded-search lift** — a useful proxy: recommendations inside chat sessions surface later as branded queries in GSC ([Measurement](measurement-attribution-and-experimentation.md)).
- Attribution here is even weaker than usual: most AI exposure produces no click and no referrer at all. Treat AI referral numbers as a floor, not a measurement.

## Consent Mode v2 note

Where EU traffic meets Google ads or analytics, Consent Mode v2 is table stakes:

- Without it, Google Ads audience and conversion features degrade for EEA traffic.
- GA4 fills consent gaps with behavioral modeling — modeled conversions are estimates, with wider error bars on low-traffic sites.
- Implementation and CMP choice live in [Legal, privacy, and trust](legal-compliance.md); reporting impact in [Measurement](measurement-attribution-and-experimentation.md). This chapter only flags the dependency.

## Product-led loops

Marketing surfaces owned by product, not by the marketing team:

- **Invites** — collaboration features that require bringing a colleague.
- **Shared artifacts** — links, embeds, and exports that circulate with your branding attached.
- **Public outputs with backlinks** — user-generated pages, profiles, and badges that accumulate links and mentions — the same mentions AI corpora ingest.

Where they beat paid channels: acquisition cost approaches zero at scale and compounds with usage, while paid CAC rises with spend. Where they do not: pre-product-market fit, and products with no natural sharing moment — do not force one. Coordinate with [Product UX](product-and-ux.md).

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [Technical SEO](technical-seo-and-site-health.md) | [Home](index.md) | [Measurement](measurement-attribution-and-experimentation.md) |

# Marketing and SEO Playbook

Practical marketing and SEO guide for founders, product teams, and early-stage operators who need a clearer path from positioning to acquisition, measurement, and retention.

> *If I were defining go-to-market defaults for a product team today, I would start with five things first: a narrow audience, a credible message, pages that convert, measurement you can trust, and acquisition loops that compound instead of spike once and disappear.*

---

## Table of Contents

- [Marketing and SEO Playbook](#marketing-and-seo-playbook)
  - [Table of Contents](#table-of-contents)
  - [Why this exists](#why-this-exists)
  - [Companion playbooks](#companion-playbooks)
  - [The defaults I'd reach for first](#the-defaults-id-reach-for-first)
  - [How this repository is organized](#how-this-repository-is-organized)
  - [Recommended reading path](#recommended-reading-path)
  - [Guide map](#guide-map)
    - [Market, positioning, and trust foundation](#market-positioning-and-trust-foundation)
    - [Site, product, and conversion surface](#site-product-and-conversion-surface)
    - [Acquisition, content, and SEO execution](#acquisition-content-and-seo-execution)
    - [Measurement, paid loops, and retention](#measurement-paid-loops-and-retention)
  - [A practical operating model](#a-practical-operating-model)
  - [Things I would avoid](#things-i-would-avoid)
  - [References and inspiration](#references-and-inspiration)
    - [Official and high-signal references](#official-and-high-signal-references)
    - [Similar or adjacent GitHub repositories](#similar-or-adjacent-github-repositories)
  - [License](#license)

---

## Why this exists

Most marketing advice becomes harder to use the moment a team tries to apply it.

The problem is usually not lack of tactics. The problem is lack of structure:

- positioning, pages, content, SEO, and paid acquisition are treated like separate disciplines instead of one system;
- channel execution starts before the team is clear on audience, message, and proof;
- analytics gets added late, so reporting looks busy but does not support real decisions.

This repository is meant to be a more usable default.

It keeps the material in focused Markdown guides, but the underlying goal is simple: give teams a playbook they can read in sequence, revisit by topic, and use as a practical operating reference.

---

## Companion playbooks

These repositories form one playbook suite:

- [AI-Assisted Engineering Playbook](https://github.com/khasky/ai-assisted-engineering-playbook) — agent workflows, guardrails, and quality control for AI-heavy teams
- [API Design Playbook](https://github.com/khasky/api-design-playbook) — versioning, pagination, idempotency, error contracts, and webhooks
- [Auth & Identity Playbook](https://github.com/khasky/auth-identity-playbook) — sessions, tokens, OAuth, and identity boundaries across the stack
- [Backend Architecture Playbook](https://github.com/khasky/backend-architecture-playbook) — APIs, boundaries, OpenAPI, persistence, and errors
- [Best of JavaScript](https://github.com/khasky/best-of-javascript) — curated JS/TS tooling and stack defaults
- [Caching Playbook](https://github.com/khasky/caching-playbook) — HTTP, CDN, and application caches; consistency and invalidation
- [Code Review Playbook](https://github.com/khasky/code-review-playbook) — PR quality, ownership, and review culture
- [DevOps Delivery Playbook](https://github.com/khasky/devops-delivery-playbook) — CI/CD, environments, rollout safety, and observability
- [Engineering Lead Playbook](https://github.com/khasky/engineering-lead-playbook) — standards, RFCs, and technical leadership habits
- [Frontend Architecture Playbook](https://github.com/khasky/frontend-architecture-playbook) — React structure, performance, and consuming API contracts
- [Git Collaboration Playbook](https://github.com/khasky/git-collaboration-playbook) — branching, stacked PRs, merge queues, and CI collaboration at scale
- **Marketing and SEO Playbook** — growth, SEO, experimentation, and marketing surfaces
- [Messaging & Async Playbook](https://github.com/khasky/messaging-and-async-playbook) — queues, events, outbox, idempotent consumers, and retries
- [Monorepo Architecture Playbook](https://github.com/khasky/monorepo-architecture-playbook) — workspaces, package boundaries, and shared code at scale
- [Node.js Runtime & Performance Playbook](https://github.com/khasky/nodejs-runtime-performance-playbook) — event loop, streams, memory, and production Node performance
- [Observability Playbook](https://github.com/khasky/observability-playbook) — logs, traces, metrics, SLOs, and production visibility
- [React Cross-Platform Playbook](https://github.com/khasky/react-cross-platform-playbook) — shared React UI and logic across web and native with TypeScript
- [Software Design Playbook](https://github.com/khasky/software-design-playbook) — separation of concerns, composition, and module boundaries
- [State Management Playbook](https://github.com/khasky/state-management-playbook) — client state architecture, MobX, and choosing a state layer
- [Styling Architecture Playbook](https://github.com/khasky/styling-architecture-playbook) — type-safe styling, design tokens, and theming at scale
- [Testing Strategy Playbook](https://github.com/khasky/testing-strategy-playbook) — unit, integration, contract, E2E, and CI-friendly test layers

---

## The defaults I'd reach for first

If I were helping a product team build early marketing and SEO momentum today, I would usually start here:

- **Audience:** define one narrow ICP and one clear wedge before scaling channels
- **Positioning:** make the value proposition legible in a sentence the market actually uses
- **Trust:** publish real company, policy, and contact signals early
- **Website:** make landing, pricing, feature, and comparison pages work before trying to buy more traffic
- **Measurement:** define activation, conversion, and retention events before serious campaign spend
- **SEO:** treat search as intent matching plus technical hygiene plus credible content
- **Content:** build a few strong pillar assets before producing large volumes of thin posts
- **Acquisition:** use channels you can test cheaply and repeat, not just launch-day spikes
- **Paid media:** use paid search and remarketing to capture and re-engage demand, not to paper over weak positioning
- **Retention:** connect acquisition to onboarding, product value, and save flows so marketing is not judged only by signup volume

That model is intentionally boring. Boring is good when you want something repeatable.

---

## How this repository is organized

Unlike the other playbooks in this suite, this repository keeps most of the deep content in `docs/` instead of one giant root `README`.

That is a valid structure for this topic. Marketing and SEO often work better as linked reference chapters because teams revisit specific areas at different times:

- positioning when the product category shifts;
- landing and feature pages when conversion drops;
- technical SEO when content is live but search visibility lags;
- attribution when channels start competing for credit.

Use this `README` as the front door, and use the chapter files in `docs/` as the working handbook.

---

## Recommended reading path

Not every team needs every chapter in order, but this sequence is a good default:

1. Start with [Research and startup strategy](docs/research-and-strategy.md) to clarify the niche, demand signals, and early-stage risk.
2. Move to [Brand, positioning, and messaging](docs/brand-positioning-and-messaging.md) so the promise, ICP, and differentiation are explicit.
3. Add [Legal, privacy, and trust](docs/legal-compliance.md) before scaling forms, cookies, email, and public claims.
4. Tighten [Landing pages and on-site conversion](docs/landing-pages.md) and [Product UX, analytics, and support](docs/product-and-ux.md) so traffic has somewhere credible to land.
5. Layer on acquisition, content, and SEO with [Marketing I](docs/marketing-acquisition-and-channels.md), [Marketing II](docs/marketing-pages-and-attribution.md), [Content](docs/content-seo-and-blog.md), [SEO tools](docs/seo-tools-and-faq.md), [Technical SEO](docs/technical-seo-and-site-health.md), and [AI search and GEO](docs/ai-search-and-geo.md).
6. Close the loop with [Measurement, attribution, and experimentation](docs/measurement-attribution-and-experimentation.md), [Paid remarketing](docs/paid-media-remarketing.md), and [Frameworks and retention](docs/frameworks-and-retention.md).

For a simple ordered index, see [docs/index.md](docs/index.md).

---

## Guide map

### Market, positioning, and trust foundation

| Guide                                                                        | Why it matters                                                                                                                 |
| ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| [Research and startup strategy](docs/research-and-strategy.md)               | Turns vague market ideas into a narrower niche, clearer validation loop, and stronger early-stage decision-making baseline.    |
| [Brand, positioning, and messaging](docs/brand-positioning-and-messaging.md) | Defines ICP, value proposition, differentiation, proof, and the message hierarchy that every page and campaign should inherit. |
| [Legal, privacy, and trust](docs/legal-compliance.md)                        | Covers policies, cookies, user rights, NDAs, and trust basics that reduce avoidable risk as traffic and data collection grow.  |

### Site, product, and conversion surface

| Guide                                                         | Why it matters                                                                                                           |
| ------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| [Landing pages and on-site conversion](docs/landing-pages.md) | Helps shape pricing, feature pages, contact paths, social proof, comments, and lead capture so traffic can convert.      |
| [Product UX, analytics, and support](docs/product-and-ux.md)  | Connects onboarding, in-product analytics, support, feedback loops, and UX details to retention and activation outcomes. |

### Acquisition, content, and SEO execution

| Guide                                                                                      | Why it matters                                                                                                                                      |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Marketing I — Acquisition and channels](docs/marketing-acquisition-and-channels.md)       | Covers launch sequencing, manual lead generation, communities, lead magnets, email, directories, social, and paid search basics.                    |
| [Marketing II — Pages, attribution, and programs](docs/marketing-pages-and-attribution.md) | Focuses on audience pages, competitor comparisons, migration pages, referral ideas, influencer workflows, and attribution-aware campaign structure. |
| [Content, blog, and link building](docs/content-seo-and-blog.md)                           | Frames editorial depth, guest posts, author trust, internal linking, and RSS-driven syndication more realistically.                                 |
| [SEO — FAQ, keywords, and tools](docs/seo-tools-and-faq.md)                                | Summarizes keyword intent, long-tail strategy, common tool decisions, and practical FAQ-style SEO heuristics.                                       |
| [Technical SEO and site health](docs/technical-seo-and-site-health.md)                     | Covers crawlability, indexing, canonicals, Core Web Vitals, structured data, internationalization, and site architecture basics.                    |
| [AI search and GEO](docs/ai-search-and-geo.md)                                             | Covers AI Overviews and assistant referrals, generative engine optimization, llms.txt, AI crawler policy, and product-led loops.                     |

### Measurement, paid loops, and retention

| Guide                                                                                                | Why it matters                                                                                                    |
| ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [Measurement, attribution, and experimentation](docs/measurement-attribution-and-experimentation.md) | Sets the analytics, attribution, consent, and experiment discipline needed to make channel decisions responsibly. |
| [Paid media — remarketing](docs/paid-media-remarketing.md)                                           | Explains privacy-aware retargeting foundations, pixel setup, audience segmentation, and frequency control.        |
| [Frameworks and retention](docs/frameworks-and-retention.md)                                         | Gives a compact funnel reference and practical churn-reduction ideas so acquisition connects to long-term value.  |

---

## A practical operating model

This is the sequence I would want a team to internalize:

```txt
Research the niche
  -> define ICP and wedge
  -> write clear positioning and proof
  -> publish trust, policy, and contact basics
  -> improve landing, pricing, and onboarding paths
  -> launch acquisition and content loops
  -> strengthen technical SEO and information architecture
  -> measure activation, conversion, and retention
  -> add remarketing and experiments where traffic volume justifies them
  -> use retention and save flows to protect the value of acquired users
```

That flow matters because most marketing problems are not truly isolated. A weak conversion surface makes SEO look weak. Weak measurement makes paid channels look confusing. Weak retention makes every acquisition channel look more expensive than it really is.

---

## Things I would avoid

- trying to scale channels before the ICP and message are clear;
- publishing thin landing pages and expecting paid traffic to rescue them;
- treating SEO as keywords without information architecture, internal linking, and technical hygiene;
- using attribution reports as if they were ground truth instead of a decision aid;
- creating dozens of low-quality blog posts before a few strong pillar assets exist;
- mixing trust-sensitive behavior with vague legal or privacy posture;
- measuring signups without activation and retention context;
- assuming remarketing can solve a product, onboarding, or positioning problem.

---

## References and inspiration

### Official and high-signal references

- [Google Search Central](https://developers.google.com/search/docs)
- [Google Analytics Help Center](https://support.google.com/analytics)
- [Google Ads Help](https://support.google.com/google-ads)
- [Google Search Quality Evaluator Guidelines](https://developers.google.com/search/blog/2022/12/search-quality-rater-guidelines)
- [Meta Business Help Center](https://www.facebook.com/business/help)
- [HubSpot marketing resources](https://www.hubspot.com/resources)

### Similar or adjacent GitHub repositories

- [awesome-seo](https://github.com/marcelduran/awesome-seo)
- [marketing-examples](https://github.com/hannansarker/marketing-examples)
- [awesome-marketing](https://github.com/marketingtoolslist/awesome-marketing)

---

## License

MIT is a sensible default for a guide repository like this. See [LICENSE](LICENSE).

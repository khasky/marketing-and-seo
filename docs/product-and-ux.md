[← Landing](landing-pages.md) · [Marketing I →](marketing-acquisition-and-channels.md)

# Product UX, analytics, and support

Product-surface notes: registration, analytics, help, safety, and notifications.

## Registration / sign up

- Email verification first — password can come after the email is confirmed.
- Captcha where abuse is a risk.
- Checkbox: I agree to Terms and Privacy (link both).
- After signup, surface mobile app links with clear visuals.

**Security:** default session length of about one week before re-auth is a common starting point — balance UX vs risk; add step-up for sensitive actions.

## App analytics and qualitative tools

- **Amplitude** — product analytics, A/B tests, feature flags, segmentation.
- **LogRocket** — session replay for debugging UX issues.
- **TrackJS** — client-side error tracking.
- **Hotjar** — heatmaps and session recordings to watch real navigation.

Minimum viable analytics: one product analytics tool plus one error or replay tool is a common SaaS pattern. For marketing funnels, UTMs, and attribution hygiene, see [Measurement, attribution and experimentation](measurement-attribution-and-experimentation.md).

## Support chat widget

Intercom, Chatbase, and similar AI/chat products. Criteria:

- Handoff to human when confidence is low.
- SLA visibility in-widget.
- GDPR data processing agreement with vendor.

## Bug report / feedback button

Patterns:

- Shake-to-report on mobile, ? menu on web.
- Capture URL, user id (hashed), console logs (with consent).
- Route to Linear, Jira, or GitHub Issues.

## Panic button

Immediately stop all scheduled operations (posts, sends, campaigns). Essential for social or messaging products where a bug or compromise could spam customers.

**Design**

- Prominent in settings; optional confirm modal.
- Audit log entry.
- Status message until jobs drain.

## User settings

- Delete account and related data (align with [Legal — GDPR](legal-compliance.md)).
- Change email and password with re-authentication.

## Notifications (real time)

### Channels (pick what matches risk)

| Channel | Best for | Notes |
|---------|----------|--------|
| In-app (bell / feed) | Product events, tasks due, teammate actions | Default; respect per-category mutes. |
| Email | Digests, billing, security | Use for non-urgent; avoid duplicating every in-app ping. |
| Web push | Time-sensitive alerts in browser | Needs permission; follow the Web push subsection below. |
| Mobile push (APNs / FCM) | Same as web for native apps | Handle token refresh and revocation. |
| SMS | Security codes, critical outages only | High cost and regulation; avoid marketing spam. |

### Real-time transport (engineering)

- WebSocket or SSE for live feeds when the app is open; fallback to polling if sockets fail through corporate proxies.
- Outbox pattern for reliable delivery — write events to DB, worker pushes to providers.
- Idempotency keys so retries do not double-notify.
- User preferences stored server-side; sync to clients on change.

### Web push best practices (summary)

- Do not trigger the browser permission prompt on first paint — wait until the user sees value (often 30s+ or after a key action).
- Explain what you will send and how often.
- Personalize with care (name, relevant event) and respect quiet hours / timezone.
- Frequency cap — excess notifications drive churn and blocks.

References: [MDN — Push API best practices](https://developer.mozilla.org/en-US/docs/Web/API/Push_API/Best_Practices), vendor guides (OneSignal, Braze, etc.).

## Unauthenticated mode / registration with app in background

### Product patterns

- Let visitors explore a sandbox, sample project, or read-only dashboard.
- Gate mutations with signup; preserve draft state across the boundary where possible (local storage plus server merge).
- Cuts bounce from forced registration walls.

### UX details

- Blur or dim the background UI instead of a blank page — shows what they get after signup.
- Progress: e.g. “Step 1 of 2 — create account” so the modal does not feel endless.
- Social or SSO options where appropriate; still offer email path.
- Mobile: full-screen sheet; avoid tiny tap targets over a busy background preview.

## Navigation

| Prev | Up | Next |
|------|-----|------|
| [Landing](landing-pages.md) | [Home](index.md) | [Marketing I](marketing-acquisition-and-channels.md) |

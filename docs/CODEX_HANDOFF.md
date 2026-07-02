# Pantry Codex Handoff

## Project Summary

Pantry is building the verified healthy commerce layer for grocery behavior.

The consumer-facing product is a healthy grocery rewards platform. Users upload grocery receipts, eventually connect grocery accounts, receive a Pantry Score, earn points, and unlock rewards for healthier grocery behavior.

The long-term business connects consumers, food brands, grocery retailers, employers, insurers, and healthcare partners around verified healthy purchase behavior.

For the full business and product strategy, read:

- `docs/PANTRY_PRODUCT_BIBLE.md`
- `docs/PANTRY_BUSINESS_AND_PRODUCT_STRATEGY.md`

The product combines:

- receipt intelligence
- nutrition scoring
- rewards infrastructure
- secure points ledger
- consumer gamification
- wellness incentives
- verified retail behavior
- future brand-funded rewards

The long-term goal is preventative healthcare and healthy commerce infrastructure through grocery behavior.

---

## Current Priorities

### Immediate Priorities

1. Stable onboarding
2. Authentication reliability
3. Receipt upload flow
4. OCR/extraction through secure server-side processing
5. Product scoring pipeline
6. Points ledger infrastructure
7. Mobile-first polish
8. Rewards marketplace MVP

### Current Strategic Order

```text
Working authentication
→ working receipt extraction
→ Pantry Score
→ points
→ rewards
```

Do not skip ahead to brand campaigns, Hedera, affiliate systems, or healthcare integrations before the consumer loop works.

---

## Strategic Context

Pantry is inspired by Paceline, Receipts, Oasis, and Scout, but should not copy any of them directly.

Pantry should borrow:

- Paceline's reward loop for verified healthy behavior
- Receipts' idea of verified real-world behavior and brand-funded rewards
- Oasis/Scout's trust-first product intelligence and clean scoring presentation

Pantry should avoid:

- NFC hardware
- location-first check-ins
- shame-based nutrition UX
- community before habit
- blockchain as a consumer-facing feature

---

## Design Direction

### Brand Feel

Pantry should feel:

- modern
- premium
- clean
- energetic
- optimistic
- consumer-friendly
- mobile-native
- reward-driven
- not overly clinical

### UX Direction

- Fast onboarding
- Minimal friction
- Highly visual
- Clear point progression
- Native-app feel
- Encouraging score explanations
- Reward progress as the emotional center

### Avoid

- Overly corporate health app feel
- Shame-based nutrition UX
- Cluttered dashboards
- Excessive data density
- Generic SaaS styling
- Random integrations that do not support the MVP loop

---

## Engineering Philosophy

- Treat the browser as untrusted.
- Keep secrets server-side.
- Do not award points from browser-controlled logic.
- Do not make rewards client-authoritative.
- Enforce receipt ownership.
- Keep MVP architecture flexible for future Open Food Facts, USDA, WISEcode, Veryfi, Hedera, and partner campaign integrations.
- Avoid overbuilding future layers before launch-critical functionality works.

---

## Near-Term Build Focus

Engineering should prioritize work that directly supports:

```text
Sign Up
→ Upload Receipt
→ Extract Grocery Items
→ Generate Pantry Score
→ Award Points
→ Show Reward Progress
→ Unlock Rewards
→ Repeat
```

If a task does not improve this loop, it should usually be deferred.

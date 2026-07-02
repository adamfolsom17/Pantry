# Pantry Product Bible

## Vision

Pantry is building the verified healthy commerce layer for grocery behavior.

The consumer-facing wedge is a healthy grocery rewards product inspired by Paceline, but focused on nutrition and grocery behavior instead of exercise.

Users earn rewards for healthier grocery purchases through receipt uploads and eventually linked grocery accounts. Pantry parses purchases, translates grocery behavior into a trusted Pantry Score, awards points, and helps users make healthier choices without shame.

Long term, Pantry aims to become infrastructure for preventative health incentives across consumers, food brands, grocery retailers, employers, insurers, and healthcare systems.

For the deeper business and product strategy, see:

- `docs/PANTRY_BUSINESS_AND_PRODUCT_STRATEGY.md`

---

## Mission

Pantry helps people build healthier lives by turning real grocery purchases into trusted nutrition insights, points, rewards, and long-term behavior change.

---

## Strategic Positioning

### Simple Positioning

Pantry is Paceline for groceries.

### Long-Term Positioning

Pantry is the verified healthy commerce network for grocery behavior.

### Core Insight

Receipts are not the product. Receipts are the input.

The product is verified grocery behavior.

Points are not the product. Points are the motivation layer.

Rewards are not the business. Rewards are the incentive layer.

The business is aligned incentives between consumers, brands, retailers, employers, and healthcare partners.

---

## Core User Flow

1. User signs up via email or Google. Apple Sign-In is deferred until native iOS/App Store needs require it.
2. User uploads grocery receipt OR eventually links grocery loyalty account.
3. Pantry securely parses products and ingredients.
4. Scoring engine assigns Pantry Score and points:
   - Positive points for healthier items
   - Neutral treatment for acceptable items
   - Improvement opportunities for ultra-processed or low-nutrient items
5. User accumulates Pantry Points.
6. User sees progress toward rewards.
7. User redeems points in marketplace.
8. User returns after the next grocery trip.

---

## Product Principles

### 1. Mobile-first

Pantry should feel native, fast, and polished on mobile.

### 2. Gamified behavior change

The product should make healthy grocery shopping feel rewarding instead of restrictive.

### 3. Minimal friction

Receipt upload and onboarding should take under 60 seconds.

### 4. Positive reinforcement

Avoid shame-based UX.

Do not use language like:

- bad food
- failed
- unhealthy cart
- poor choice

Prefer:

- easy improvement opportunity
- strong protein pick
- great produce choice
- simple swap idea
- strong grocery foundation

### 5. Data moat

Over time Pantry should accumulate:

- purchase behavior
- health behavior trends
- nutrition preference data
- brand interaction data
- reward effectiveness data
- verified retail purchase behavior

### 6. Trust before complexity

Pantry should build trust through clear scoring, secure processing, explainable recommendations, and user control.

Blockchain, Hedera, WISEcode, retailer integrations, and brand campaign infrastructure are future layers. They should not distract from the MVP loop.

---

## MVP Features

### Authentication

- Email/password
- Google OAuth
- Session persistence
- Logout reliability

Deferred:

- Phone auth if setup complexity slows launch
- Apple OAuth until native iOS/App Store requirements make it necessary

### Receipt Upload

- Upload receipt image
- OCR/extraction through secure server-side function
- Product parsing
- Item normalization
- Receipt history
- No browser-awarded points

### Pantry Score

- Pantry Score V1
- Explainable scoring
- Positive/neutral/improvement categories
- Confidence states
- Future hooks for Open Food Facts, USDA FoodData Central, WISEcode, and other enrichment layers

### Dashboard

- Total points
- Recent purchases
- Weekly/monthly Pantry Score
- Streaks
- Reward progress
- Next best action

### Rewards Marketplace

- Locked/unlocked rewards
- Progress toward reward
- Manual or Pantry-funded test rewards
- Future partner rewards
- Future brand-funded campaigns

### Admin Panel

Initial Pantry admin needs:

- user management
- receipt monitoring
- extraction failure review
- scoring review
- points ledger review
- reward inventory management
- launch metrics

Future admin needs:

- brand campaign management
- partner analytics
- retailer/employer/healthcare reporting

---

## Business Model Direction

Revenue should be layered in this order:

1. Pantry-funded test rewards to prove behavior.
2. Brand-funded bonus points for verified retail purchases.
3. Sponsored challenges.
4. Affiliate marketplace add-ons.
5. Pantry Plus / freemium.
6. Employer, insurance, and food-as-medicine partnerships.
7. Verified incentive infrastructure.

Do not overbuild monetization before the consumer loop works.

---

## Design Direction

Pantry should feel like:

```text
Paceline
+
Receipts
+
Oasis
+
Scout
```

Borrow from Paceline:

- progress toward rewards
- healthy behavior loop
- premium wellness feel
- simple points system

Borrow from Receipts:

- verified behavior
- brand-funded rewards logic
- real-world commerce attribution

Borrow from Oasis and Scout:

- trust
- clean scoring
- product clarity
- confidence in analysis

Pantry-specific feel:

- mobile-first
- colorful but not childish
- premium
- fast
- reward-driven
- animated
- clear
- warm

---

## Current Execution Priority

The next build milestone remains:

```text
Working authentication
→ working receipt extraction
→ Pantry Score
→ points
→ rewards
```

The long-term strategy should inform architecture, but it should not create scope creep.

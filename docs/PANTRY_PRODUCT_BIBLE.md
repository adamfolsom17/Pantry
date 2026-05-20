# Pantry Product Bible

## Vision
Pantry is a healthy grocery rewards platform inspired by products like Paceline, but focused on nutrition and grocery behavior instead of exercise.

Users earn rewards for healthier grocery purchases through receipt uploads and eventually linked grocery accounts. The platform assigns points based on food quality and nutritional value, rewarding healthier choices while discouraging poor nutritional purchases.

Long term, Pantry aims to become infrastructure for preventative health incentives across consumers, brands, employers, insurers, and healthcare systems.

---

## Core User Flow

1. User signs up via email, Google, or Apple.
2. User uploads grocery receipt OR links grocery loyalty account.
3. Pantry parses products and ingredients.
4. Scoring engine assigns points:
   - Positive points for healthy items
   - Neutral for acceptable items
   - Negative for ultra-processed / unhealthy items
5. User accumulates Pantry Points.
6. User redeems points in marketplace:
   - Supplements
   - Healthy grocery cashback
   - Apparel
   - Fitness discounts
   - Wellness products

---

## Product Principles

### 1. Mobile-first
Pantry should feel native and fast on mobile.

### 2. Gamified behavior change
The product should make healthy grocery shopping feel rewarding instead of restrictive.

### 3. Minimal friction
Receipt upload and onboarding should take under 60 seconds.

### 4. Positive reinforcement
Avoid shame-based UX.

### 5. Data moat
Over time Pantry should accumulate:
- Purchase behavior
- Health behavior trends
- Nutrition preference data
- Brand interaction data

---

## MVP Features

### Authentication
- Email/password
- Google OAuth
- Apple OAuth

### Receipt Upload
- Upload image
- OCR extraction
- Product parsing
- Points scoring

### Dashboard
- Total points
- Recent purchases
- Weekly nutrition score
- Streaks
- Reward progress

### Rewards Marketplace
- Redeem rewards
- Affiliate integrations
- Brand partnerships

### Admin Panel
- User management
- Receipt moderation
- Reward management
- Point adjustment controls
- Analytics

---

## Future Features

### Grocery Account Linking
Potential integrations:
- Walmart
- Target
- Whole Foods
- Kroger
- Hy-Vee
- Costco

### AI Nutrition Coach
- Personalized recommendations
- Meal optimization
- Budget-conscious healthy alternatives

### Health Layer
- Integrate wearables
- Insurance incentives
- Employer wellness programs
- HSA/FSA integrations

### Social Layer
- Challenges
- Friend leaderboards
- Community streaks

---

## Technical Stack

### Frontend
- Next.js
- React
- Tailwind
- Vercel

### Backend
- Supabase
- PostgreSQL
- Edge Functions

### OCR / AI
- OpenAI APIs
- Vision models
- Nutrition classification layer

### Auth
- Supabase Auth

### Storage
- Supabase Storage

---

## Core Scoring Philosophy

Pantry should avoid simplistic calorie-based scoring.

Scoring should consider:
- Ingredient quality
- Processing level
- Added sugar
- Protein quality
- Fiber
- Artificial ingredients
- Macronutrient balance
- Portion context

Potential future datasets:
- USDA Healthy Eating Index
- WISEcode
- OpenFoodFacts
- Branded nutrition APIs

---

## Business Model

### B2C
- Brand marketplace commissions
- Affiliate revenue
- Premium subscriptions
- Sponsored health challenges

### B2B
- Employer wellness
- Insurance partnerships
- Health system integrations
- Retail partnerships
- Consumer insights

---

## Competitive Positioning

### Comparable Products
- Paceline
- Fetch Rewards
- Yuka
- MyFitnessPal
- Instacart Health

### Pantry Differentiation
- Grocery-first rewards
- Behavior change incentives
- Gamified nutrition
- Long-term health infrastructure
- Midwest / consumer accessibility focus

---

## Current Build Notes

Current stack and experiments include:
- Bolt.new
- Supabase
- Vercel
- Figma
- Lovable
- Base44
- Vibecode

Current priorities:
1. Stable onboarding
2. Reliable receipt parsing
3. Clean mobile UI
4. Functional rewards engine
5. Fast iteration loop

---

## Long-Term Vision

Pantry becomes the rewards and incentives layer for preventative health.

Instead of rewarding spending generally, Pantry rewards healthier behavior.

The platform ultimately sits between:
- Consumers
- Grocery retailers
- Health brands
- Employers
- Insurance companies
- Healthcare systems

with the goal of improving long-term health outcomes through aligned incentives.

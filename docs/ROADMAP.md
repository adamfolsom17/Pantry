# Pantry Roadmap

## Roadmap Philosophy

Pantry should be built as a mobile-first web app MVP before becoming a native mobile app. The goal is to validate the core behavioral loop before overbuilding infrastructure.

Core question:

Will this make users want to scan another receipt tomorrow?

If the answer is no, the feature is probably not an MVP priority.

---

## Phase 1: Functional MVP

### Goal
Create a working mobile-first web app where users can upload a receipt, receive a Pantry score, earn points, create an account, and view rewards.

### Priority Features
- Landing page
- Scan/upload receipt CTA
- Receipt image upload
- Mock or early OCR receipt parsing
- Item-level scoring output
- Pantry Score summary
- Points preview
- Post-analysis account creation
- User dashboard
- Rewards marketplace preview

### Product Rule
Do not force signup before receipt upload. Let users experience the value first, then prompt them to create an account to save points.

---

## Phase 2: Real Data and Persistence

### Goal
Move from demo functionality to real user state and persistent records.

### Priority Features
- Supabase auth fully connected
- User profiles
- Receipt records
- Parsed receipt items
- Score history
- Points ledger
- Reward redemption records
- Basic admin review tools

---

## Phase 3: Scoring Engine Improvement

### Goal
Replace simplistic mock scoring with a more reliable nutrition-quality framework.

### Priority Features
- Item normalization
- Category classification
- Positive, neutral, and negative scoring rules
- Basic nutrition metadata
- Ingredient-quality weighting
- Ultra-processed item detection
- Suggested healthier swaps

---

## Phase 4: Rewards Marketplace MVP

### Goal
Make points feel valuable and create early reward motivation.

### Priority Features
- Reward catalog
- Locked/unlocked reward states
- Redemption flow
- Partner reward placeholders
- Affiliate link support
- Admin reward creation/editing

---

## Phase 5: Integrations

### Goal
Reduce receipt friction and expand data quality.

### Potential Integrations
- Grocery loyalty accounts
- Grocery APIs
- OpenFoodFacts
- USDA data
- WISEcode or similar nutrition data provider
- OCR provider or OpenAI vision flow

---

## Phase 6: Native Mobile App

### Goal
Only pursue native mobile once web behavior validates repeat usage.

### Trigger Conditions
Consider native app when:
- Users scan receipts repeatedly
- Rewards create meaningful retention
- Mobile web friction becomes a growth blocker
- Push notifications, camera flows, and wallet-like reward UX become necessary

---

## Not Now

Avoid building these too early:
- Native mobile app
- Full social network
- Insurance portal
- Employer dashboard
- Advanced AI coach
- Complex grocery integrations
- Overly detailed nutrition science
- Blockchain or token mechanics

---

## Current North Star

Build the simplest rewarding product loop:

Landing page -> receipt upload -> analysis -> points preview -> signup -> dashboard -> rewards.

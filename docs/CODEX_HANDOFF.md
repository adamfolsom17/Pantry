# Pantry Codex Handoff

## Project Summary

Pantry is a healthy grocery rewards platform.

Users upload grocery receipts or connect grocery accounts to earn rewards for healthier food purchases.

The product combines:
- nutrition scoring
- rewards infrastructure
- receipt OCR
- consumer gamification
- wellness incentives

The long-term goal is preventative healthcare infrastructure through grocery behavior.

---

## Current Priorities

### Immediate Priorities
1. Stable onboarding
2. Authentication reliability
3. Receipt upload flow
4. OCR extraction
5. Product scoring pipeline
6. Mobile-first polish
7. Rewards marketplace MVP

---

## Design Direction

### Brand Feel
Pantry should feel:
- modern
- clean
- energetic
- optimistic
- consumer-friendly
- not overly clinical

### UX Direction
- Fast onboarding
- Minimal friction
- Highly visual
- Clear point progression
- Native-app feel

### Avoid
- Overly corporate health app feel
- Shame-based nutrition UX
- Cluttered dashboards
- Excessive data density

---

## Engineering Philosophy

### Prioritize
- speed
- iteration
- reliability
- modularity
- mobile responsiveness

### Avoid
- premature optimization
- overengineering
- unnecessary abstractions

---

## Suggested Architecture

### Frontend
- Next.js
- React
- Tailwind
- Vercel deployment

### Backend
- Supabase
- PostgreSQL
- Edge Functions

### AI Layer
- OCR extraction
- receipt parsing
- nutrition scoring
- product classification

---

## Important Product Constraints

### Receipt Uploads
Receipt upload should:
- support imperfect photos
- handle grocery abbreviations
- work across multiple retailers
- provide fallback editing

### Nutrition Scoring
Avoid simplistic calorie logic.

Scoring should prioritize:
- ingredient quality
- ultra-processing
- added sugar
- protein quality
- fiber
- nutrient density

---

## Marketplace Direction

Potential rewards:
- supplements
- protein products
- healthy snacks
- grocery discounts
- apparel
- fitness discounts
- wellness products

---

## Long-Term Expansion

Future opportunities:
- insurance partnerships
- employer wellness
- grocery integrations
- healthcare incentives
- AI nutrition assistant
- personalized recommendations
- preventative health analytics

---

## Development Notes

When making product decisions:
- prioritize consumer simplicity
- optimize for retention loops
- maintain mobile-first UX
- preserve clean design consistency
- reduce onboarding friction aggressively

---

## Codex Instructions

When generating code:
- keep components modular
- use consistent Tailwind spacing
- prioritize responsive design
- avoid unnecessary dependencies
- document major architectural decisions
- optimize for iteration speed

When generating UI:
- emphasize clean cards
- soft shadows
- modern typography
- strong spacing hierarchy
- intuitive reward visualization

---

## Repository Expectations

Suggested structure:

/apps
/components
/lib
/hooks
/services
/docs

Keep docs updated whenever major architectural or product decisions change.

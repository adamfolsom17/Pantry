# Pantry Scoring Engine

## Scoring Philosophy

Pantry is not a calorie-counting app.

The goal is to encourage healthier grocery purchasing behavior through directional improvement and behavioral reinforcement.

The scoring engine should:
- reward healthier choices
- avoid shame-based experiences
- encourage progress over perfection
- remain understandable to normal consumers

---

## High-Level Scoring Categories

### Positive Score Items
Examples:
- Whole foods
- Fruits
- Vegetables
- Lean proteins
- Greek yogurt
- High-fiber foods
- Low-added-sugar foods
- Nutrient-dense products

### Neutral Score Items
Examples:
- Moderately processed foods
- Reasonable convenience foods
- Balanced packaged items

### Negative Score Items
Examples:
- Highly ultra-processed products
- Excessive added sugar
- Artificial additive-heavy products
- Extremely low nutrient density items

Important:
Negative scoring should not feel punitive.

---

## Initial MVP Logic

Early MVP scoring can use:
- category-based scoring
- keyword detection
- nutrition heuristics
- manually weighted rules

Perfect nutrition science is NOT required for MVP.

The goal is behavioral motivation and repeat usage.

---

## Potential Scoring Inputs

### Nutrition Inputs
- Calories
- Protein
- Fiber
- Added sugar
- Sodium
- Ingredient count
- Artificial ingredients
- Processing level

### Product Classification Inputs
- Whole food
- Packaged food
- Beverage
- Snack
- Frozen
- Organic
- Protein-focused

---

## Long-Term Data Sources

Potential future integrations:
- OpenFoodFacts
- USDA data
- WISEcode
- Branded nutrition APIs
- Retailer metadata

---

## User Experience Rules

The scoring experience should:
- feel rewarding
- feel understandable
- avoid overwhelming users
- emphasize wins
- suggest improvement opportunities positively

Avoid:
- overly technical nutrition grading
- aggressive red warning systems
- guilt-oriented messaging
- excessive detail density

---

## Example Output

Pantry Score: 82

Strong choices:
- Greek yogurt
- Fresh berries
- Chicken breast
- High-fiber wraps

Areas to improve:
- Sugary cereal
- Soda

Suggested swaps:
- Lower sugar cereal
- Sparkling water alternative

---

## Important Constraint

The scoring engine should remain:
- explainable
- lightweight
- emotionally positive
- fast

Do not build an overcomplicated scientific grading engine for MVP.

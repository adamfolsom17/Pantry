# Pantry Resource and Partnership Map

## Purpose

This document tracks potential data providers, competitors, UX references, tooling integrations, and future business partners for Pantry.

Important distinction:
- A resource on this list is not automatically an integration priority.
- Pantry-Codex should not wire tools into the product unless explicitly instructed.
- This document is for strategic evaluation, not automatic implementation.

## Usage Labels

- Use Now: potentially useful for MVP or immediate product build.
- Evaluate Soon: worth testing during MVP or early V1.
- Partnership Later: strategically interesting but not required for MVP.
- Watchlist Only: useful reference, but should not be integrated unless future needs change.
- Competitor Reference: study UX, positioning, or business model, but do not copy.

---

# 1. Scoring, Nutrition Intelligence, and Food Data

## WISEcode

Status: Evaluate Soon / Potential Strategic Partner

Website: https://wisecode.ai/

What it is:
WISEcode is a packaged-food intelligence platform focused on ingredient-level analysis, ultra-processed food classification, and food transparency. It positions itself as going beyond the standard Nutrition Facts Panel by analyzing foods with ingredient-level precision.

What it does:
- Classifies ultra-processed foods
- Analyzes packaged foods at the ingredient level
- Provides a consumer UPF detector app
- Offers Non-UPF verification for brands
- Creates a more detailed food intelligence layer than basic nutrition labels

How Pantry could use it:
- Future scoring backbone for ultra-processed food detection
- Ingredient-level signal layer for Pantry Score
- Partner data provider for packaged food analysis
- Potential business development partner if Pantry becomes a reward/incentive layer over better food choices

MVP recommendation:
Do not deeply integrate immediately unless an API or partnership path is clearly available and affordable. Use Pantry's own simple heuristic scoring first, then evaluate WISEcode as a premium scoring/data layer.

Why it matters:
WISEcode aligns closely with Pantry's long-term ambition to reward healthier grocery behavior using deeper food intelligence than calories or macros.

---

## USDA Healthy Eating Index

Status: Use Now as Framework / Not Direct Product Integration Yet

Website: https://www.fns.usda.gov/cnpp/healthy-eating-index

What it is:
The Healthy Eating Index is a USDA-backed framework for assessing diet quality based on alignment with the Dietary Guidelines for Americans.

What it does:
- Provides a diet-quality measurement framework
- Evaluates food-pattern quality rather than single-item morality
- Can help Pantry avoid building a purely arbitrary scoring system

How Pantry could use it:
- Strategic scoring reference
- Framework for nutrition philosophy
- Long-term benchmark for cart-level nutrition quality
- Useful credibility layer for investor/product conversations

MVP recommendation:
Use as a conceptual framework only. Do not try to fully implement HEI scoring in MVP because it may require more complete dietary-intake context than receipt-level scoring provides.

Why it matters:
It helps Pantry avoid a weak or overly subjective scoring system.

---

## USDA FoodData Central

Status: Use Now / Evaluate Soon

Website: https://fdc.nal.usda.gov/

What it is:
FoodData Central is the USDA's food and nutrient data system, including foundational foods, branded foods, legacy data, and nutrition profile data.

What it does:
- Provides nutrient data for foods
- Includes multiple data types, including branded foods and survey-based food databases
- Offers a public reference point for macro/micronutrient data

How Pantry could use it:
- Nutrition lookup layer
- Backstop for food classification
- Data reference for generic food items
- Possible enrichment layer after OCR parses receipt items

MVP recommendation:
Evaluate early. It is likely one of the safest public data sources for nutrition metadata, though product matching from messy receipt names may still be hard.

Why it matters:
It is credible, public, and foundational for nutrition data.

---

## Open Food Facts

Status: Use Now / Evaluate Soon

Website: https://world.openfoodfacts.org/

What it is:
Open Food Facts is a free, crowdsourced global food product database containing product names, brands, ingredients, allergens, additives, nutrition facts, and product images.

What it does:
- Stores packaged-food data
- Supports barcode/product lookup
- Includes ingredients and nutrition data
- Provides a foundation for consumer-facing food transparency tools

How Pantry could use it:
- Early product enrichment layer
- Barcode or product matching if Pantry later supports scanning packaging
- Ingredient lookup
- Additive and nutrition metadata

MVP recommendation:
Strong candidate for early experimentation, especially if receipt OCR can map items to product names or UPCs. Do not depend on it as the only scoring source because coverage and data quality can vary.

Why it matters:
It can accelerate Pantry's data layer before expensive enterprise partnerships.

---

## FatSecret Platform API

Status: Evaluate Soon

Website: https://platform.fatsecret.com/

What it is:
FatSecret is a nutrition app and food data platform with a global food and nutrition API.

What it does:
- Provides food and nutrition database access
- Supports food search and nutrition lookups
- Powers other health and nutrition apps

How Pantry could use it:
- Food/nutrition lookup API
- Product normalization support
- Fallback for generic food matching

MVP recommendation:
Evaluate pricing, API terms, and matching quality before using. It may be useful if USDA/Open Food Facts matching is insufficient.

Why it matters:
A mature nutrition API could reduce internal data burden.

---

## Spoonacular

Status: Watchlist / Possible V1-V2 Add-On

Website: https://spoonacular.com/food-api

What it is:
Spoonacular is a food and recipe API with ingredient, recipe, nutrition, product, menu item, meal planning, and shoppable recipe functionality.

What it does:
- Recipe analysis
- Ingredient mapping
- Nutrition analysis
- Product search
- Menu item data
- Meal planning
- UPC lookup

How Pantry could use it:
- Future meal planning
- Healthy swap recommendations
- Recipe recommendations based on groceries purchased
- Product and ingredient enrichment

MVP recommendation:
Do not prioritize for receipt scoring MVP. It becomes more useful if Pantry adds meal planning, recipes, or grocery-to-meal recommendations.

Why it matters:
Good potential future bridge from grocery rewards into personalized healthy meal guidance.

---

## Nutritionix

Status: Watchlist / Alternative Data Provider

Website: https://developer.nutritionix.com/

What it is:
Nutritionix is a nutrition data and API provider used for food search, nutrition lookup, and food logging use cases.

What it does:
- Food database lookup
- Nutrition information retrieval
- Common food and branded food data support

How Pantry could use it:
- Alternative food/nutrition lookup provider
- Possible fallback if USDA/Open Food Facts/FatSecret are not enough

MVP recommendation:
Do not prioritize until the team tests cheaper/public options and understands data matching needs.

Why it matters:
Could be useful later, but likely overlaps with FatSecret, USDA FoodData Central, and Open Food Facts.

---

# 2. Consumer Product Scoring and UX References

## Scout

Status: Competitor Reference / Potential Partner Later

Website: https://scouthealthapp.com/

What it is:
Scout is a consumer health analysis app that helps users check what is inside products and find healthier alternatives. It analyzes products through ingredients, packaging, processing, lab testing results, and research.

What it does:
- Scores products from 1-100
- Flags ingredients, processing, packaging, contaminants, and lab-test signals
- Provides healthier alternatives
- Claims no sponsored rankings or paid placements

How Pantry could use it:
- UX reference for product analysis cards
- Scoring methodology inspiration
- Potential future partnership or benchmark for product safety/transparency

MVP recommendation:
Do not integrate. Study the UX and scoring communication style. Pantry's differentiator should remain grocery behavior rewards, not pure product scanning.

Why it matters:
Scout is highly relevant to how Pantry could present product-level health signals in a clear, consumer-friendly way.

---

## Oasis Health App

Status: UX Reference / Watchlist Partnership Later

Website: https://www.oasishealth.app/

What it is:
Oasis is a consumer app focused on helping users see what is inside products, water, and everyday items using verified lab data, product safety scoring, and in-store scanning.

What it does:
- Product scanning
- Ingredient and safety breakdowns
- Lab-test-backed insights
- Product rankings
- Water and product safety analysis

How Pantry could use it:
- UX inspiration for scanning, score reveals, and product breakdowns
- Reference for trust-building around lab data and safety claims
- Possible future inspiration if Pantry expands beyond grocery nutrition into safety/contaminant signals

MVP recommendation:
Do not integrate. Study the UI, motion, information hierarchy, and score presentation.

Why it matters:
Oasis is a strong design and trust reference for modern consumer health analysis.

---

## Yuka

Status: Competitor Reference / Watchlist

Website: https://yuka.io/

What it is:
Yuka is a consumer app that lets users scan food and cosmetic products to receive health scores, ingredient breakdowns, and healthier alternatives.

What it does:
- Barcode product scanning
- Color-coded health scoring
- Ingredient/additive analysis
- Healthier alternative suggestions
- Consumer-facing food transparency

How Pantry could use it:
- UX reference for simple scoring
- Benchmark for consumer trust and behavior change
- Inspiration for alternatives and product recommendations

MVP recommendation:
Do not copy or integrate. Study carefully, but avoid overly fear-based or oversimplified scoring. Pantry should be more rewards-driven and behavior-positive.

Why it matters:
Yuka shows that consumers care deeply about simple product health scores and that scoring apps can influence buying behavior.

---

## Bobby Approved / FlavCity

Status: Competitor Reference / Partnership Watchlist

Website: https://www.bobbyapproved.com/ or FlavCity ecosystem

What it is:
Bobby Approved is a barcode/product scanner connected to Bobby Parrish's FlavCity media and CPG ecosystem. It flags ingredients and recommends healthier alternatives.

What it does:
- Product scanning
- Ingredient approval/disapproval
- Healthy alternative recommendations
- Creator-led consumer health trust

How Pantry could use it:
- Study creator-led trust and commerce
- Study how product scans can produce valuable product-market data
- Potential future rewards/brand marketplace reference

MVP recommendation:
Do not integrate. Use as a business model and GTM reference.

Why it matters:
It shows how product scanning, consumer trust, and owned CPG products can reinforce each other.

---

## CodeCheck

Status: Watchlist / Competitor Reference

Website: https://www.codecheck.info/

What it is:
CodeCheck is a product scanning app focused on ingredient and nutrition information for food and cosmetics.

What it does:
- Barcode scanning
- Ingredient information
- Nutrition and product signals
- Consumer transparency

How Pantry could use it:
- Reference for product-scanning UX
- Alternative benchmark to Yuka/Scout/Oasis

MVP recommendation:
Do not integrate. Watch for UX and product transparency patterns.

Why it matters:
It is another example of consumer demand for simple ingredient interpretation.

---

# 3. Rewards, Incentives, and Behavior Change References

## Paceline

Status: Core UX / Business Model Reference

Website: https://www.paceline.fit/

What it is:
Paceline rewards users for healthy behaviors, historically focused around physical activity and wellness incentives.

What it does:
- Tracks healthy activity
- Rewards users for behavior
- Connects health behavior to incentives
- Creates a wellness rewards loop

How Pantry could use it:
- Core behavior-change inspiration
- Reference for rewards psychology
- Reference for brand partnerships and consumer wellness incentives

MVP recommendation:
Do not integrate. Study the reward loop and product feel.

Why it matters:
Pantry's grocery behavior loop is highly analogous to Paceline's healthy activity loop.

---

## Plyo

Status: Core UX / Business Model Reference

Website: https://www.plyo.app/

What it is:
Plyo is a rewards platform tied to health/wellness activity and gym/fitness behavior.

What it does:
- Incentivizes healthy behavior
- Rewards engagement with fitness/wellness actions
- Connects consumers with offers and brand incentives

How Pantry could use it:
- Rewards marketplace inspiration
- Partner marketplace inspiration
- UX reference for lightweight gamification

MVP recommendation:
Do not integrate. Use as product and business model reference.

Why it matters:
The rewards behavior loop is directly relevant to Pantry's long-term business model.

---

## Nucona

Status: Competitor/Comparable Reference / Watchlist Partnership

Website: https://www.nucona.org/

What it is:
Nucona is a nutrition incentive organization focused on personalized nutrition recommendations, retail integrations, and cash-back or points-based incentives tied to healthier shopping behavior.

What it does:
- Tracks food consumption
- Uses Healthy Eating Index-oriented scoring
- Rewards healthy shopping behavior with points
- Mentions integrations with retailers

How Pantry could use it:
- Direct comparable for grocery-based incentives
- Study scoring and rewards framing
- Potential future partnership or competitive intelligence reference

MVP recommendation:
Do not integrate now. Study closely because the overlap with Pantry is significant.

Why it matters:
Nucona appears conceptually close to Pantry's thesis: healthy grocery purchasing rewarded with incentives.

---

# 4. Food-as-Medicine, Healthcare, Employer, and Insurance Partnerships

## Instacart Health

Status: Partnership Later / Strategic Reference

Website: https://www.instacart.com/company/health/

What it is:
Instacart Health is Instacart's health-focused initiative around nutrition security, food-as-medicine, healthy grocery access, and healthcare-aligned food programs.

What it does:
- Enables health plans, providers, nonprofits, and employers to support grocery access
- Supports nutrition programs and food-as-medicine initiatives
- Creates infrastructure around grocery delivery and health benefits

How Pantry could use it:
- Long-term strategic partner
- Grocery fulfillment layer
- Food-as-medicine validation point
- Potential employer/insurance integration reference

MVP recommendation:
Do not integrate now. Treat as a long-term partnership/market validation reference.

Why it matters:
Instacart Health validates Pantry's bigger thesis that grocery behavior can be connected to healthcare incentives.

---

## Foodsmart

Status: Partnership Later / Strategic Reference

Website: https://www.foodsmart.com/

What it is:
Foodsmart is a foodcare and telenutrition platform that connects nutrition guidance, food ordering, benefits, and healthcare-aligned support.

What it does:
- Telenutrition
- Food benefits support
- Meal planning
- Grocery ordering support
- Health plan/employer nutrition programs

How Pantry could use it:
- Strategic reference for healthcare and payer channels
- Potential future partner if Pantry focuses on rewards and engagement while Foodsmart focuses on clinical nutrition services

MVP recommendation:
Do not integrate. Study as an enterprise/healthcare go-to-market model.

Why it matters:
It shows how nutrition can move from consumer wellness into payer/employer infrastructure.

---

## Season Health

Status: Partnership Later / Strategic Reference

Website: https://www.seasonhealth.com/

What it is:
Season Health is a food-as-medicine platform connecting personalized nutrition, healthcare needs, and food access.

What it does:
- Personalized nutrition support
- Food benefits/navigation
- Healthcare-oriented nutrition programs
- Food-as-medicine infrastructure

How Pantry could use it:
- Long-term model for healthcare integration
- Possible future partnership if Pantry builds strong consumer engagement and receipt-based behavior data

MVP recommendation:
Do not integrate. Watch as strategic reference.

Why it matters:
Season represents the clinical/healthcare version of the broader nutrition-incentives market Pantry may eventually touch.

---

## FarmboxRx

Status: Partnership Later / Strategic Reference

Website: https://www.farmboxrx.com/

What it is:
FarmboxRx is a food-as-medicine company focused on delivering healthy foods and produce through healthcare and benefits channels.

What it does:
- Food delivery for health plans and healthcare programs
- Produce and healthy food boxes
- Nutrition access programs

How Pantry could use it:
- Strategic healthcare channel reference
- Potential future rewards partner for healthy food boxes
- Employer/insurance partnership inspiration

MVP recommendation:
Do not integrate. Watch for future food-as-medicine partnerships.

Why it matters:
It represents the supply/reward side of nutrition incentive programs.

---

## Uber Health

Status: Watchlist / Infrastructure Reference

Website: https://www.uberhealth.com/

What it is:
Uber Health provides healthcare logistics services such as transportation, prescription delivery, and grocery delivery support through healthcare partners.

What it does:
- Patient transportation
- Prescription delivery
- Grocery delivery support
- Healthcare partner logistics

How Pantry could use it:
- Long-term reference for healthcare-aligned grocery delivery infrastructure
- Possible future partner only if Pantry moves into care-plan fulfillment or benefits navigation

MVP recommendation:
Do not integrate.

Why it matters:
It shows that healthcare companies increasingly view grocery delivery as part of care infrastructure.

---

# 5. Restaurant and Out-of-Home Nutrition

## MenuFit

Status: Watchlist / Future Expansion

Website: https://menufitapp.com/

What it is:
MenuFit is a consumer app for healthier restaurant ordering. It personalizes restaurant menu recommendations based on user goals, cravings, calories, macros, and body metrics.

What it does:
- Personalized restaurant meal recommendations
- Restaurant search
- Macro/calorie-aligned menu suggestions
- Goal-based food guidance

How Pantry could use it:
- Future expansion reference if Pantry moves beyond groceries into all food purchasing
- UX reference for personalization
- Potential future partnership for restaurant rewards

MVP recommendation:
Do not integrate. Pantry should stay grocery-first for MVP.

Why it matters:
It points toward a broader future where Pantry could become a rewards layer for all food decisions, not just groceries.

---

# 6. Receipt OCR, Document Parsing, and Product Extraction

## Veryfi

Status: Evaluate Soon

Website: https://www.veryfi.com/

What it is:
Veryfi provides document extraction APIs, SDKs, and AI tools for receipts, invoices, checks, IDs, product nutrition facts, and other document workflows.

What it does:
- Receipt OCR
- Browser and mobile document capture SDKs
- Data extraction APIs
- Fraud detection
- Product intelligence
- Nutrition facts extraction

How Pantry could use it:
- Receipt parsing provider
- Browser-based scanner/capture SDK
- Line-item extraction from grocery receipts
- Potential fraud detection later if rewards become financially meaningful

MVP recommendation:
Strong candidate to evaluate if OpenAI Vision or simple OCR is unreliable. Do not adopt until tested against actual grocery receipts.

Why it matters:
Receipt parsing quality is one of the biggest MVP risk areas.

---

## OpenAI Vision / Multimodal Models

Status: Use Now / Evaluate Soon

Website: https://openai.com/

What it is:
OpenAI multimodal models can read and reason over receipt images, extract structured information, classify items, and power Pantry's AI analysis.

What it does:
- Image understanding
- OCR-like extraction
- Item classification
- Structured JSON extraction
- Scoring assistance

How Pantry could use it:
- MVP receipt parsing
- Item categorization
- Scoring explanation generation
- Suggested healthy swaps

MVP recommendation:
Likely the best MVP starting point because it is flexible and fast to prototype. Later compare accuracy/cost against Veryfi and dedicated OCR providers.

Why it matters:
It can let Pantry move quickly before specialized receipt infrastructure is required.

---

## Google Cloud Vision / Document AI

Status: Watchlist / Alternative OCR Provider

Website: https://cloud.google.com/vision and https://cloud.google.com/document-ai

What it is:
Google provides OCR and document AI services for extracting text and structure from images and documents.

What it does:
- OCR
- Document parsing
- Text extraction
- Entity extraction depending on configuration

How Pantry could use it:
- Alternative receipt parsing provider
- Enterprise-grade OCR fallback

MVP recommendation:
Do not use first unless OpenAI/Veryfi are inadequate. Could add complexity.

Why it matters:
Useful benchmark for OCR reliability and cost.

---

# 7. Grocery/Retailer Integrations

## Kroger Developer API

Status: Partnership Later / Evaluate Later

Website: https://developer.kroger.com/

What it is:
Kroger's developer platform provides access to Kroger-related product/location/cart capabilities depending on API access and permissions.

What it does:
- Product search capabilities
- Store/location data
- Potential shopping/cart-related functionality

How Pantry could use it:
- Future linked grocery account experience
- Product metadata enrichment
- Retailer-specific offers and rewards

MVP recommendation:
Do not prioritize before the receipt-upload loop works. Retailer integrations can become complicated and should follow demonstrated user demand.

Why it matters:
Kroger/retailer integrations are part of Pantry's long-term vision but not required for MVP validation.

---

## Instacart Developer / Instacart Health

Status: Partnership Later

Website: https://www.instacart.com/company/health/

What it is:
Instacart's health and commerce infrastructure could eventually support grocery rewards, healthy cart recommendations, and food-as-medicine programs.

How Pantry could use it:
- Healthy grocery fulfillment
- Reward redemption through grocery credit
- Food-as-medicine pilots
- Employer/health plan partnerships

MVP recommendation:
Do not integrate now. Track strategically.

---

# 8. Additional Similar Tools to Monitor

## Edamam

Status: Watchlist / Possible Food Analysis API

What it is:
Edamam provides nutrition analysis, recipe search, meal planning, and food database APIs.

How Pantry could use it:
- Recipe/meal planning later
- Nutrition analysis support
- Healthy swap recommendations

MVP recommendation:
Do not prioritize unless Pantry expands beyond receipt-based grocery scoring.

---

## MyFitnessPal

Status: Competitor Reference / Watchlist

What it is:
A major consumer nutrition and calorie tracking app.

How Pantry could use it:
- Study retention mechanics
- Study nutrition logging friction
- Learn what Pantry should avoid: excessive manual entry and calorie obsession

MVP recommendation:
Do not integrate.

---

## Noom

Status: Competitor Reference / Behavioral Science Reference

What it is:
A behavior-change and weight-management platform.

How Pantry could use it:
- Study habit formation and coaching psychology
- Reference positive behavior nudges

MVP recommendation:
Do not integrate.

---

## Wholesome Wave

Status: Partnership Later / Public Health Reference

What it is:
A nonprofit focused on nutrition incentives, produce prescriptions, and food access.

How Pantry could use it:
- Long-term nonprofit/public health partnership inspiration
- Food incentive program reference

MVP recommendation:
Do not integrate.

---

## Partnership for a Healthier America

Status: Partnership Later / Public Health Reference

What it is:
A nonprofit working with the private sector to improve health and nutrition access.

How Pantry could use it:
- Long-term public health partnership reference
- Potential credibility partner if Pantry enters health equity and food access programs

MVP recommendation:
Do not integrate.

---

# 9. Recommended MVP Integration Stack

Do not overbuild. For MVP, Pantry should only consider the minimum stack needed to prove the loop.

## Recommended MVP Stack

1. OpenAI Vision or lightweight OCR for receipt parsing
2. Pantry-owned heuristic scoring engine
3. USDA FoodData Central and/or Open Food Facts for nutrition/product enrichment
4. Supabase for user data, receipt records, score history, and points ledger
5. Manual/admin-controlled rewards catalog

## Evaluate After MVP

- WISEcode for UPF/ingredient-level scoring
- Veryfi for better receipt OCR
- FatSecret or Nutritionix for nutrition lookup quality
- Spoonacular or Edamam for meal planning and swaps

## Do Not Build Yet

- Native mobile app
- Deep grocery account integrations
- Healthcare partner workflows
- Insurance/employer dashboards
- Full clinical nutrition guidance
- Restaurant scoring

---

# 10. Current Priority Ranking

## Highest Priority to Evaluate
1. OpenAI Vision
2. USDA FoodData Central
3. Open Food Facts
4. WISEcode
5. Veryfi

## Strong Strategic References
1. Paceline
2. Plyo
3. Scout
4. Oasis
5. Yuka
6. Nucona

## Long-Term Business Partnership References
1. Instacart Health
2. Foodsmart
3. Season Health
4. FarmboxRx
5. Wholesome Wave
6. Partnership for a Healthier America

## Later Expansion Only
1. MenuFit
2. Spoonacular
3. Edamam
4. Kroger API
5. Nutritionix

---

# Final Rule for Pantry-Codex

Do not integrate any provider from this list without a specific founder-approved prompt.

When asked to evaluate a tool, Pantry-Codex should first answer:
- What problem does this solve?
- Is this required for the current MVP loop?
- Is there a cheaper/manual alternative?
- Does it improve repeat receipt scanning?
- Does it create dependency risk?
- Does it improve scoring trust or reward value?

Only build integrations that directly improve the core MVP loop or solve a real technical bottleneck.

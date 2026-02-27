Project 1: E-Commerce Product Metadata Validation
Scenario: LLM extraction of structured data from handcrafted jewelry descriptions for eBay listings.

The Problem: The model hallucinated a high-value gemstone ("Emerald") when the source text stated "Emerald-colored glass".
Business Impact: High risk of "Item Not As Described" returns, potential fraud claims, and loss of seller credibility.

Evaluator Notes: Identified gemstone inaccuracy and fixed Type Mismatches (numeric values like 45.00 and 925 incorrectly formatted as strings).
View Code: [jewelry_metadata_validation.json](./jewelry_metadata_validation.json.)

Project 2: Marketing Intent Classification (Social Media)
Scenario: Categorizing Instagram comments to identify high-value sales leads for a CRM team.

The Problem: The model failed to detect "conversion signals" (a wedding event and 30-day timeline), incorrectly labeling a "hot lead" as a low-priority inquiry.
Business Impact: Missed revenue opportunities and poor customer experience for users with immediate purchase intent.

Evaluator Notes: Corrected lead priority from "Low" to "High" after identifying the user's explicit intent to purchase for a wedding next month.
View Code: [marketing_intent_classification.yaml](./marketing_intent_classification.yaml.)

Project 3: JSON Sentiment & Entity Extraction
Scenario: Processing retail customer feedback to identify store improvements.

The Problem: Model failed to detect "Mixed" sentiment and omitted critical operational friction (store layout) from the summary.
Business Impact: Prevents managers from identifying friction, leading to decreased foot traffic and lost sales.

Evaluator Notes: Corrected sentiment from Positive to Mixed and resolved failures of completeness regarding operational feedback.
View Code: [customer_feedback_extraction.json](./customer_feedback_extraction.json.)

Project 4: YAML Content Quality Rubric (KDP Focus)
Scenario: Evaluating AI-generated book summaries for Amazon KDP based on "Gold Standard" rubrics.

The Problem: Model violated "No First-Person" guidelines by using "I" instead of "The author".
Business Impact: Unprofessional summaries decrease conversion rates on book listings.

Evaluator Notes: Adjusted tone consistency and guideline adherence scores; issued a final verdict that the content is not ready for publishing.
View Code: [content_quality_rubric.yaml](./content_quality_rubric.yaml)

Project 5: JSON Schema Integrity (Catalog Governance)
Scenario: Categorizing new inventory arrivals for a digital storefront.

The Problem: "Schema Drift"—the model misclassified home scent as jewelry and outputted numerical stock levels as strings.
Business Impact: Breaks search filters and prevents accurate inventory math, leading to supply chain reporting errors.

Evaluator Notes: Corrected category from "Jewelry" to "Decor" and resolved type mismatch for stock levels.
View Code: [inventory_schema_integrity.json](./inventory_schema_integrity.json.)

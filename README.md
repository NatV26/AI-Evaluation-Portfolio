Project 1: E-Commerce Product Metadata Validation
Scenario: An LLM was asked to extract structured data from a handcrafted jewelry description for an eBay listing.
The Problem: The model hallucinated a high-value gemstone ("Emerald") when the source text clearly stated "Emerald-colored glass."
Business Impact: This error would lead to "Item Not As Described" returns, potential fraud claims, and a loss of seller credibility.

**Link to Code:** [jewelry_metadata_validation.json](./jewelry_metadata_validation.json.)

Project 2: Marketing Intent Classification (Social Media)
Scenario: An AI was deployed to categorize Instagram comments for a jewelry brand to identify high-value sales leads for the CRM team.
The Problem: The model failed to detect specific "conversion signals" (a wedding event and 30-day timeline), incorrectly labeling a "hot lead" as a low-priority general inquiry.
Business Impact: This error leads to missed revenue opportunities and a poor customer experience for users expressing immediate purchase intent.

**Link to Code:** [marketing_intent_classification.yaml](./marketing_intent_classification.yaml.)

Project 3: JSON Sentiment & Entity Extraction (Customer Feedback)
Scenario: A retail chain uses AI to process customer feedback to identify store improvements.

The Problem: The model failed to detect "Mixed" sentiment, ignoring a major complaint about store layout. It also incorrectly formatted the review_id as a string and omitted the negative entity from its summary.

Business Impact: Misleading summaries prevent store managers from identifying critical operational friction, potentially leading to decreased customer foot traffic and lost sales.

**Link to Code:**  [customer_feedback_extraction.json](./customer_feedback_extraction.json.)


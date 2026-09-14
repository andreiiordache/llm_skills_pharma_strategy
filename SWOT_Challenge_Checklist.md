# AI SWOT Challenge Checklist

**Goal:** To rigorously challenge a given SWOT analysis, moving beyond simple listing to critical evaluation of each bullet point's validity, focus, and actionable utility in strategic planning.

This checklist is designed for an AI agent to iterate through every item in the S, W, O, and T lists, ensuring that the output is not merely "completed" but truly vetted by a consultant mindset.

Here are some general items in each SWOT category to prompt analysis of the text:

## Categories
### Categories for internal items (S, W)
iA   Human resources
iB   Physical resources
iC   Financial resources
iD   Activities and processes
iE   Past experiences

### Categories for external items (O, T)
eA  Future trends - in your field or the culture
eB  The economy
eC  Funding sources (foundations, donors, legislatures)
eD  Demographics
eE  The physical environment as the world changes (climate change, natural phenomena etc) 
eF  Legislation (new legislation coming into force, new rules about to be enforced etc)
eG  Local, national, or international events (concerts, wars, trade shows etc)

---
## **Agent Workflow / Core Algorithm**
*(Repeat this cycle for *every* bullet point on the SWOT list.)*

**Phase 1: Initial Reading & Categorization (Step 1)**
1.  Read and parse the current bullet (S, W, O, or T).
2.  Identify the core subject/claim of the bullet.
3.  Assign a preliminary confidence score to the claim (e.g., High/Medium/Low based on available data).

**Phase 2: Critical Interrogation (Step 2 - The Challenge)**
4.  Run through the set of critical questions below (based on Measurability, Phrasing, Allocation, and Usefulness) before proceeding to the next bullet.
5.  Provide a concise summary or 'Verdict' for this interrogation phase.

**Phase 3: Categorical Fit Assessment (Step 3)**
6.  Assess how well the challenged bullet fits its current category (S/W/O/T). Does it belong here, or is it misclassified?
7.  Provide a clear classification verdict.

**Phase 4: Iterative Conclusion (Step 4 - Wrap Up & Linkage)**
8.  Determine the strategic utility of the bullet for next steps (e.g., SO, WO, ST, WT Strategies). Is it just noise, or does it drive action?
9.  Conclude the evaluation for this specific bullet and move on.

---
## **Phase 2: Critical Interrogation Questions (The Challenge)**

*For each given SWOT bullet point:*

### A. Measurability & Quantifiability Check
*(Can we prove this?)*
1.  **Quantification Query:** Does the statement include any data, trend indicators, or measurable scale (e.g., "20% market share," "3-month revenue dip")? If not, what key metric should be added to make it debatable/testable?
2.  **Reversibility Check:** Have we quantified *why* this is a Strength/Weakness/Opportunity/Threat? (e.g., Is the weakness 'poor branding,' or is it quantified as 'social media engagement below industry standard x?')

### B. Phrasing & Clarity Check
*(Is this clear, debatable, and focused?)*
3.  **Specificity Query:** Is the statement too broad or vague (e.g., "Poor team morale")? Can we replace general terms with specific causes/examples? Is there a possibility that there are multiple ideas / items in one bullet? if multiple ideas, are they coherent or shall the user decouple them? 
4.  **Actionability Check:** Does the statement describe a *condition* (which is okay), or does it imply an action? If it implies action, what is that action?

### C. Allocation Check (S vs W / O vs T)
*(Is this internally focused, externally focused, and accurate to its pole?)*
5.  **Internal/External Query:** Does the item describe something *inside* our direct control (Resource)? If so, it belongs in S or W. Did we mistake an internal capability for an external market condition? Is it true?
6.  **Relationship Query:** Have we confirmed if this item is directly related to its classification? (e.g., A "Threat" must be something *outside* the organization; a "Strength" must be controllable.)

### D. Usefulness & Strategy Linkage Check
*(Will this actually help us make a decision?)*
7.  **Opportunity/Threat Risk Query:** If this is an Opportunity or Threat, what is the estimated impact (High/Medium/Low) and probability (High/Medium/Low)? Are we reacting to a low-probability event?
8.  **Leverage Potential Query (TOWS Matrix Focus):** Is there at least one immediate strategic path enabled by this bullet? (e.g., If W is 'High Cost,' can we use an O like 'New Market' that requires high spending, making the problem a constraint?)
### E. Web Verification Check (NEW)
(Can we verify this externally?)
9.  External Source Search: Run a focused web search on the core claim of the bullet point (e.g., "industry trend X," "competitor Y's performance"). Determine if the statement can be verified, debunked, or contextualized using reliable external sources. If verification is possible, summarize the findings; if not, flag it as a claim needing internal data.

---
## **Phase 3 & 4 Output Template for Each Bullet**

[Bullet Text]: *[Insert SWOT item here]*
* **Category:** [S/W/O/T] (Needs Re-evaluation? Yes/No)
* **Interrogation Summary:** [Brief summary of challenges found in A, B, C, and D.]
* **Web Verification Summary:** [Brief summary of challenges or confirmations found]
* **Final Verdict & Action Suggestion:** [A single concise statement that answers: *Is this item useful for developing a strategy? If not, how should it be refined or tagged as 'Noise'?*]
* **Format:** Preferred formats are MD files. For High/Medium/Low use ★★★/★★☆/★☆☆ and add words High/Medium/Low. 

**[END OF BULLET]**

Overall summary after listing all bullets should explain to the user which categories have been identified, how many and which categories are not present in the current analysis.Present as a Table.
Overall summary will also include a general confidence score per category. Present as table.

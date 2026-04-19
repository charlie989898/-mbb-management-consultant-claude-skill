# Issue Trees & Hypothesis Trees

The single most important analytical tool in consulting. Everything else — frameworks, analyses, decks — is downstream of the tree. If your tree is wrong, your work is wrong.

---

## The Core Distinction

**Issue tree:** Maps all the possible factors that could explain a problem. You don't know where the problem is yet — you're creating an exhaustive map to guide exploration. Good for initial problem structuring when you're genuinely uncertain.

**Hypothesis tree:** States your best guess about where the problem is, then tests it. You're not exploring — you're confirming or denying. Good when you have enough context to form a working hypothesis (which is most of the time after Day 1).

The best consultants use both together: start with an issue tree to ensure completeness (MECE), then prioritize branches into a hypothesis tree to guide where you actually spend time.

---

## MECE: The Governing Principle

Every branch of your tree must be:
- **Mutually Exclusive:** No overlap between branches. If "price" and "discount depth" are separate branches, you have overlap — discount depth is part of price.
- **Collectively Exhaustive:** No gaps. If you're decomposing revenue and only have "existing customers" and "new customers," you've excluded reactivated customers. That gap can hide the answer.

MECE isn't perfectionism — it's a practical guard against two specific failures: wasted effort (working on something that's already captured in another branch) and missed answers (leaving an important branch unexplored).

**The test:** Could someone read your tree and find every possible cause of the problem? Could they find each cause in exactly one place?

---

## How to Build an Issue Tree

**Step 1: State the root question precisely**

"Why are profits declining?" is too broad. "Why did EBITDA margin compress from 18% to 14% between FY2022 and FY2024 in the North America segment?" is precise enough to structure. Precision drives MECE structure. Vague questions produce vague trees.

**Step 2: Choose your decomposition logic**

There are five decomposition methods — pick the right one for the problem:

**A. Algebraic (best for financial problems)**
Break into a mathematical identity. Revenue = Volume × Price × Mix. Profit = Revenue − Costs. This is inherently MECE because math is MECE.

*Example: EBITDA margin compression*
- Revenue side: Volume effect | Price effect | Mix effect
- Cost side: COGS | SG&A | R&D | D&A

**B. Process (best for operational problems)**
Break into sequential stages. Each stage is a potential location for the problem.

*Example: Why is customer acquisition slow?*
- Awareness → Consideration → Trial → Purchase → Retention
Each stage is MECE (a customer can only be in one stage at a time) and collectively exhaustive (every customer journey goes through these steps).

**C. Segmentation (best for heterogeneous populations)**
Break into non-overlapping groups that cover the whole population.

*Example: Why is customer satisfaction declining?*
- By segment: Enterprise | Mid-market | SMB
- By region: North America | EMEA | APAC
- By product: Product A | Product B | Product C

**D. Conceptual (best for strategic problems)**
Use a logical framework. Not as rigorous as algebraic, but sometimes the right fit.

*Example: Why are we losing market share?*
- Internal factors: Product gaps | Pricing | Sales execution
- External factors: Competitor moves | Market shift | Customer preference change

**E. Binary (best when you're testing a single hypothesis)**
Is it A or not-A? Useful for fast triage.

*Example: Is this a volume problem or a price problem?*
Test volume first. If volume is fine, the problem is price/mix. If volume is off, decompose volume further.

**Step 3: Go to the right depth**

3-4 layers is usually right. Fewer = too vague to guide analysis. More = too detailed to see the structure.

*Layer 1:* Revenue vs. Costs
*Layer 2:* Revenue = Volume vs. Price vs. Mix
*Layer 3:* Volume = New customers vs. Existing customer growth vs. Churn
*Layer 4:* New customers = # of sales opportunities × close rate (now you're pointing to specific analyses)

**Step 4: Prune by priority before analyzing**

Don't analyze every branch. Before running any analysis, form a view on which branches are most likely to contain the answer and which you can quickly rule out.

The prioritization criteria:
- **Magnitude:** How much of the problem could this branch explain at maximum?
- **Likelihood:** Based on your early knowledge, how probable is this branch?
- **Testability:** How quickly can you confirm or deny this branch?

Start with branches that are high magnitude AND quickly testable. If you can rule out a branch in 20 minutes, do it first — you're eliminating dead ends and narrowing fast.

---

## Building a Hypothesis Tree

Once you have a working hypothesis, restructure the tree around it.

**Example:**
Question: Why is EBITDA margin declining?
Initial hypothesis: "Margin compression is driven by the shift to enterprise customers, who receive deeper discounts, not by cost increases."

Hypothesis tree:
1. **Is the margin decline on the revenue side or cost side?** → (Test: bridge analysis)
2. **If revenue side: is it price, volume, or mix?** → (Test: revenue decomposition)
3. **If mix: is enterprise % of revenue increasing?** → (Test: segment revenue split trend)
4. **If yes: are enterprise discounts higher than SMB?** → (Test: realized price by segment)
5. **If yes: is the enterprise mix shift intentional or unplanned?** → (Test: sales strategy vs. actual)

This is directive. Each node points to a specific analysis. You're testing the hypothesis from the top down, confirming branches or redirecting.

---

## The Ghost Deck Connection

The issue/hypothesis tree is the backbone of the ghost deck. Each terminal branch of your tree maps to a slide or analysis:

| Tree branch | Analysis | Slide |
|---|---|---|
| Revenue side — price effect | Realized price by segment vs. prior year | "Enterprise pricing held; SMB pricing declined 8%" |
| Revenue side — mix effect | Revenue % by segment over time | "Enterprise mix grew from 30% to 45%" |
| Cost side — SG&A | SG&A as % of revenue vs. peers | "SG&A in line with industry; not the driver" |

Before you do any analysis, the tree tells you exactly what slides you need. Before you write any slides, the tree tells you exactly what analyses to run.

---

## Common Tree Mistakes

**Solutioning instead of decomposing.** "We should cut costs" is not a branch of an issue tree — it's a recommendation. Branches describe potential causes or factors, not solutions.

**Overlap between branches.** "Customer acquisition" and "new customer sales" are the same thing. When branches overlap, you double-count the problem and miss the real decomposition.

**The catch-all "other" branch.** Having a branch labeled "other" means you haven't finished thinking. Either decompose "other" into something meaningful or eliminate it.

**Depth that doesn't add structure.** Adding layers for their own sake. If "Volume" → "Number of customers" → "Count of paying customers" isn't adding analytical clarity, you've over-branched.

**A tree nobody navigates.** Built it, presented it, filed it. A live hypothesis tree should be on the wall (or in the working doc) for the whole engagement, updated as branches are confirmed or denied.

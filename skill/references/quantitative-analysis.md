# Quantitative Analysis Reference: Working Consultant's Guide

This is how you actually do the quantitative work of consulting. Direct, practical, built from three years of client engagements. Not theoretical. Real protocols, real tools, real mistakes to avoid.

---

## 1. The First 30 Minutes with Any Dataset

When a client hands you data — Excel file, database export, financial report — follow this protocol before you do *any* analysis:

**Understand the schema**
- What does each column represent? Ask for the data dictionary.
- What's the grain? One row = one customer? One transaction? One day? One site?
- How many columns? How many rows? What's the time period covered?

**Check completeness**
- What's the row count? Does it match what the client said they'd provide?
- What time period? Are all months covered or are some missing?
- Are there obvious gaps — a spike in Jan 2023 then nothing until Mar 2023?

**Interrogate quality**
- Run a pivot table by year and month. Are all periods represented?
- Check for duplicates: Do you have the same transaction ID twice? Same customer in the same period twice?
- Nulls in critical fields: How many rows have blank revenue? Blank cost? Blank customer ID?
- Impossible values: Negative revenue? Dates in the future? Quantities that don't make sense?
- Are amounts reasonable? If it's revenue, does it align with the P&L? Within 2-3%?

**Understand provenance**
- Did a person manually enter this or did it export from a system?
- Which system? (SAP, Salesforce, a 1990s mainframe?) Systems have quirks.
- Does the client trust it? Have they caught errors before?
- Has the definition changed over time? "We added this field in Q3 2023" changes how you interpret earlier data.

**Cross-check totals**
- Sum the revenue in your dataset. Does it match the annual revenue in the financial statements?
- Not a perfect match? You now have a puzzle to solve before you can proceed. Don't ignore it.

**Why this matters**: One wrong assumption about data structure cascades through every analysis downstream. A client once handed us transaction data where each row represented 10 units but the column header didn't say so. We built a demand forecast off it. Wrong by an order of magnitude.

---

## 2. Core Excel Skills — The 80/20 Tools

These four tools show up in 80% of consulting analyses.

**Pivot tables**
- Fastest way to slice any dataset. Revenue by segment by quarter. Headcount by function by level. Cost by category by business unit.
- Don't overthink it. Drag dimensions into rows and columns. Drag metrics into values.
- Once the pivot is built, *then* ask "what's the insight here?" Pivots are exploratory, not answers.
- Tip: If your pivot table is huge and slow, you probably need SQL or Python instead of Excel.

**VLOOKUP and INDEX-MATCH**
- You're constantly combining datasets: Customer file + transaction file + product file.
- VLOOKUP does most jobs. But know its limits: can't look left, breaks if keys aren't unique, slow on huge datasets.
- INDEX-MATCH is more robust. Learn it. It's not harder.
- When combining datasets, *always* spot-check the results. Manual verification of 20 rows catches most errors.

**IF / SUMIF / COUNTIF**
- Don't manually label 10,000 rows. Write a formula: `=IF(revenue > 1000000, "Large", "Small")`
- SUMIF to aggregate by category: `=SUMIF(region, "North", revenue)`
- These formulas are faster than you, more reliable than you, and searchable later.

**Waterfall charts**
- The consultant's standard visualization for "why did X change from last period?"
- Revenue bridge: last year's revenue → volume effect → price effect → mix effect → new customers → churn → this year's revenue.
- Finance teams recognize them instantly. They're unambiguous.
- In Excel: Insert a waterfall chart (or build one with stacked columns if your version is old). Label every segment.

**Sensitivity tables**
- Non-negotiable for any recommendation with financial projections.
- Two-variable data table: vary assumption A across columns, assumption B down rows. Show output in each cell.
- Example: If you're forecasting EBITDA, show how it changes as revenue growth goes from 0-10% and EBITDA margin from 5-15%.
- This forces you to confront your assumptions and shows the client the range of outcomes.
- Build this before you present. It changes how you talk about the recommendation.

**Model architecture**
- Hard-code nothing. Create an assumptions tab. Reference it.
- Color code: blue for inputs, black for formulas, gray for intermediate calcs.
- Named ranges for key assumptions. Makes formulas readable: `=revenue * assumed_margin` instead of `=A5 * B27`.
- Someone else should be able to navigate your model without you explaining it.

**When Python > Excel**
- Dataset >500K rows (Excel slows down)
- Same analysis needs to run weekly/monthly with new data (automate it)
- You need statistical methods Excel can't handle (logistic regression, clustering)
- For most consulting work, Excel is sufficient.

---

## 3. Financial Statement Analysis — What to Read For

You're not memorizing statements. You're running a diagnostic to find signals.

**P&L — the diagnostic scan**

Revenue growth rate: Accelerating or decelerating? If it was 15% last year and 8% this year, something changed. Price, volume, or mix?

Gross margin: Is it expanding or compressing? If compressing, is it price pressure (clients won't pay more) or cost inflation (your supply costs are up)? Different problems.

Operating leverage: Is EBITDA margin growing faster than revenue? If not — if EBITDA margin is flat while revenue grows — your costs are growing with revenue. That's a scaling problem.

SG&A as % of revenue: Compare to peers. If you're at 25% and competitors are at 18%, you're either over-investing in growth or inefficient. The difference matters.

One-time items: Restructuring charges? Asset write-downs? Gain on sale of a business? Strip these out to see operating performance. One-time items obscure the real trend.

**Balance sheet — the leverage check**

Working capital: Calculate Days Sales Outstanding (DSO = AR / daily revenue), Days Inventory Outstanding (DIO = inventory / daily COGS), Days Payable Outstanding (DPO = AP / daily COGS).

- High DSO (>60) = you're not collecting from customers fast. Cash problem.
- Low DPO (<30) = you're not leveraging your suppliers. You're paying them faster than necessary.
- High DIO in a slow-growth business = cash tied up in inventory. Opportunity cost.

Cash and debt: How much cash runway do you have? What's the debt maturity profile? Any debt covenants you're near breaching?

Goodwill and intangibles: How much of the balance sheet is from acquisitions you made? Is goodwill being amortized or written down? If the company has $500M in goodwill on a $1B equity base, you've got impairment risk if performance dips.

**Cash flow — the reality check**

Is EBITDA converting to cash? (Cash conversion = FCF / EBITDA. Should be >0.8.)

What's consuming the cash? Working capital build (bad — you're funding growth through collections delays). Capex (necessary but compare to depreciation — if you're spending 2x depreciation, you're growing the asset base). Debt service (is it manageable relative to cash generation?).

Can they fund growth from operations or do they need external capital? Self-funding is stronger. Dependence on capital markets is riskier.

**Key ratios to internalize**

- Gross margin, EBITDA margin, EBIT margin — watch the trend
- Revenue growth: YoY and CAGR over 3-5 years
- Return on Invested Capital (ROIC) — single best measure of business quality
- Net Debt / EBITDA — leverage and debt capacity
- DSO, DIO, DPO — working capital efficiency
- Asset turnover — how much revenue per dollar of assets?

**Margin bridge analysis**

The standard tool for explaining profitability changes.

Start: Last year's gross margin = 40%
End: This year's gross margin = 38%

Bridge segments:
- Volume effect: Higher volume spread fixed costs → +0.5%
- Price effect: Pricing pressure in Q4 → -1.2%
- Mix effect: Shift to lower-margin products → -1.3%
- Cost changes: Supplier cost inflation → -0.2%

Sum = 40% - 1.2% = 38%

This is the standard. Finance teams expect it. It forces you to name what changed and quantify it.

---

## 4. Statistical Thinking for Consultants

Not a stats course. The intuition that actually matters.

**Correlation vs. causation**

High correlation between ice cream sales and drowning deaths. The causal variable is warm weather, not ice cream.

Before claiming causation, you need:
1. A plausible mechanism. "As temperature rises, ice cream sales increase *and* drowning increases."
2. Evidence that you've ruled out obvious confounders. (Is there a third variable driving both?)
3. Experimental evidence or a natural experiment. A/B test, or a time period where one variable changed but the confounder didn't.

If you only have correlation, say "correlation." The client will respect it more than an unsupported causal claim.

**Sample size and representativeness**

*For surveys:* 100 responses gives you ±10% margin of error (95% confidence). 400 gives ±5%. 1,000 gives ±3%. For most consulting work, 100-200 responses is enough to identify directional patterns.

*For interviews:* You're not doing statistics. You're looking for saturation — when additional interviews stop producing new themes. Usually 15-25 per major segment is enough.

Common mistake: "We did 5 customer interviews." That's signal, not research. Label it correctly. "Five interviews revealed patterns worth testing with a larger sample" ≠ "Customer research shows..."

**When a trend is real vs. noise**

Ask these questions:
- Is the sample large enough that this could be random?
- Does the trend show up consistently across subgroups or only in the full aggregate?
- Hold when you exclude outliers?
- Is there mean reversion risk? (If a metric was unusually high last period, it will probably come down regardless of what you do.)

Example: "Retention improved 3% this quarter." Is that real? Check: (1) Did 3% improvement require a sample of only 10 customers or 1,000? (2) Did it improve for all segments or just one? (3) Was last quarter abnormally low? If you can't answer these, you don't know if you've found signal or noise.

**Regression interpretation**

You probably won't run regressions, but you'll read them. Know what to check:
- R² > 0.7 = strong relationship
- Are coefficients statistically significant? (p < 0.05 means not random)
- Multicollinearity? (Are two predictor variables highly correlated? Then you can't trust which one matters.)
- Does the relationship make business sense? (Sometimes the math works but the story doesn't.)

**Distributions, not averages**

"Average NPS is 30" hides a lot. You might have 60% promoters (NPS 9-10) and 40% detractors (NPS 0-6).

Always ask: What does the distribution look like? Top quartile vs. bottom quartile? This is almost always a more useful question than "what's the mean?"

---

## 5. Model Building Discipline

How to build a model that's useful, not just correct.

**Architecture first**

Sketch the structure before you build:
- What are the inputs? (Assumptions, starting values)
- What are the outputs? (The answer you're solving for)
- What calculations connect them?

This prevents models that work but no one can understand.

**Assumption documentation**

Every assumption gets labeled and sourced:
- "Revenue growth: 8% (based on management guidance, cross-checked against analyst consensus, validated with top-10 customers)"
- Not hard-coded in row 47 with no label.

Future you and the client will thank you when you can defend where each number came from.

**Model hygiene**

- Inputs in one place (assumptions tab). Calculations separate.
- Color: blue for hard-coded inputs, black for formulas.
- No hard-coded numbers buried in middle of calculations.
- Named ranges for key assumptions. Makes formulas readable.
- Version control: date-stamp files. Keep old versions.

**Sensitivity tables before you present**

Build a 2-variable sensitivity table on your 2-3 most impactful assumptions. This:
1. Forces you to confront your assumptions
2. Shows the client the range of outcomes
3. Changes how you talk about the recommendation (from "we'll get to $100M" to "we'll get to $80-120M depending on...")

**Model audit before sharing**

- Does it add up? Check totals independently.
- Does it make sense at the extremes? (Set growth to 0%, then 100%. Does output move in the right direction?)
- Can someone else navigate it without you?

If you can't answer yes to all three, it's not ready.

---

## 6. Benchmarking Methodology

How to actually run a benchmarking analysis — not just "compare to average."

**Step 1: Define the metric precisely**

Not "profitability." Gross margin? EBITDA margin? ROIC? Be specific.

**Step 2: Define the peer set**

Same industry, similar business model, similar scale. Don't compare a direct-sales company (high SG&A) to a channel-sales company (low SG&A). Different structures, different baselines.

Aim for 8-12 peers. Enough for a range, not so many that you lose focus.

**Step 3: Source the data**

- Public companies: 10-K, 10-Q (SEC filings)
- Databases: Capital IQ, Bloomberg, Refinitiv
- Industry benchmarks: Hackett Group, APQC, McKinsey benchmarks
- Trade associations: Often publish anonymized benchmarks
- Mix sources. Don't rely on one.

**Step 4: Normalize for comparability**

Accounting differences matter. One company uses LIFO inventory, another FIFO. One accelerates revenue recognition, another doesn't.

Fiscal year ends: If you're comparing Q1 results across companies with different fiscal years, the seasons are different.

Business mix: If peer A makes 60% software (high margin) and peer B makes 20% software, their gross margins won't be comparable without adjustment.

Scale effects: Small companies often have worse ratios than large ones (less leverage, higher unit costs). Know this going in.

**Step 5: Interpret the gap**

Don't just show the gap. Explain what drives it.

"You're 5 points of SG&A below best-in-class" sounds like a problem to solve. But the drivers matter:
- Is it headcount efficiency? (Your competitors are more automated)
- Real estate? (You have cheaper locations)
- Go-to-market? (They spend more on sales)

The drivers determine what's actually actionable. Without understanding them, you can't recommend what to change.

---

## Final Check: Questions to Ask Before Any Analysis Leaves Your Desk

1. Does the data make sense? (Have you interrogated it?)
2. Can someone else follow your logic? (Is your model clear?)
3. Are your assumptions documented and defensible? (Can you explain where each came from?)
4. Have you stress-tested your conclusion? (What would have to change for it to flip?)
5. Does the magnitude pass the sniff test? (If you're recommending a 50% margin improvement, have you explained how?)

These five questions catch 90% of problems before they reach the client.

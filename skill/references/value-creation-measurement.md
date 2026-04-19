# Value Creation Measurement Framework

**Audience:** Principal and Director-level consultants (9-13 years experience)
**Purpose:** Quantify consulting impact for client boards, PE sponsors, and future business development
**Last Updated:** 2026-04-01

---

## Table of Contents

1. The Definite vs Derived Value Framework
2. Measuring Definite Value
3. Measuring Derived Value
4. Integrating Value Metrics into Engagements
5. Value Creation in Specific Contexts
6. Communicating Value to Stakeholders

---

## 1. The Definite vs Derived Value Framework

### Core Definitions

**Definite Value:** Direct, tangible, financially quantifiable benefits that appear in accounting statements or cash flows.
- Revenue growth: +$5M annual revenue from new customer segment
- Cost reduction: -$2M COGS through supply chain optimization
- Margin improvement: +8% contribution margin on existing product line
- Working capital release: $3M freed from inventory optimization
- NPV of strategic initiative: $25M present value over 5 years

**Derived Value:** Intangible, second-order benefits that create competitive advantage and reduce organizational risk.
- Employee engagement lift: NPS improvement from 45 to 62
- Process efficiency: Order-to-cash cycle time reduction from 45 to 18 days
- Strategic clarity: Board alignment on 3-year direction enabling faster decision-making
- Brand strengthening: Market perception shift enabling premium pricing
- Risk mitigation: Compliance framework preventing $50M+ regulatory exposure

### Why Both Matter

**Client perspective:** CFOs and boards need Definite Value to justify fees and satisfy audit committees. But they recognize Derived Value drives long-term competitive moats.

**PE sponsor perspective:** 100-day plans start with Definite Value estimates. Derived Value justifies premium exit multiples (6x EBITDA vs 5x) through operational excellence.

**Your value proposition:** Most competitors can identify Definite Value. Senior consultants uncover, measure, and realize Derived Value—where 30-50% of total impact often lies.

### The Measurement Hierarchy

| Level | Scope | Timeline | Confidence |
|-------|-------|----------|-----------|
| **Initiative level** | Single workstream (e.g., procurement savings) | Months | High (80-95%) |
| **Engagement level** | Full program across all workstreams | 6-18 months | Medium (60-80%) |
| **Portfolio level** | Multiple concurrent engagements + organic trends | 18+ months | Lower (40-60%) |

**Rule:** Measure with highest confidence at initiative level. Escalate rigorously to engagement and portfolio levels, clearly calling out attribution complexity.

---

## 2. Measuring Definite Value

### ROI Formulas for Consulting Interventions

**Basic ROI:**
```
ROI (%) = (Net Benefit / Consulting Fee) × 100

Example: Supply chain project realizes $2M savings, costs $400K
ROI = ($2M / $400K) × 100 = 500%
```

**Benefit-to-Cost Ratio:**
```
BCR = Total Benefits / Total Costs

Typical consulting BCR targets: 3:1 to 7:1
BCR < 2:1: Justify via strategic imperatives (risk, compliance)
```

**Payback Period:**
```
Payback = Consulting Fee / Monthly Benefit Run-Rate

Example: $2M savings realized over 12 months = $167K/month
Payback = $400K / $167K = 2.4 months (very strong)

Typical target: 6-12 months for transformation
```

### Cost-Benefit Analysis Methodology

1. **Identify all costs:** Consulting fees, internal resources diverted, system/tooling investment, change management
2. **Quantify benefits:** Separate one-time gains (headcount reduction accrual) from run-rate (annual savings)
3. **Apply conservative assumptions:** 80% realization rate year 1, ramp to 100% by year 3
4. **Discount future benefits:** Use client WACC (typically 8-12% for mid-market)
5. **Document attribution:** What % would have happened without consulting? (Usually 10-30% organic; you claim the lift)

**Template Calculation (24-month horizon):**

| Item | Months 1-6 | Months 7-12 | Months 13-24 | Total |
|------|-----------|-----------|------------|--------|
| **Benefits (annual run-rate $2M)** |  |  |  |  |
| Consulting realization rate | 30% | 70% | 100% | |
| Monthly benefit | $50K | $117K | $167K | $1.8M |
| Attribution adjustment (-20%) | -$10K | -$23K | -$33K | -$360K |
| **Net monthly benefit** | $40K | $94K | $134K | $1.44M |
| **Costs** |  |  |  |  |
| Consulting fees (front-loaded) | $300K | $100K | $0 | $400K |
| Internal resources | $50K | $50K | $0 | $100K |
| Systems investment | $75K | $25K | $0 | $100K |
| **Total costs** | $425K | $175K | $0 | $600K |
| **Period net benefit** | -$385K | -$81K | $1.608M | $1.142M |

**NPV @ 10% discount rate = $972K**
**3-year ROI = (1.142M / 0.6M) × 100 = 190%**

### EBITDA Tracking: Before and After

Establish baseline EBITDA in engagement kickoff (Month 0). Rebase at milestones.

**Definite Value components affecting EBITDA:**
- Revenue growth → higher EBITDA dollars
- COGS reduction → higher EBITDA margin
- OpEx reduction → higher EBITDA
- Working capital release → improves free cash flow (not EBITDA, but valued by PE)

**Example tracking dashboard:**

| Metric | Baseline | Month 6 | Month 12 | Attribution |
|--------|----------|---------|----------|------------|
| Revenue | $50M | $51.2M | $53.4M | +$3.4M (+6.8%) |
| COGS | $30M | $29.4M | $28.8M | -$1.2M supply chain work |
| OpEx | $12M | $11.8M | $11.4M | -$0.6M headcount, process |
| EBITDA | $8M | $10M | $13.2M | +$5.2M (65% increase) |
| EBITDA % | 16% | 19.5% | 24.7% | |

**Challenge:** Isolate consulting impact from market tailwinds, pricing, volume. Use control-based approach: "If no intervention, we'd expect 2-3% organic EBITDA growth = $160-240K. We achieved $5.2M, thus conservatively claim $4.96M of consulting value."

### NPV/IRR for Strategic Initiatives

**When to use:** Multi-year transformations, technology investments, market entries.

**NPV Formula:**
```
NPV = Σ [Annual Benefit / (1 + WACC)^Year] - Initial Investment

Example: 5-year supply chain automation
Year 0: -$2M investment
Years 1-5: +$800K annual benefit, WACC 10%

NPV = -$2M + $800K/(1.1)^1 + $800K/(1.1)^2 + ... + $800K/(1.1)^5
    = -$2M + $800K × 3.79 = $3.032M - $2M = $1.032M
```

**IRR (Internal Rate of Return):** Discount rate where NPV = 0. Target IRR: 25-40% for consulting-led initiatives.

Use Excel: `=IRR([-2M, 800K, 800K, 800K, 800K, 800K])` = 22.2%

### Revenue Attribution: Isolating Consulting Impact

**Challenge:** Revenue growth rarely flows from consulting alone. Disentangle from:
- Market expansion (organic 2-5%)
- Sales team scaling
- Product improvements
- Competitive dynamics

**Methodology:** Control group or time-series regression.

**Control Group Approach (most rigorous):**
- Treatment segment: Sales region with new sales playbook from consulting
- Control segment: Similar region without playbook
- Attribution = (Treatment growth % - Control growth %) × Revenue

Example:
- Treatment region revenue growth: +18%
- Control region revenue growth: +6%
- Incremental attribution: +12% = +$6M on $50M base
- Less 20% risk buffer for model error: = $4.8M attributed value

**Run-Rate vs One-Time:**
- One-time: Special order, margin on close-out; typically excluded from value
- Run-rate: Repeatable, expected to continue 3+ years; full inclusion justified

### Supply Chain Savings Quantification

**Procurement savings types:**

1. **Unit cost reduction:** Supplier consolidation, volume discounts, renegotiation
   - Formula: (Old price - New price) × Forecast volume × 3-year realization rate
   - Example: $5/unit → $4.50/unit, 500K units/year = $250K annual, 3-year = $750K

2. **Logistics optimization:** Inbound consolidation, network redesign, mode shift
   - Baseline cost per unit shipped; document new efficiency; multiply by volume
   - Typical savings: 8-15% of logistics spend

3. **Inventory optimization:** Days inventory outstanding (DIO) reduction
   - Formula: (Old DIO - New DIO) × (COGS / 365) × Carrying cost rate (20%)
   - Example: 60 DIO → 45 DIO, $30M COGS, 20% carrying cost
   - Savings = 15 × ($30M/365) × 0.20 = $246K annual

4. **Excess inventory liquidation:** One-time working capital release (not recurring)
   - Formula: Excess inventory value × Recovery %
   - Example: $2M excess stock sold at 60% of cost = $1.2M one-time cash

**Savings waterfall (annual, fully run-rate):**

| Driver | Savings | Confidence | 3-Year Value |
|--------|---------|-----------|-------------|
| Procurement | $500K | 90% | $1.35M |
| Logistics | $200K | 75% | $450K |
| Inventory optimization | $250K | 85% | $638K |
| **Gross savings** | **$950K** | **83% blended** | **$2.438M** |
| Less: Implementation cost | -$150K | | -$150K |
| Less: Benchmark conservatism (-15%) | -$142K | | -$365K |
| **Net value** | **$658K** | | **$1.923M** |

### Headcount Optimization Measurement

**Typical drivers:** Spans-and-layers restructuring, automation, process consolidation.

**Calculation:**
```
Annual savings = Headcount reduction × Fully loaded cost per employee
Fully loaded cost = Salary + Benefits + Overhead allocation + Recruitment costs

Example:
- 20 FTE reduction at $80K salary
- Benefits: 30% = $24K
- Overhead: 40% = $32K
- Fully loaded: $136K per FTE
- Annual savings: 20 × $136K = $2.72M

Less one-time separation costs:
- Severance (1.5 months): $17K per FTE × 20 = $340K
- Net 1-year value: $2.72M - $0.34M = $2.38M

Recurring 3-year value: $2.72M × 3 years = $8.16M
```

**Key guardrails:**
- Document productivity impact: Validate that output doesn't suffer post-reduction
- Include hiring/ramp costs if backfill needed: Often offsets 20-30% of gross savings
- Monitor attrition: Unplanned departures can erode savings

### Technology Investment ROI (Implementation Consulting)

**Framework for ERP, CRM, automation projects:**

```
ROI = (Annual Business Benefit - Annual Technology Cost) / Implementation Cost

Example: $3M ERP implementation
- Annual license/support: $200K
- Annual OpEx (IT labor, maintenance): $150K
- Total annual tech cost: $350K

Benefits realization (conservative estimates):
- Process automation, headcount reduction: $600K/year
- Inventory visibility improvement: $200K/year
- Decision speed (faster close): $150K/year
- Total annual benefit: $950K

Year 1 ROI: ($950K - $350K) / $3M = 20%
Year 3 cumulative benefit: ($600K × 3) = $1.8M
Net 3-year value: ($950K × 3) - ($350K × 3) - $3M = $1.5M
3-year ROI: 50%
```

---

## 3. Measuring Derived Value

### Organizational Health Index (OHI) Methodology

OHI combines employee engagement, process maturity, and strategic alignment into a composite score (0-100).

**Components (equal weighting, 25 points each):**

1. **Employee Engagement (0-25):** eNPS survey
   - Baseline eNPS + engagement survey at project start
   - Retest at 6 and 12 months
   - Target improvement: +15-20 eNPS points

2. **Process Maturity (0-25):** Capability assessment
   - Rate each process 1-5 (Ad-hoc to Optimized)
   - Baseline average: 2.1 (typical)
   - Post-engagement target: 3.5-4.0

3. **Strategic Alignment (0-25):** Board alignment survey
   - Question: "How clear is our 3-year strategic direction?" (1-10 Likert)
   - Baseline: 4.2, Target: 8.5+

4. **Decision Velocity (0-25):** Cycle time metrics
   - Track days to make major decisions (M&A, product, capex)
   - Baseline: 30 days, Target: 10-15 days

**Calculation example:**
- Engagement: 16/25 (eNPS 35→50)
- Process: 20/25 (avg 2.1→3.8)
- Alignment: 19/25 (clarity 4.2→8.0)
- Velocity: 18/25 (30 days→12 days)
- **OHI = 73/100** (baseline 45 → post-engagement 73)

**Valuation:** Correlate OHI gains to retention (reduces rehire cost), productivity (eNPS+10 = 2-3% productivity lift), and attrition risk.

### Employee Engagement and NPS Tracking

**eNPS (Employee Net Promoter Score):**
```
eNPS = % Promoters - % Detractors (Likert 0-10 question: likelihood to recommend company as employer)

Baseline interpretation:
- eNPS > 50: World-class (Microsoft, Apple)
- eNPS 30-50: Strong performer
- eNPS < 10: Retention risk

Our goal in engagement work: +15-20 eNPS point lift over 12 months
```

**Valuation: Cost of turnover**
```
Cost of 1% unplanned attrition = Headcount × 1% × Replacement cost (120% salary)

Example: 500-person company, avg salary $100K
1% attrition cost = 500 × 0.01 × $120K = $600K/year

If eNPS improvement reduces turnover from 12% to 9% (3% absolute):
Value = 500 × 3% × $120K = $1.8M
```

### Process Efficiency KPIs

**Standard metrics by domain:**

| Process | Baseline KPI | Post-engagement Target | Value Driver |
|---------|------------|---------------------|-------------|
| Order-to-cash | 45 days | 18 days | Working capital release: ($100M revenue / 365) × 27 days = $7.4M |
| Procure-to-pay | 20 days | 12 days | Automation saves 1.5 FTE @ $150K = $225K annually |
| Hire-to-productivity | 120 days | 60 days | Faster time-to-contribution; reduces ramp burden |
| Customer issue resolution | 15 days | 3 days | NPS improvement, reduced escalation |
| Decision-to-implementation | 30 days | 10 days | Market responsiveness; harder to quantify but strategic |

**Calculation template for O2C:**

| Metric | Baseline | Post-engagement | Days Improved | Financial Impact |
|--------|----------|-----------------|---------------|-----------------|
| Average days outstanding | 45 | 18 | 27 | |
| Annual revenue | $100M | | | |
| Daily revenue | $274K | | | |
| Working capital release | | | 27 × $274K = **$7.4M** | (1x benefit) |
| Cost of capital (10%) | | | $7.4M × 10% = **$740K** | (annual value) |

### Strategic Clarity Indicators

**Measurement approach:** Pre/post executive alignment survey.

**Survey questions (Likert 1-10):**
1. How clear is our 3-year strategic direction?
2. Do you know how your role connects to strategy?
3. Is resource allocation aligned with priorities?
4. Confidence in leadership's decision-making?

**Baseline typical: 4.2/10; Post-engagement: 7.8/10**

**Valuation:** Link to decision speed.
- Misaligned decisions = rework, delayed initiatives, missed opportunities
- Assume baseline: 20% of strategic decisions require major rework
- Post-engagement: 5% rework rate
- Savings: 15% × 10 major decisions/year × $100K avg rework cost = $150K annually

### Brand and Reputation Metrics

**Quantification approach:** Market perception study.

**Typical metrics:**
- Brand consideration: "Would you consider us as a vendor?" (% baseline → target)
- Pricing perception: "Our pricing is fair value" (Likert 1-10)
- Quality perception: "Best-in-class quality" (Likert 1-10)

**Financial linkage:**
```
Pricing elasticity approach:
- Baseline perception score: 6.2/10
- Post-engagement: 7.8/10
- Industry benchmark: 8.1/10

If +1.6 point improvement = +3% pricing power on $50M revenue:
Value = $50M × 3% = $1.5M annually
3-year NPV @ 10% discount = $1.5M × 2.49 = $3.74M
```

### Risk Mitigation Valuation

**Framework: Expected loss avoidance**

```
Value of risk mitigation = Probability of loss × Loss magnitude

Example: Compliance framework prevents regulatory penalties

Baseline risk:
- 40% probability of $10M fine if audit finds gaps
- Expected loss = 0.40 × $10M = $4M

Post-engagement:
- Framework reduces probability to 5%
- New expected loss = 0.05 × $10M = $500K

Value = $4M - $500K = $3.5M
```

**Common risk mitigation projects:**
- Compliance/regulatory: Reduced fine probability
- Cybersecurity: Breach cost avoidance
- Supply chain resilience: Business continuity risk reduction
- Governance: Shareholder lawsuit risk reduction

---

## 4. Integrating Value Metrics into Engagements

### Baselining: SOW and Kickoff

**In Statement of Work, define:**
- **Definite Value targets:** "$3-5M cost savings (80% confidence)"
- **KPIs to track:** Order-to-cash cycle, eNPS, EBITDA, headcount
- **Baseline measurement plan:** "Week 1: capture current state data"
- **Measurement cadence:** "Monthly tracking dashboards; 90-day formal review"
- **Attribution rules:** "Organic baseline estimated at 2%; consulting claims incremental impact"

**Kickoff activities (Week 1-2):**
1. Baseline data collection: Run COGS analysis, survey employees, measure process cycle times
2. Establish control groups: If possible, identify peer functions unaffected by consulting work
3. Create intake dashboard: Simple Profit & Loss view with pre-engagement state

### Mid-Engagement Tracking: Dashboards and Scorecards

**Cadence:** Monthly update; presented to steering committee.

**Dashboard structure (1 page):**

| Category | Metric | Baseline | Current | Target | Status |
|----------|--------|----------|---------|--------|--------|
| **Revenue & Margin** | Revenue | $50M | $51.8M | $54M | On track |
| | COGS % | 60% | 58.2% | 55% | Ahead |
| | EBITDA | $8M | $10.9M | $12M | Ahead |
| **Operations** | O2C days | 45 | 28 | 18 | On track |
| | Headcount | 500 | 490 | 475 | On track |
| **Engagement Health** | eNPS | +18 | +34 | +45 | Ahead |
| | Capability maturity | 2.1 | 3.2 | 4.0 | On track |

**Red flags triggering escalation:**
- Definite value >15% behind plan
- Engagement health (OHI, eNPS) declining
- Key process KPI deteriorating (quality, error rates)

### Post-Engagement Evaluation: 90-Day and 180-Day Reviews

**90-Day Review (shortly after engagement close):**
- Quantify realized benefits to date
- Identify gaps vs commitments; propose corrective actions
- Collect success stories for case studies
- Gather testimonials from exec sponsors

**Template:**
```
ENGAGEMENT: Supply Chain Transformation
CLIENT: Acme Manufacturing
TIMELINE: 6 months, closed Month 6

DEFINITE VALUE REALIZED TO DATE (90 days post-close):
- Procurement savings: $480K/year (vs $500K target, 96% realization)
- Logistics efficiency: $165K/year (vs $200K target, 83% realization)
- Headcount reduction accrual: $1.8M (vs $2.0M target, 90% realization)
- Working capital release: $4.2M (one-time, vs $4.5M target, 93%)

Total Definite Value realized: $6.645M (92% of 3-year NPV target of $7.2M)

DERIVED VALUE ACHIEVED:
- OHI improvement: 45 → 68/100
- eNPS lift: +15 points (retention risk reduced)
- Process maturity: 2.1 → 3.6 (avg)
- Decision velocity: -18 days (30→12 days)

CONFIDENCE IN SUSTAINABILITY: 88%
- Most benefits are structural (new processes, systems)
- Retention risk: ~5% of value if key personnel leave
- Recommendation: Monthly check-in at 6 months and 12 months
```

**180-Day Review (6 months post-close):**
- Confirm sustainability and identify erosion (typical: 5-15% of benefits drift)
- Update case study for business development
- Identify adjacent opportunities for Phase II work

### Value Tracking in PE Contexts: 100-Day Plans and Value Bridges

**PE 100-Day Plan approach:**

First 100 days post-acquisition focus on quick-win Definite Value (often $2-10M):
- Procurement synergies
- Cost structure optimization
- Working capital unlocking

**Example value bridge (PE add-on acquisition):**

```
ACQUISITION: Acme Food acquired for $100M EBITDA (6x multiple = $600M purchase price)

100-DAY VALUE CREATION:
│
├─ Revenue synergies: $5M EBITDA
│  ├─ Cross-selling existing products: $3M
│  └─ Eliminate redundant SKUs (margin lift): $2M
│
├─ Procurement: $4M EBITDA
│  ├─ Consolidate suppliers (3 → 1): $2.5M
│  └─ Negotiate volume discounts: $1.5M
│
├─ Headcount: $3M EBITDA
│  ├─ Eliminate redundant corporate: $2M
│  └─ Flatten management layers: $1M
│
├─ Overhead: $2M EBITDA
│  ├─ Consolidate facilities: $1.2M
│  └─ IT/finance process consolidation: $0.8M
│
└─ TOTAL 100-DAY VALUE: $14M EBITDA

POST-ACQUISITION EBITDA: $100M + $14M = $114M
NEW VALUATION @ 7x multiple: $798M (vs $600M entry)
VALUE CREATION: $198M (or 33% return in Year 1)
```

**Role of consulting:** De-risking value realization via post-acquisition integration management, ensuring execution against $14M target (typical realization: 85-95%).

### Designing Simple Dashboards for Ongoing Benefit Tracking

**Post-engagement sustainability requires client capability to self-track.**

**Year 1 dashboard (post-engagement, quarterly):**

**Finance view (for CFO):**
- EBITDA vs baseline (trended, 12 quarters)
- Headcount cost vs savings target
- Working capital as % of revenue (vs baseline)

**Operations view (for COO):**
- Key process KPIs: O2C days, procure-to-pay days, defect rates
- Staffing vs plan
- Utilization rates (if relevant)

**Culture view (for CHRO):**
- eNPS trend (quarterly survey)
- Voluntary turnover %
- Internal promotion rate (vs external hires)

**Design principle:** 1 page, quarterly update. Automated where possible (feeds from ERP, HRIS). Highlight changes vs prior quarter.

---

## 5. Value Creation in Specific Contexts

### PE/M&A: Due Diligence Value Sizing

**During M&A diligence, quantify value sources for 100-day and 3-year cases.**

**Process:**
1. Benchmark target EBITDA vs peers (often reveals cost gaps)
2. Identify revenue synergy levers: cross-selling, geography expansion, customer base consolidation
3. Quantify cost synergies: duplicate functions, vendor consolidation, OpEx reduction
4. Size standalone improvement opportunity: management changes, process optimization

**Example — Platform acquisition of three add-ons:**

| Value Source | Year 1 $ | Year 3 $ | Confidence | Rationale |
|--------------|----------|----------|-----------|-----------|
| **Revenue synergies** | $6M | $12M | 70% | Conservative cross-sell to existing base |
| **Procurement** | $3M | $6M | 85% | 3 vendors → 1; proven synergy from prior deal |
| **Headcount** | $4M | $4M | 80% | Eliminate 40 FTE duplicate corporate |
| **Overhead** | $1.5M | $1.5M | 75% | Consolidate real estate, IT |
| **Gross synergies** | $14.5M | $23.5M | 77% | |
| **Less: realization risk (20%)** | -$2.9M | -$4.7M | | Typical integration execution miss |
| **Less: duplicate JV costs** | -$1M | -$1M | | Transition period overhead |
| **NET SYNERGY VALUE** | **$10.6M** | **$17.8M** | | |

**At $100M EBITDA entry point, $10.6M Year 1 value = 11% EBITDA uplift; significant.**

### Post-Merger Integration Value Capture

**100-day plan execution typically achieves 80-90% of identified synergies; year 1-3 achieves 100-110% as new opportunities surface.**

**Consulting's role in PMI:**
- Validate assumptions (Are vendor relationships really consolidatable? Cost savings real?)
- Drive accountability (Weekly synergy realization dashboard; escalate misses)
- Remove obstacles (Internal politics delaying decisions; consultant acts as neutral expediter)
- Quantify unforeseen opportunities (As integration progresses, often identify additional $1-3M upside)

### Cost Transformation: Savings Waterfall and Run-Rate vs One-Time

**Typical cost transformation quantification:**

```
BASELINE COST STRUCTURE:
COGS: $30M (60% of revenue)
OpEx: $12M (24% of revenue)
Total controllable costs: $42M
Target: Reduce to $40M (80% of revenue) = $2M savings

WATERFALL (annualized run-rate):

Procurement optimization         $600K
├─ Supplier consolidation: 3→1  $350K
├─ Vendor volume discounts       $250K

Logistics efficiency             $400K
├─ Network optimization          $200K
├─ Mode shift (air → ground)     $200K

Manufacturing overhead           $500K
├─ Eliminate duplicate shifts    $300K
├─ Lean manufacturing            $200K

SG&A reduction                   $300K
├─ Shared service consolidation  $150K
├─ Process automation            $150K

Headcount optimization           $200K
├─ Attrition (no backfill)       $200K

GROSS SAVINGS:                   $2.0M (100% target achieved)

LESS: One-time costs in Year 1:
├─ Severance                     -$100K (one-time)
├─ System/tooling                -$50K (one-time)
└─ Training/transition           -$30K (one-time)

NET YEAR 1 BENEFIT:              $1.82M
YEAR 2+ ANNUAL RUN-RATE:         $2.0M (no one-time costs)
3-YEAR NPV @ 10%:                $5.35M
```

**Key distinction:**
- **Run-rate savings:** Repeatable, structural; count fully for 3-5 year case
- **One-time benefits:** Working capital, asset sales; count only once in Year 1; exclude from Year 2+ run-rate

### Revenue Growth: Pipeline Impact, Conversion Rate Improvements, Pricing Uplift

**Sales effectiveness consulting value chain:**

```
REVENUE GROWTH OPPORTUNITY: $50M → $56M (+12%, $6M incremental)

Attribution sources (estimated):
├─ Market growth (organic): 2% = $1M (exclude from consulting value)
├─ Pricing uplift: 3% = $1.5M
│  └─ Driver: Sales training on value-based selling (consulting led)
├─ Volume growth: 4% = $2M
│  ├─ Sales process improvement (faster close): 2% = $1M
│  └─ New product launch (go-to-market): 2% = $1M
└─ Sales force productivity: 3% = $1.5M
   └─ CRM implementation & training (consulting enabled)

Consulting attribution:
- Core credit (pricing, sales process): $2.5M (50% of non-organic)
- Partial credit (enablement): +$1.5M (50%)
- Total consulting value: $2.5M - $1.5M = $1M annually
- 3-year value: $2.5M (conservative, assumes some regression)
```

### Digital Transformation: Automation ROI, Process Digitization Savings

**Technology implementation value (RPA example):**

```
PROCESS: Invoice processing (P2P)
Baseline: 15 FTE, 20 days cycle time, 2% error rate

RPA AUTOMATION TARGET:
├─ 70% process automation via bots
├─ Remaining 30% human exception handling
├─ Cycle time: 20 days → 5 days (90% improvement)
├─ Error rate: 2% → 0.3% (compliance improvement)

FINANCIAL IMPACT:
├─ Headcount reduction: 10.5 FTE eliminated
│  └─ Cost: 10.5 × $80K fully loaded = $840K annual run-rate
├─ Cycle time improvement
│  └─ $100M COGS / 365 days × 15 days freed = $4.1M working capital release
│  └─ At 10% cost of capital = $410K annual benefit
├─ Error cost reduction
│  └─ 1.7% error rate reduction × 50K invoices × $10 cost/error = $85K
├─ Compliance risk mitigation
│  └─ Audit efficiency, reduced restatement risk = qualitative +

TOTAL YEAR 1 BENEFIT: $1.335M ($840K run-rate + $410K + $85K)
TECHNOLOGY COST: $400K (software + setup)
ROI: ($1.335M - $400K) / $400K = 234% in Year 1
PAYBACK: 3.6 months

3-YEAR VALUE: $1.335M × 3 = $4.005M (less tech cost) = $3.605M
```

### Organizational Redesign: Spans-and-Layers Savings, Productivity Improvements

**Typical organizational redesign value:**

```
BASELINE: 10 layers, average span of 3.5
REDESIGN TARGET: 7 layers, span of 5.5

QUANTIFICATION:
├─ Management headcount reduction: 120 → 75 managers (45 eliminated)
│  └─ Cost: 45 × $150K fully loaded = $6.75M annual
├─ Decision velocity improvement: 30 days → 12 days
│  └─ Enables faster market response (harder to quantify, ~5-10% revenue benefit)
│  └─ Conservative estimate: $2M annual uplift on $100M revenue
├─ Span improvement increases manager effectiveness
│  └─ Each manager oversees 5.5 vs 3.5 reports; process efficiency unlocks 10% additional output
│  └─ 75 managers × 10% productivity = 7.5 FTE value = $600K

GROSS VALUE: $6.75M + $2M + $0.6M = $9.35M annually

LESS: One-time severance & transition (2 months per departing manager)
   = 45 × $150K × 2/12 = $1.125M (one-time)

NET YEAR 1: $9.35M - $1.125M = $8.225M
YEAR 2+ RUN-RATE: $9.35M
3-YEAR VALUE: $9.35M × 3 = $28.05M
```

---

## 6. Communicating Value to Stakeholders

### The Value Creation Bridge (Waterfall Chart)

**Visual tool for board and investor presentations.**

**Layout:** Base (entry EBITDA) → Waterfall steps (each value driver) → Summit (exit EBITDA)

**Example waterfall:**
```
Entry EBITDA: $100M
   ↓ Revenue synergies:   +$6M
   ↓ Procurement:         +$4M
   ↓ Headcount:           +$3M
   ↓ Overhead:            +$2M
   ↓ One-time costs:      -$1M
   ↓
Exit EBITDA: $114M (14% uplift in Year 1)

Annotation below each bar:
- Dollar amount and % of total value
- Confidence level (90%, 85%, etc.)
- Key driver (e.g., "3→1 supplier consolidation")
```

**Pro tips:**
- Color bars: Green (revenue up), Red (cost down, but still positive impact)
- Include confidence levels: Helps set realistic expectations with investors
- Add "walk" from entry to exit multiple: $100M @ 6x = $600M → $114M @ 7x = $798M (33% value creation)

### Board-Level Value Reporting

**Quarterly reporting template to executive board:**

**Format: 2-page summary**

**Page 1 — Headline dashboard:**
```
ENGAGEMENT HEALTH SCORECARD

Value realization:        92% of plan (Green)
Timeline:                 On track (Green)
Key risks:               Low; supplier transition delay (Yellow)
Next escalation:         None unless >$500K variance

Definite Value Realized:
Q1: $2.1M (vs $2.5M plan, 84%)
Q2: $2.8M (vs $2.5M plan, 112%)
YTD: $4.9M (vs $5.0M plan, 98%)

Derived Value Progress:
eNPS: +12 points (target +20; on track)
OHI: 58/100 (baseline 42; target 70)
O2C cycle: 28 days (baseline 45; target 18)
```

**Page 2 — Narrative and next steps:**
- Key wins this quarter (story-based, not just numbers)
- Risks and mitigations
- Upcoming milestones (e.g., "Month 4: full procurement renegotiation closes; expect $600K realization")
- Recommendations for next phase (e.g., "Phase II: IT cost optimization, estimated $1.5M additional value")

### Procurement-Friendly ROI Narratives

**When justifying consulting fees to procurement teams, emphasize risk and guarantees.**

**Narrative structure:**
1. **The ask:** "Approve $500K consulting engagement"
2. **The minimum guarantee:** "We commit to at least $1.5M in documented savings (3:1 ROI minimum)"
3. **The upside:** "Typical client achieves $2-3M (4-6:1 ROI)"
4. **The risk:** "If we miss $1.5M target by >20%, we return 50% of fee"
5. **The reference:** "Three comparable companies in your industry achieved 4.2x ROI on average"

**Key: Make savings believable, not aspirational.**

### Case Studies as Proof Points for Business Development

**After project close, develop 1-2 page case study for BD use.**

**Template:**
```
CLIENT PROFILE: Acme Manufacturing, $200M revenue, 500 employees

THE CHALLENGE:
Supply chain costs rising 5% annually; working capital consuming $15M;
decision velocity slow (30-day approval cycles)

OUR APPROACH:
6-month supply chain transformation:
- Procure-to-pay process redesign
- Supplier base consolidation (15→6 vendors)
- Inventory optimization via demand sensing

RESULTS:
Definite Value:
- Procurement savings: $650K annual (vs $500K target, 130% realization)
- Working capital release: $4.2M (vs $3.5M target, 120% realization)

Derived Value:
- Decision velocity: 30 days → 12 days
- eNPS improvement: +18 points (retention risk reduced)
- OHI improvement: 45 → 71/100

TOTAL VALUE: $8.2M (3-year NPV), ROI 1,460% vs $500K fee

CLIENT QUOTE:
"[VP Operations] Our supply chain isn't just leaner—it's more agile. Decision-making
is dramatically faster. This engagement transformed how we operate."

BUSINESS DEVELOPMENT CALL-TO-ACTION:
If similar supply chain pressure exists in your business, we'd welcome a conversation.
Typical engagement: 4-6 months, $400-600K fee, $2-5M value delivery.
```

---

## Quick Reference: Formula Summary

**ROI:** (Net Benefit / Fee) × 100
**Payback Period:** Fee / Monthly Benefit Run-Rate
**Benefit-to-Cost Ratio:** Total Benefits / Total Costs
**NPV:** Σ [Annual Benefit / (1 + WACC)^Year] - Initial Investment

**Working Capital Release:** (Old DIO - New DIO) × (COGS / 365) × Carrying cost %
**Headcount Savings:** Headcount reduction × Fully-loaded cost per FTE
**eNPS Value:** Turnover reduction % × Headcount × Replacement cost (120% salary)

**Use with confidence. Update annually as client economics evolve.**

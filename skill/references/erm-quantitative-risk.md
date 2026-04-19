# Enterprise Risk Management & Quantitative Risk Analysis

## 1. Enterprise Risk Management Framework

### ISO 31000 & COSO ERM

The modern ERM function integrates three foundational frameworks:

**ISO 31000** (International Standard for Risk Management) provides principles, a 5-step process (establish context → identify → analyze → evaluate → treat), and ongoing monitoring. It's principle-based and applicable across sectors.

**COSO ERM 2017** (Committee of Sponsoring Organizations) is the corporate standard in North America, particularly for public companies. It defines ERM as "the culture, capabilities, and practices, integrated with strategy-setting and execution that organizations use to manage risk in creating, preserving, and realizing value." Key components:
- Governance & culture
- Strategy & objective-setting
- Performance (risk identification, analysis, response)
- Review & revision
- Information, communication, and reporting

Together, ISO 31000 and COSO form the backbone of credible ERM programs.

### Risk Taxonomy

Enterprise risks fall into six primary categories:

| Risk Category | Definition | Examples |
|---|---|---|
| **Strategic** | External or internal risks affecting competitive position, growth, or business model | Disruptive technology, market share loss, M&A integration failure |
| **Operational** | Risks from inadequate processes, systems, or people | Process breakdowns, system failures, human error, supplier disruption |
| **Financial** | Risks from liquidity, credit, currency, or commodity exposure | Foreign exchange volatility, interest rate swings, counterparty default |
| **Compliance & Regulatory** | Risks from non-compliance with laws or regulations | Regulatory fines, license revocation, legal judgments |
| **Reputational** | Risks from loss of trust, brand damage, or public perception failure | Product safety issues, environmental violations, executive misconduct |
| **Cyber** | Risks from data breaches, ransomware, or system compromise | Intellectual property theft, data breach, business interruption, supply chain compromise |
| **ESG** | Risks from environmental, social, or governance issues | Carbon emissions stranded assets, labor law violations, board dysfunction |

### Risk Appetite vs. Risk Tolerance

**Risk Appetite** is the amount and type of risk a board is willing to accept to achieve strategic objectives. It's a proactive statement of intent and is typically expressed in broad qualitative terms (e.g., "We maintain a low risk appetite for regulatory violations and a moderate appetite for operational innovation risk").

**Risk Tolerance** is the acceptable variation around risk appetite—operational boundaries. If risk appetite is 5-10% revenue volatility from market swings, tolerance might be +/- 2% around that range before escalation is required.

Best practice: Set risk appetite by category, specify risk owners, and connect to executive compensation (KRIs tied to incentives).

### Three Lines of Defense Model

| Line | Owner | Responsibility |
|---|---|---|
| **First** | Business units & operations | Day-to-day risk management, control design, monitoring |
| **Second** | Risk, Compliance, Quality functions | Policy setting, oversight, monitoring of first-line controls |
| **Third** | Internal Audit | Independent assessment of risk management and first/second-line effectiveness |

This structure prevents conflicts of interest and ensures both accountability and independence.

---

## 2. ERM Platforms: Selection & Implementation

### Platform Comparison

| Platform | Best For | Typical Cost | Implementation | Key Strength |
|---|---|---|---|---|
| **Riskonnect** | Mid-market operational + cyber risk | $100k-$300k/yr | 3-4 months | Unified operational + cyber workflows |
| **AuditBoard** | Public companies; audit + risk unified | $200k-$500k/yr | 4-6 months | SEC/SOX compliance built-in; audit integration |
| **LogicGate Risk Cloud** | Scalable, flexible workflows | $80k-$250k/yr | 2-3 months | Configuration flexibility; ease of use |
| **MetricStream** | Large multinationals, complex governance | $300k-$1M+/yr | 6-12 months | Scalability, GRC breadth, audit trail |
| **ServiceNow GRC** | Organizations already on ServiceNow | $150k-$600k/yr (with platform) | 4-8 months | Integration with IT Service Management |

**Selection Criteria:**
- Company size and geographic spread
- Current IT architecture (ServiceNow, SAP, Oracle)
- Primary risk focus (operational, financial, cyber, compliance)
- Public company vs. private (SOX/public company disclosures add cost)
- In-house IT maturity (custom workflows vs. out-of-box)

**Implementation Benchmarks:**
- Small/mid-market: 3-6 months, $200k-$400k total cost (software + implementation partner)
- Enterprise: 6-12 months, $500k-$2M+
- Annual software maintenance: 15-25% of implementation cost

---

## 3. Monte Carlo Simulation

### Methodology

Monte Carlo simulation generates thousands of iterations of a model, with random inputs drawn from probability distributions, to estimate output distributions and quantify uncertainty.

**Typical workflow:**
1. Identify key risk variables (capex cost, demand, price, margin)
2. Assign probability distributions to each
3. Specify correlations between variables (e.g., cost and schedule inflation are positively correlated)
4. Run 5,000-10,000 iterations
5. Analyze output distribution (percentiles, confidence intervals)

### Probability Distributions

| Distribution | When to Use | Characteristics |
|---|---|---|
| **Triangular** | Limited data; easy estimation of min/likely/max | Non-parametric; most common in consulting |
| **PERT** | Expert judgment; project management | Smooth; less extreme tail risk than triangular |
| **Normal (Gaussian)** | Market returns, financial metrics | Bell-curve; symmetric tails |
| **Lognormal** | Prices, costs (never negative); right skew | Skewed; useful for cost growth, market size |
| **Uniform** | Complete ignorance within bounds | All outcomes equally likely; rare in practice |

**Correlation Modeling:** Use correlation matrices to link inputs (e.g., demand and price are negatively correlated: -0.6). Tools typically accept Pearson correlation coefficients.

### Output Interpretation

Monte Carlo outputs are probability distributions, not point estimates. Key metrics:

- **P10, P50, P90**: 10th, 50th, 90th percentiles; read as "10% probability of result being lower; 50% is median; 90% is upper bound"
- **Expected Value**: Mean of output distribution
- **Range** (P10–P90): Uncertainty band
- **Confidence Interval**: E.g., "95% confidence NPV is between $50M–$80M"

### Value-at-Risk (VaR) & Expected Shortfall (ES)

**VaR(95%)** = "We are 95% confident losses will not exceed $X." Common in financial institutions (Basel III requires capital against VaR).

**Expected Shortfall (ES)** = Average loss in worst 5% of outcomes. More conservative than VaR and captures tail risk better. Regulators increasingly prefer ES.

### Tools

- **@RISK** (Palisade): Excel-based; industry standard; $995/user/year
- **Oracle Crystal Ball**: Excel-based; strong optimization; enterprise licensing
- **ModelRisk** (Vose): Advanced; custom distributions; $500/user/year
- **Lumivero**: Risk analysis and decision-making; mid-market focus

**Excel-Based Workflows:** All major tools integrate with Excel. Consultants often use @RISK or build custom VBA models for transparency and client control.

---

## 4. Decision Tree Analysis

### Methodology

Decision trees map a series of binary or multi-way decisions and uncertain outcomes, assigning probabilities and monetary values to each branch. They solve for Expected Monetary Value (EMV).

**Decision Node** (square): Represents a choice under management control.
**Chance Node** (circle): Represents an uncertain outcome.

**Rollback Method:** Working backward from final outcomes, calculate expected value at each node:
- At chance nodes: Sum (probability × outcome value)
- At decision nodes: Select branch with highest EMV

### Example: Drug Development

```
                          → FDA Approval (p=0.3) → Revenue $2B → EMV = $600M
Decision: Invest $200M →
                          → FDA Rejection (p=0.7) → Loss $200M → EMV = -$140M
                                                               Net EMV = $460M
```

### When to Use vs. Monte Carlo

| Aspect | Decision Tree | Monte Carlo |
|---|---|---|
| **Discrete choices** | Ideal | Not ideal |
| **Continuous variables** | Cumbersome (requires binning) | Natural |
| **Correlation complexity** | Simple | Handles well |
| **Audience communication** | Very clear; visual | Requires interpretation |
| **Typical use** | Go/no-go decisions, R&D, M&A deals | Financial projections, capex valuation |

**Sensitivity Analysis on Trees:** Vary branch probabilities and values; recalculate EMV. Identify which assumptions drive decisions.

---

## 5. Sensitivity Analysis & Tornado Diagrams

### Methodology

Sensitivity analysis determines which input assumptions most influence output (e.g., NPV, EBITDA margin, market share).

**One-Way Sensitivity:** Vary one input across a range (e.g., ±20%); plot output vs. input. High slope = high sensitivity.

**Tornado Diagram:** Rank inputs by sensitivity. Widest bars represent biggest impact. Visually dominates executive discussions.

**Partial Correlation Coefficients:** In Monte Carlo, measure correlation between each input and output. Ranges from -1 to +1; magnitude indicates impact. Often displayed as "importance rankings."

**Scenario Analysis vs. Sensitivity Analysis:**
- **Sensitivity:** "How does NPV change if discount rate moves 1%?"
- **Scenario:** "If economic recession occurs, how does the entire model change? (GDP down 3%, unemployment up 2%, capex delayed 6 months, margins compressed)"

Scenarios are more realistic but require more work.

---

## 6. Stress Testing

### CCAR/DFAST for Banks

**Comprehensive Capital Analysis and Review (CCAR)**: Federal Reserve stress test for large banks. Requires institutions to demonstrate capital adequacy under severe scenarios.

**Dodd-Frank Act Stress Test (DFAST)**: Broader regulatory stress test; all large banks must pass.

**Scenario Design:**
- **Baseline:** Current economic conditions
- **Adverse:** Recession scenario; unemployment +2-3%, GDP -2%, house prices -20%
- **Severely Adverse:** Deep recession; unemployment +4-5%, GDP -4%, house prices -35%

### Reverse Stress Testing

Rather than applying scenarios to a model, reverse stress testing asks: "What combination of events would threaten solvency?" This identifies unknown vulnerabilities and tail risks.

### How Consultants Build Stress Test Models

1. **Data Assembly:** Historical financials, macro variables, asset-liability breakdowns
2. **Regression Analysis:** Link P&L/balance sheet items to macro variables (unemployment, rates, commodity prices)
3. **Scenario Application:** Apply adverse/severely adverse assumptions to estimated relationships
4. **Capital Impact:** Calculate impact on capital ratios under stress
5. **Sensitivity & Correlation:** Test correlations between losses (e.g., do credit losses and market losses both hit simultaneously?)

Common deliverable: "Capital trajectory under stress" chart showing capital ratio over 9 quarters under each scenario.

---

## 7. Quantitative Risk in Consulting Engagements

### Major Project Risk Assessment

**Typical engagement:** An industrial company planning a $500M capex expansion. Risks include:
- Cost overrun (historical range: 10-30%)
- Schedule delay (typical: 6-18 months)
- Demand ramp slower than expected (historical variance in industrial: 20-40% lower than plan)

**Approach:**
1. Gather historical cost/schedule data from company's project portfolio
2. Build Monte Carlo model: capex, schedule, ramp assumptions
3. Output: P10/P50/P90 distributions for total cost and payback period
4. Sensitivity analysis: Identify cost inflation, ramp, and engineering scope as top drivers
5. Recommendation: Build contingency buffer (typically 15-25% for industrial projects) into business case

### M&A Risk Quantification

**Typical engagement:** Buyer due diligence on a $200M acquisition. Quantify downside risk.

**Model structure:**
- Base case revenue/EBITDA (from vendor due diligence)
- Downside case: Customer concentration materializes in loss; integration delay impacts revenue recognition
- Upside case: Cross-sell and cost synergies materialize

**Monte Carlo on multiple scenarios:** Generate distribution of post-acquisition EBITDA and IRR. Output: "We are 80% confident IRR will exceed hurdle rate; 20% risk of IRR shortfall."

### Capex Investment Risk & Supply Chain Risk Quantification

**Capex:** Model construction costs, equipment prices, labor inflation, permitting delays. Similar to project risk above.

**Supply Chain:** Quantify impact of supplier disruption. Model: supplier failure probability × inventory holding cost × time to alternative sourcing. Monte Carlo across supplier base.

---

## 8. Benchmarks & Implementation Timelines

### ERM Spend as % of Revenue

| Company Size | ERM Spend / Revenue |
|---|---|
| Fortune 500 bank | 0.08–0.15% |
| Large industrial | 0.03–0.06% |
| Mid-market | 0.05–0.12% |

Includes staff, software, consulting.

### ERM Software Costs

- **Software license:** $80k–$1M+/year (depends on platform, users, scale)
- **Implementation (partner services):** $100k–$2M (depends on complexity, scope)
- **Year 1 total:** Typically 1.5–3x annual software cost
- **Ongoing (Y2+):** Software + maintenance (~20% of implementation cost/year)

### Implementation Timeline

| Organization Size | Timeline | Team Size |
|---|---|---|
| Mid-market (1–2K employees) | 3–4 months | 2–3 FTE internal + 3–5 consultant FTE |
| Enterprise (5K+ employees) | 6–12 months | 5–10 FTE internal + 8–15 consultant FTE |
| Global with multiple geographies | 9–18 months | 10–20 FTE internal + 15–30 consultant FTE |

**Quick Wins (First 90 Days):**
- Risk appetite statement
- Risk register template and initial population
- KRI dashboard (basic)
- Quarterly risk reporting rhythm

**Full capability (12–18 months):**
- Integrated risk taxonomy across all categories
- Scenario analysis and stress testing
- Automated monitoring and escalation
- Board-level dashboard and reporting

---

## Key Takeaways for Practitioners

1. **Risk appetite drives strategy:** Explicit risk appetite statement must precede risk management program design.
2. **Tool selection follows function:** Choose platform based on risk profile (operational vs. financial), not brand name.
3. **Monte Carlo dominates quantitative work:** More flexible and realistic than decision trees for continuous variable portfolios.
4. **Sensitivity analysis is your best friend:** Tornado diagrams are the most effective way to communicate risk drivers to executives.
5. **Stress testing is non-negotiable:** Especially for regulated entities; increasingly standard for any large investment.
6. **Implementation is long:** Budget 6–12 months for enterprise ERM; 3–4 months for mid-market.
7. **Culture beats tools:** A well-defined risk appetite and three-lines-of-defense governance matter more than software sophistication.

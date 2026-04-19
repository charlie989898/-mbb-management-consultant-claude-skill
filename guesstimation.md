# Guesstimation: Structured Estimation Under Uncertainty

## Why This Actually Matters

Guesstimates aren't an interview parlor trick. You'll use them constantly once you're in client work. A partner asks "rough size of this opportunity?" in a meeting with the CEO. A stakeholder wants to know if it's worth digging into an analysis. You need to size something before the data team can even pull a report.

The real skill is **rapid decomposition under uncertainty** — breaking a big unknown into smaller, defensible estimates. It's not about getting the exact number. It's about getting to the right order of magnitude fast enough to be useful, and being able to explain your logic clearly.

## The Core Approach (Your Process)

Every estimate follows the same 4 steps. Internalize these so you can do them without thinking.

**1. Clarify the scope.** What exactly are we estimating?
- Which geography? Which time period? Which customer segment?
- US market or global? This year or annual run rate?
- Don't skip this. Half your estimates will fail because you estimated the wrong thing.

**2. Decompose into components.**
- Break the big number into smaller pieces you can actually estimate.
- Good decomposition: (TAM) = (Total addressable market) = (Total population) × (% in target segment) × (Average spend per person)
- Bad decomposition: "I'll just guess the total."

**3. Estimate each component.**
- Use anchors you know (population, GDP, salaries, business metrics).
- Adjust from analogies ("This is like that, but smaller").
- You're not pulling numbers from air — you're building from reference points.

**4. Sanity check.**
- Does the answer pass a sniff test?
- Cross-check with a different decomposition. If you get wildly different numbers, figure out why.
- Signal your confidence. "Around $200M, probably $150-300M range" is honest. "$47.3M" is probably false precision.

## Your Toolkit: Mental Models and Anchors

Carry these numbers in your head. You'll use them constantly.

**Population & Demographics**
- US: ~330M people, ~130M households, ~2.5 people per household
- India: ~1.4B people
- Global: ~8B people
- Typical workforce: ~50% of population, so US has ~165M workers

**Economics & Business**
- US GDP: ~$25 trillion per year (~$75K per capita)
- Median US household income: ~$70K
- A "large company": $1B+ annual revenue
- Fortune 500 threshold: ~$10-15B revenue
- SaaS gross margin: 70-80%
- Retail gross margin: 30-50%
- Professional services utilization: 65-75% (your time, billed)
- Corporate average salary: $80-100K; median is lower (~$60K)

**Time & Work**
- ~365 days per year; ~250 working days per year
- ~8,760 hours per year; ~2,000 billable hours per year
- ~22 working days per month
- That's roughly 40 billable hours per week, minus admin, learning, bench time

**Physical & Geographic**
- A football field ≈ 1 acre
- US land area: ~3.8M square miles; ~60% is non-urban
- A gallon of gas: ~5-6 lbs
- A typical car trip: 12,000 miles per year
- Manhattan: ~23 square miles, ~1.6M people (very dense; ~70K per square mile)

## Estimation Methods

Pick the method that fits the problem.

**Population-down approach**
Start from total population, segment down to your target.
- Market for yoga mats = (US population) × (% who exercise) × (% who do yoga) × (mats per person per year) × (price)
- Quick and intuitive; forces you to think about penetration

**Economic share approach**
What fraction of GDP or corporate spending does this represent?
- Market for project management software = (US corporate spending) × (% on software) × (% on project management)
- Good for B2B markets where you can anchor to business budgets

**Physical flow approach**
Volume × Frequency × Price
- Coffee revenue in NYC = (coffee shops) × (customers per shop per day) × (drinks per customer) × (price)
- Forces granular thinking about actual transactions

**Analogy method**
"This market is like that market, adjusted."
- The market for telemedicine will be ~30% of the market for traditional healthcare (adjusted for lower utilization)
- Requires a good reference market you actually know

## Worked Examples

These are real questions you'll face. Walk through each one out loud to see your own logic.

### 1. Market for Corporate Travel Management Software in the US

**Clarify:** Annual software spend by US companies on travel management platforms.

**Decompose:**
- US corporate employees: 130M households × 60% workforce participation = ~78M; take ~70% in companies large enough to use travel software = ~55M employees
- Companies with 500+ employees (the real market): US has ~5,000 companies this size
- Average spend per company: $1-5 per employee per year seems reasonable for a SaaS platform = $2/employee
- Plus enterprise deals: Top 100 companies might spend $5-10 per employee

**Estimate:**
- Middle market (5,000 companies × $2/employee × average 2,000 employees): ~$20B
- Wait, that's too big. Let me recalibrate.
- Actually: ~2,000 companies buy this category. Average spend: $200K-500K per year.
- Total: 2,000 × $300K = $600M

**Sanity check:**
- That's 600M/25T = 0.0024% of GDP. Seems low but plausible for a vertical software category.
- Cross-check: There are ~3,000 companies with 1,000+ employees. If 70% buy travel software and spend $300K average, that's 2,100 × $300K = $630M. Close.
- Answer: ~$500-700M range

### 2. Savings from 10% Reduction in Turnover (5,000 employees, $100K avg salary)

**Clarify:** Annual cost of employee turnover including recruiting, training, lost productivity. What does a 10% reduction save?

**Decompose:**
- Cost to replace one employee: recruiting (~$15K), onboarding + training (~$20K), lost productivity in first 6 months (~$40K per person). Total: ~$75K
- Current turnover: assume 15% annually in corporate environment = 750 people per year
- 10% reduction in turnover = 75 fewer people leaving per year

**Estimate:**
- 75 people × $75K cost to replace = $5.625M per year

**Sanity check:**
- That's 5.6M / (5,000 × 100K) = 11% of total payroll. Reasonable for turnover cost savings.
- Is 15% turnover realistic? Yes, typical for corporate is 12-18%.
- Answer: ~$5-6M per year

### 3. Coffee Shops in New York City

**Clarify:** Licensed coffee shops; retail coffee sales, not Starbucks corporate counted separately if relevant.

**Decompose:**
- NYC population: ~8M; Manhattan is ~1.6M
- In Manhattan (highest density), estimate one coffee shop per 1,500-2,000 people = ~800-1,000 shops in Manhattan alone
- Outer boroughs are less dense but still urban. Scale down to 1 shop per 2,500-3,000 people
- Brooklyn: ~2.6M people / 2,500 = ~1,000 shops
- Queens: ~2.3M people / 3,000 = ~750 shops
- Bronx + Staten Island: ~2.1M people / 4,000 = ~500 shops

**Estimate:**
- Total: 1,000 + 1,000 + 750 + 500 = 3,250 shops
- Plus chains (Starbucks, Dunkin, local chains): another ~500-1,000
- Total: ~3,500-4,000

**Sanity check:**
- That's 1 shop per 2,000-2,300 people. In a dense urban market, that feels right.
- Google says ~4,000 coffee shops. You just estimated like a consultant.

### 4. B2B SaaS Expansion Opportunity (500 enterprise customers at $200K ACV, expanding to SMBs)

**Clarify:** Annual revenue opportunity if you move downmarket to companies with $10-100M revenue (SMBs).

**Decompose:**
- Total addressable market (TAM) for your product in SMB segment:
  - US companies with $10-100M revenue: ~50,000 companies
  - Market penetration: assume you could capture 2% over 3-5 years = 1,000 customers
  - SMB ACV: Enterprise is $200K. SMBs typically buy 30-50% of that = $75K ACV
  - Annual recurring revenue from SMB: 1,000 × $75K = $75M at maturity

**Estimate:**
- Year 1: Ramp to 100 SMB customers = $7.5M ARR incremental
- Year 3: 400-500 customers = $30-40M incremental
- This is a $30-50M incremental business at scale

**Sanity check:**
- Your current business: 500 × $200K = $100M ARR
- Opportunity is 30-50% of current = meaningful but not game-changing
- Requires sales org change (SMBs buy differently). Risk: real but size checks out.

### 5. Cost to Process One Insurance Claim (200-bed hospital)

**Clarify:** Total cost to hospital to process, verify, and pay one insurance claim (not patient out-of-pocket, not insurance processing).

**Decompose:**
- Average claims per hospital per year: 200 beds × 70% occupancy × 8 days average stay × 2 claims per discharge = ~4,480 claims (order of magnitude: ~4,000-5,000)
- Total claims department cost:
  - Staff: 20 FTEs at $60K average = $1.2M
  - Systems + infrastructure: ~$500K
  - Total: ~$1.7M per year
- Cost per claim: $1.7M / 4,500 = ~$375 per claim

**Estimate:** ~$300-400 per claim

**Sanity check:**
- Does it pass intuition? 1-2 days of a claims processor's time at $150K (loaded cost) = ~$600-1,200. Your estimate of $375 assumes batching and automation. Reasonable.
- Cross-check from insurer side: Insurance companies spend ~$0.50-2.00 per claim to process (they're scaled). Hospital has more manual work. Your $375 is probably high but in the ballpark.
- Answer: $300-500 per claim

## How to Communicate an Estimate

You're in a meeting. The partner asks for your gut on a number. Here's how you sound credible.

**Set up your logic:**
- "Let me think through this. I'd start by..."
- "The way I'd break this down..."
- "Here's my working hypothesis..."

**Show the decomposition, not the answer first:**
- "There are roughly 330M people in the US. Of those, maybe 60% are in the workforce. Of those, maybe 40% work for companies large enough to use this software. That's roughly 80M employees. If..."
- People follow your logic, not your conclusion.

**Land the number with confidence but appropriate hedging:**
- Confident: "I'd estimate around $150M market size."
- Hedged but credible: "My estimate is around $150M, probably in the $100-200M range."
- Too hedged: "Could be anywhere from $50M to $500M." (Now it's useless.)

**Signal when you're uncertain:**
- "I'm less confident on this piece because..."
- "That component is my biggest assumption."
- Shows maturity, not weakness.

## Common Mistakes (Don't Do These)

**Not clarifying scope:** You estimate global market when they asked US. Wasted effort.

**Skipping decomposition:** "I think it's $500M" with no breakdown. No credibility.

**Anchoring to the first number you hear:** Someone says "$1B," you estimate around there. Wrong. Build from first principles.

**Being so hedged your estimate disappears:** "$20-500M" tells them nothing. Better to say "$100M, probably $70-150M."

**No cross-check:** You get $200M one way. You should always ask "how else could I validate this?" and do it.

**False precision:** "$47.3M" when your real answer is "around $50M." It signals you don't understand the limits of your own estimate.

**Confusing revenue with profit, market with TAM, annual with cumulative:** Clarify early.

## Building the Habit

You get better at this by doing it. A lot.

**Daily practice:**
- Pick one random estimate a day. ("How many tweets per day?" "What's the revenue of the sandwich market?")
- Do it out loud. Hear your own logic.
- Then look up the real number and calibrate.

**Calibrate your anchors:**
- When you see a real number, update your mental model.
- "That company's turnover cost was 1.2x salary, not 1.5x. I'll remember that."

**Do them with a partner:**
- A colleague checks your logic. "Wait, why did you assume that penetration rate?"
- You defend or adjust. Either way, you think harder.

**Track where you were wrong:**
- Keep a list of estimates you've done and the actual numbers.
- Your calibration gets better. Your decompositions get sharper.

The goal isn't perfection. It's to build the decomposition muscle so you can tackle any question, break it into pieces you actually understand, and deliver a credible answer fast. That's a superpower in consulting.

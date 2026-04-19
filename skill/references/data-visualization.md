# Data Visualization for Consultants

The chart is not the insight. The insight is the insight. The chart is just the fastest way to transfer it.

---

## The One Rule That Overrides Everything

**Every chart needs a message title, not a topic title.**

Wrong: "Revenue by Region"
Right: "APAC revenue grew 34% while North America declined — the mix is shifting"

The title is the "so what." The chart is the evidence. If someone reads only your title and gets the point, you've done it right. If they need to study the chart to understand what you're claiming, rewrite the title.

---

## Choosing the Right Chart

There are 5 questions your chart can answer. Pick the right chart for the question:

**Comparison:** How do things rank against each other?
→ Bar chart (horizontal for many categories, vertical for fewer)
→ Bullet chart when comparing actual vs. target

**Trend over time:** How has something changed?
→ Line chart (always for time series — never bar charts for time trends)
→ Area chart when showing cumulative volume or total matters

**Part of a whole:** What's the composition?
→ Stacked bar chart (better than pie — easier to compare and read)
→ Waterfall chart when showing how components add/subtract to a total (the consulting standard for bridges)
→ Avoid pie charts for more than 3 segments

**Distribution:** What's the spread?
→ Histogram for large datasets
→ Box plot when showing quartiles and outliers
→ Dot plot for small datasets where individual values matter

**Relationship between two variables:** How do they correlate?
→ Scatter plot
→ Bubble chart when a third variable adds meaningful context

**The most-used consulting charts:**
- Waterfall (bridges): explaining what changed from period A to period B
- Bar charts: comparisons, rankings
- Line charts: trends
- Scatter plots: benchmarking, positioning maps
- 2x2 matrices: strategic frameworks (not technically data charts, but the most-used visual)

---

## The McKinsey/BCG Chart Standards

**One message per slide, one chart per message.** If you have two insights, use two slides.

**Chart title = action title.** Full sentence. States the finding. Directs the reader's eye to what matters.

**Axis labels matter.** Every axis is labeled with units. No ambiguity about what's being measured or in what units.

**Source and notes always present.** Bottom of chart, smaller font: "Source: Company financials; Note: FY2024 figures adjusted for one-time restructuring charge."

**Highlight the key data.** If one bar in a bar chart is the point, color it differently from the others. Don't make the reader find it.

**Kill the chartjunk.** No 3D effects. No decorative shadows. No gradient fills. No background images. Every element that doesn't add information should be removed.

**Color palette: maximum 4 colors.** Primary insight color (your company's blue or black), contrast color for comparison, neutral gray for context, red for alerts/negatives. If you need more than 4 colors, you're probably combining too many datasets.

---

## Waterfall Charts: The Consulting Standard

The waterfall (bridge) chart is how consultants explain change. Use it for:
- Revenue bridge (what drove the change from last year to this year)
- Margin bridge (why did profitability change)
- P&L build (how do the components stack to the total)
- Any decomposition of a change into its drivers

**How to build it:**
- Start bar (where you began)
- Positive changes float above the axis in one color
- Negative changes hang below in another color
- End bar (where you ended)
- Label each segment with the absolute change AND the driver name

*Example — Revenue Bridge, FY2023 to FY2024:*
$400M → Volume +$35M → Price +$18M → New customers +$22M → Churn -$31M → FX -$12M → $432M

The reader immediately understands: growth despite churn and FX headwinds, driven by volume and new customers.

---

## Scatter Plots for Benchmarking

The scatter plot is the best way to show where your client sits relative to peers. Standard format:
- X axis: one variable (e.g., revenue growth)
- Y axis: another variable (e.g., EBITDA margin)
- Each dot = one company
- Client's dot is labeled and highlighted
- Draw a diagonal or trend line to show the typical relationship
- Companies in the "upper right" are best-in-class — high on both dimensions

Add a quadrant overlay (dotted lines at median values) to create a 2x2: companies are "Stars" (upper right), "Growing" (lower right), "Profitable but slow" (upper left), or "Challenged" (lower left).

The message title writes itself: "Client sits in bottom quartile on both growth and margin — significant gap to best-in-class peers."

---

## The Pyramid Principle Applied to Charts

Think of a page of charts like a pyramid. The top of the hierarchy:

1. **Key message** (one sentence in the slide title)
2. **Supporting evidence** (the charts themselves, 1-3 per page)
3. **Underlying data** (in the appendix, not on the main slide)

Never start with the data and work up to the insight. Lead with the insight and support it with data.

---

## Common Chart Crimes (And How to Fix Them)

**The data dump table.** A 12-column, 30-row table with no highlighting. Fix: Pick the 3-4 numbers that matter. Build a chart from those. Put the full table in the appendix.

**The truncated Y-axis.** Starting a bar chart at $47M instead of $0 makes a 2% difference look like 50%. Fix: Always start bar charts at zero. If you need to show small changes, use a line chart or label the delta explicitly.

**The spaghetti line chart.** Eight lines on one chart, all similar colors, crossing each other. Fix: Pick the 2-3 lines that matter. Gray out the rest as context.

**The 3D bar chart.** The third dimension adds no information and distorts perspective. Fix: Delete it. Always.

**The chart with no source.** "Where did this data come from?" is a question you don't want in a client meeting. Fix: Every chart has a source.

**The percentage that doesn't add to 100.** A pie chart where the slices sum to 97% (rounding error). Fix: Check your math. Round consistently. Add an "other" category to close the gap.

**Color-coding that means nothing.** Five bars in five different colors with no legend explanation. Fix: Color = meaning. One highlight color for the key data point. Gray for everything else.

---

## Presenting Charts Verbally

The talk track for a chart follows the same pyramid:

1. State the message: "What this chart shows is that our margin gap has widened significantly over the past three years."
2. Explain the structure: "We're comparing our EBITDA margin (the blue line) against the peer median (the gray)."
3. Point to the evidence: "You can see the gap was 2 points in 2021, but has grown to 8 points in 2024."
4. State the implication: "This tells us the gap is structural, not cyclical — and it maps to the period when we made two acquisitions at lower margins."

Never start with: "So this chart shows..." and then describe what the axes are before saying what it means. Lead with the message.

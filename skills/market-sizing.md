# Market Sizing — VibeCorp CoworkSkill

## COPY FROM HERE
```
You are a market sizing analyst. Your job is to help me build a credible, bottoms-up market size estimate and assess whether the timing is right to enter this market.

You will use two frameworks: TAM/SAM/SOM and the T-Score Market Timing methodology.

Do not use top-down market reports as the primary basis for sizing. Start from real unit economics and real customer counts, then build up.

---

PART 1: TAM / SAM / SOM

Define and calculate three numbers. For each, show the math explicitly — not a conclusion, but the actual multiplication.

TAM — Total Addressable Market
Everyone who could theoretically benefit from this solution, regardless of whether you can reach them or whether they're ready to buy. This is the ceiling. It is not your opportunity — it is the size of the universe.

Method: State the unit (number of people, number of companies, number of transactions), the price point (annual contract value, average transaction size, or willingness to pay), and the multiplication. Example: "14 million freelancers in the US × $600/year = $8.4B TAM." If you're unsure of the unit count, I will help you find a defensible proxy.

SAM — Serviceable Addressable Market
The portion of the TAM you can realistically reach given your go-to-market model, geography, language, distribution channel, and customer profile. This is where you are actually competing.

Method: Start from TAM and apply constraint filters one at a time. Show each filter and its effect on the number. Example: "US-only × English-speaking × companies with 10–500 employees × in industries where the problem is acute = 850,000 companies × $1,200/year = $1.02B SAM."

SOM — Serviceable Obtainable Market
What you can realistically capture in years 1–3, given your team, funding, sales capacity, and competitive environment. This is your planning number — it should be defensible, not aspirational.

Method: Estimate how many customers you can acquire given your current or planned GTM capacity. Use a bottoms-up model: "2 sales reps × 20 deals/year each × $18,000 ACV = $720K ARR by Year 1. Scale to 8 reps by Year 3 = $2.88M ARR." Then sanity-check this against your SAM: SOM should be less than 5% of SAM at the 3-year mark for an early-stage company.

After calculating all three, flag any number that required a significant assumption, and rate the assumption: [High confidence / Medium confidence / Low confidence — needs validation].

---

PART 2: T-SCORE MARKET TIMING

Score the market from 1–5 on each of the five T dimensions. A score of 1 = very unfavorable, 5 = highly favorable. Be honest — an inflated T-Score is useless.

T1 — Technology Readiness
Is the enabling technology mature, stable, and accessible enough to build on? Score 5 if the core tech is proven and commodity. Score 1 if you're betting on technology that doesn't exist yet or is still in research phase. Explain the specific technology dependency and its current maturity level.

T2 — Talent Availability
Can you hire the people you need to build and sell this? Score 5 if the required skills are abundant and hireable at reasonable cost. Score 1 if the key skills are scarce, require years of experience to develop, or are dominated by a small number of institutions. Identify the 2 hardest roles to fill and assess market supply.

T3 — Adjacent Trend Timing
Are complementary markets, behaviors, or regulations growing in a way that creates tailwind for this market? Score 5 if 2+ adjacent trends are accelerating in your favor. Score 1 if adjacent markets are contracting or moving away from your assumptions. Name the specific adjacent trends and assess whether they are accelerating, stable, or decelerating.

T4 — Tolerance for Change
How ready is the target market to switch from their current solution? Score 5 if there is active dissatisfaction, a triggering event (regulation, cost increase, competitive pressure), or the incumbent has degraded. Score 1 if the market is locked in by long contracts, high switching costs, or deep institutional inertia. Identify the specific switching cost and what would overcome it.

T5 — T-Minus Runway
How long until the timing window closes? Is this market about to be flooded by well-funded competitors? Is there a regulatory or technology shift that will make the opportunity irrelevant? Score 5 if the window is open and stable (2–5+ years). Score 1 if the window is closing fast (under 12 months) or you are already late. Assess the competitive velocity and any known upcoming catalysts that could close the window.

---

T-SCORE CALCULATION AND INTERPRETATION

Average the five scores:

T-Score = (T1 + T2 + T3 + T4 + T5) / 5

4.0–5.0: Exceptional timing. Strong tailwinds, low friction, window is open. Move fast.
3.5–3.9: Good timing. Proceed with confidence. Monitor the one or two lower scores closely.
2.5–3.4: Mixed timing. You can enter, but identify and actively manage the weak dimensions. Expect friction.
1.5–2.4: Poor timing. Either too early (technology or market not ready) or too late (window closing, market locked). Consider waiting or repositioning.
1.0–1.4: Wrong moment. The conditions for success are not present. Do not confuse a contrarian position with a bad-timing position — these are different things.

---

FINAL OUTPUT

Produce a Market Sizing Summary in this format:

TAM: $[X]B — [one sentence on methodology]
SAM: $[X]M or $[X]B — [one sentence on key constraints applied]
SOM (3-year): $[X]M — [one sentence on GTM assumption]

T-Score: [X.X] / 5.0
- T1 Technology Readiness: [score] — [one line]
- T2 Talent Availability: [score] — [one line]
- T3 Adjacent Trend Timing: [score] — [one line]
- T4 Tolerance for Change: [score] — [one line]
- T5 T-Minus Runway: [score] — [one line]

Timing Assessment: [Exceptional / Good / Mixed / Poor / Wrong moment]

Key Risks to This Sizing:
1. [Most dangerous assumption]
2. [Second most dangerous assumption]
3. [One external event that would materially change the numbers]

---

Start by asking me: "Describe the market you're trying to size in one sentence — what does your solution do, and who buys it?"
```
## COPY TO HERE

---

## Framework & Methodology

### TAM/SAM/SOM: Why Bottoms-Up Matters

The standard mistake in market sizing is **top-down reasoning**: find a market research report, cite a TAM figure, and apply a percentage capture rate. This produces numbers that are defensible in presentation but useless for planning.

A $50B market report tells you almost nothing about whether you can build a $5M ARR business. It does not tell you who specifically will pay, what they will pay, or how fast you can reach them. The bottoms-up approach forces you to answer those questions before you can produce a number — which is exactly the discipline that makes the exercise valuable.

The three-layer model works as a funnel:

- **TAM** is a ceiling check — is the total universe of value large enough to support a venture-scale or sustainable business? If the TAM is $50M, a 10% capture rate is a $5M business, which may or may not be worth the risk profile.
- **SAM** is a realism check — most teams dramatically overestimate how much of a market they can actually serve. Geography, language, integration requirements, regulatory constraints, and go-to-market capacity all narrow the reachable universe. The filters applied to get from TAM to SAM are often more revealing than the numbers themselves.
- **SOM** is a planning check — it anchors financial projections to operational capacity rather than market share fantasy. The "under 5% of SAM at 3 years" sanity check is a practical heuristic: early-stage companies that project 20% market share in year 3 are not being ambitious, they are being unserious.

### T-Score: An Original Framework for Market Timing

The T-Score framework addresses a gap in standard market analysis: **market size and market timing are independent variables, and both matter.** A large market at the wrong moment is not an opportunity — it is a graveyard of well-funded companies that were right too early (or too late).

The five dimensions were selected because they cover the primary categories of timing risk:

| Dimension | Risk Category |
|---|---|
| Technology Readiness | Infrastructure risk |
| Talent Availability | Execution risk |
| Adjacent Trend Timing | Market momentum risk |
| Tolerance for Change | Customer adoption risk |
| T-Minus Runway | Competitive timing risk |

A company can have an excellent market (large TAM, well-defined SAM) and a poor T-Score — meaning the market exists but the conditions for success are not yet present. Conversely, a company with a modest market can have an excellent T-Score — meaning the window is open, friction is low, and the time to move is now.

The 3.5 threshold is a practical judgment call derived from the observation that markets below this threshold typically require either category creation (expensive and slow) or tolerance for a prolonged adoption curve that most startups cannot fund. It is not a hard rule — context matters — but it is a useful flag.

---

## Example Usage

**User:** I'm building an AI-powered contract review tool for small law firms (1–10 attorneys).

**Claude:**

Let's build this out.

**PART 1: TAM / SAM / SOM**

**TAM**
There are approximately 49,000 law firms in the US with fewer than 10 attorneys, plus roughly 310,000 solo practitioners. That's ~360,000 potential units. At an estimated $1,800/year ACV for a professional AI tool (based on comparable legal software pricing), that yields:

360,000 firms × $1,800/year = **$648M TAM**

Assumption confidence: Medium. The firm count is from ABA data (high confidence). The $1,800 ACV is an estimate — needs validation against actual willingness to pay.

**SAM**
Apply filters:
- US-only, English-language (removes ~30%): 252,000 firms
- Firms with sufficient contract volume to justify a dedicated tool (exclude pure litigation-only practices, estates-only, criminal defense): roughly 40% of small firms do transactional work regularly → 100,800 firms
- Firms with at least some tech adoption (exclude fully paper-based, which is ~25% of small firms): 75,600 firms
- Firms currently not using a large enterprise vendor like Thomson Reuters or Lexis (who have their own contract tools): remove ~15% → 64,000 firms

64,000 firms × $1,800/year = **$115M SAM**

Assumption confidence: Medium-Low. The "transactional work" filter is estimated; actual number needs validation.

**SOM (3-year)**
Assuming product-led growth with a freemium layer converting at 3%, plus a small inside sales team (2 reps by Year 2):
- Year 1: 150 paying customers × $1,800 = $270K ARR
- Year 2: 600 customers (PLG growth + 2 reps) = $1.08M ARR
- Year 3: 1,800 customers (PLG compound + 4 reps) = $3.24M ARR

SOM at 3 years = **$3.24M ARR**
Sanity check: $3.24M / $115M SAM = 2.8% — within the <5% heuristic. Reasonable.

---

**PART 2: T-SCORE**

**T1 — Technology Readiness: 4**
Large language models capable of contract analysis are proven and commercially accessible (OpenAI, Anthropic, Google). The technology risk is in accuracy and hallucination management for legal-grade output — this is a real engineering challenge but not a research problem. Technology is ready; execution quality is the variable.

**T2 — Talent Availability: 3**
ML engineers are competitive but available. The harder hire is someone who understands legal workflows deeply enough to build a product attorneys will trust. Legal-tech product expertise is scarce. Rating reduced by the difficulty of the legal domain expertise requirement.

**T3 — Adjacent Trend Timing: 5**
Law firm AI adoption is accelerating sharply following GPT-4's release. Client pressure to reduce legal costs is increasing. Bar associations are actively publishing AI guidance (rather than prohibiting it). Multiple adjacent tailwinds are accelerating simultaneously.

**T4 — Tolerance for Change: 3**
Small firm attorneys are conservative technology adopters. Liability concerns around AI-generated legal analysis are genuine and not fully resolved. However, the economics are compelling (reducing associate time) and solo practitioners have no legacy infrastructure to protect. Mixed.

**T5 — T-Minus Runway: 3**
Window is open but narrowing. Well-funded competitors (Harvey, Ironclad, Kira) are primarily targeting enterprise; the small firm segment is less contested today. But enterprise players will move downstream within 2–3 years as they saturate the enterprise market. 18–36 month window to establish a defensible position.

**T-Score: (4 + 3 + 5 + 3 + 3) / 5 = 3.6 — Good Timing**

---

**Market Sizing Summary**

TAM: $648M — 360,000 US small law firms × $1,800/year ACV
SAM: $115M — filtered to transactional-focused, tech-adopting firms not locked into enterprise vendors
SOM (3-year): $3.24M ARR — PLG conversion + inside sales, 1,800 customers at Year 3

T-Score: 3.6 / 5.0 — Good Timing
- T1 Technology Readiness: 4 — LLMs proven; execution quality is the variable
- T2 Talent Availability: 3 — ML engineering available; legal domain expertise scarce
- T3 Adjacent Trend Timing: 5 — legal AI adoption accelerating with multiple tailwinds
- T4 Tolerance for Change: 3 — conservative adopters, liability concerns, but strong economics
- T5 T-Minus Runway: 3 — 18–36 month window before enterprise players move downstream

Timing Assessment: Good

**Key Risks to This Sizing:**
1. ACV assumption ($1,800/year) is unvalidated — small firms may only sustain $600–900/year, which cuts SAM and SOM by 50–67%
2. "Tolerance for Change" score could deteriorate quickly if a bar association issues restrictive AI guidance
3. If Harvey or Ironclad launches a small-firm tier in the next 12 months, the competitive window compresses significantly

---

## When to Use

- Before fundraising — investors will ask for market sizing; bottoms-up numbers are far more credible than top-down report citations
- When evaluating a new market segment or geographic expansion
- When the team is debating whether a market is "big enough" — this turns the debate into a calculation
- Before making a significant GTM investment (hiring a sales team, launching paid acquisition) — SOM tells you what the realistic ceiling on that investment is
- When assessing a potential acquisition target or partnership

## When NOT to Use

- Before the problem is validated — market sizing an unvalidated problem produces a precise answer to the wrong question; use the Problem Validation skill first
- As the primary basis for a pricing decision — SOM and ACV are interdependent; pricing work needs its own framework
- When the market is so new that no comparable data exists — in genuinely novel markets, bottoms-up sizing requires analogies from adjacent markets, which introduces compounding uncertainty that this framework will surface but cannot resolve
- As a substitute for customer development — knowing the market is large does not mean you know how to reach it or sell into it

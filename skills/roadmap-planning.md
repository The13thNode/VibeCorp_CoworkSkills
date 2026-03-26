# Roadmap Planning — VibeCorp CoworkSkill #9

Build prioritized, defensible roadmaps using structured frameworks. Cut through opinion wars and align your team on what gets built, when, and why.

---

## COPY FROM HERE

You are a senior product strategist and roadmap planning expert. Your job is to help me build a prioritized, realistic roadmap that aligns with business goals and team capacity.

Work through this in a structured way:

**Phase 1 — Current State Audit**
Ask me:
- What product/initiative am I roadmapping? (new product, feature backlog, company OKRs, etc.)
- What is the time horizon? (next quarter, 6 months, 12 months, 3 years)
- What are the 1-3 most important business goals this roadmap must serve?
- What constraints exist? (team size, budget, technical debt, dependencies, market timing)
- Who is the roadmap audience? (engineering team, board, customers, investors)
- What does my current backlog or list of initiatives look like? (ask me to share it)

**Phase 2 — Prioritization**
Once I share my initiatives, apply the right framework(s):

1. **MoSCoW Method** — Sort everything into:
   - Must Have: Non-negotiable for the goal/deadline to be met
   - Should Have: Important but not critical; defer if needed
   - Could Have: Nice-to-have; only if time and capacity allow
   - Won't Have (this time): Explicitly out of scope for this cycle

2. **ICE Scoring** — Score each initiative 1-10 on:
   - Impact: How much will this move the needle on the key metric?
   - Confidence: How sure are we this will work as expected?
   - Ease: How easy is it to implement? (10 = very easy)
   - ICE Score = Impact × Confidence × Ease
   Rank items by ICE score and flag outliers worth discussing.

3. **RICE Scoring** (for initiatives with enough data):
   - Reach: How many users/customers affected per period?
   - Impact: Effect per individual (use scale: 3=massive, 2=significant, 1=medium, 0.5=low, 0.25=minimal)
   - Confidence: % certainty (100% = high, 80% = medium, 50% = low)
   - Effort: Person-months of work
   - RICE Score = (Reach × Impact × Confidence) / Effort
   Higher score = higher priority.

4. **One Metric That Matters (OMTM)** — Identify the single metric each phase of the roadmap is optimizing for. Everything should trace back to it.

**Phase 3 — Sequencing and Sprints**
- Map dependencies: What blocks what? Identify the critical path.
- Time-box into sprints: Suggest how to group work into 2-week sprints with realistic capacity assumptions.
- Flag risks: What could derail the timeline? What are the top 3 assumptions we're betting on?

**Phase 4 — Communication Templates**
Based on the audience, produce the right format:
- Team view: Detailed sprint-by-sprint with owners and acceptance criteria
- Board/investor view: Outcome-focused, strategic milestones, no implementation detail
- Customer-facing view: Themes and timeframes only ("Coming soon", "In progress", "Done")

Throughout, challenge my assumptions. Ask "why now?" for high-priority items. Push back on scope creep. Help me say no with evidence.

Let's start. Ask me Phase 1 questions one section at a time.

## COPY TO HERE

---

## Framework Reference

### MoSCoW Method

A categorization technique that forces explicit prioritization decisions.

| Category | Definition | Guidance |
|---|---|---|
| Must Have | Failure condition if missing | Limit to 40-60% of capacity |
| Should Have | Strong business case, not time-critical | 20-30% of capacity |
| Could Have | Desirable, low cost of exclusion | 10-20% of capacity |
| Won't Have | Explicitly deferred | Document the decision and reason |

The discipline is in the Must Have list. If everything is a Must, nothing is. Force yourself to cut until it genuinely hurts.

### ICE Scoring

Best used for: Early-stage backlogs, teams without strong usage data, quick relative ranking.

```
ICE Score = Impact (1-10) × Confidence (1-10) × Ease (1-10)
Max score: 1,000
```

Scoring anchors:
- Impact 10: Directly doubles a key metric
- Impact 5: Measurable but modest improvement
- Impact 1: Negligible effect
- Confidence 10: Proven by data/prior experiments
- Confidence 5: Strong hypothesis, some supporting evidence
- Confidence 1: Pure speculation
- Ease 10: Hours of work, no dependencies
- Ease 5: 1-2 week effort, manageable complexity
- Ease 1: Months of work, heavy dependencies

ICE favors quick wins. Balance it against strategic bets with lower ease scores.

### RICE Scoring

Best used for: Product teams with usage data, comparing features for a defined user base.

```
RICE Score = (Reach × Impact × Confidence%) / Effort
```

Example:
- Feature A: Reach 5,000 users/month × Impact 2 × Confidence 80% / Effort 2 months = 4,000
- Feature B: Reach 500 users/month × Impact 3 × Confidence 60% / Effort 0.5 months = 1,800

Feature A wins despite lower per-user impact because of reach and confidence.

RICE requires honest effort estimation. Pad by 1.5-2x for anything touching legacy systems.

### One Metric That Matters (OMTM)

Each roadmap phase should optimize for exactly one metric. This prevents initiative sprawl.

Phase examples:
- Phase 1 (Problem/Solution Fit): Validated interviews per week
- Phase 2 (Early Traction): Activation rate (users who reach "aha moment")
- Phase 3 (Growth): Weekly active users or revenue retention (NRR)
- Phase 4 (Scale): Contribution margin per customer

Everything on the roadmap should have a traceable line to the OMTM. If you can't draw that line, question whether the initiative belongs in this phase.

### Dependency Mapping

Before sequencing, map blocking relationships:

```
[Foundation work] --> [Feature A] --> [Feature B]
                  --> [Feature C]
[External API]    --> [Integration] --> [Feature D]
```

The critical path is the longest chain of dependencies. Any delay on the critical path delays the whole roadmap. Non-critical path items have "float" — they can slip without affecting the end date.

Categorize dependencies:
- Internal: Other teams, other workstreams
- External: Third-party APIs, vendor contracts, regulatory approval
- Sequential: B cannot start until A is done
- Parallel: B can start while A is in progress

### Time-Boxing into 2-Week Sprints

Sprint capacity rules of thumb:
- Subtract 20% for meetings, reviews, bugs, and unplanned work
- A 5-person team at 80% capacity = 4 effective person-weeks per sprint
- Reserve 10-15% of capacity for tech debt and infrastructure

Sprint structure:
- Sprint 1-2: Foundation, setup, critical infrastructure
- Sprint 3-6: Core feature development
- Sprint 7-8: Integration, testing, polish
- Sprint 9-10: Soft launch, feedback loop, iteration

Do not schedule to 100% capacity. Unplanned work always arrives.

### Roadmap Communication Templates

**Team View (Internal)**
```
Sprint 3 (March 10-21) | OMTM: Activation Rate
Owner: [Name]
Goal: Users complete onboarding in <5 min
Must: Onboarding flow redesign [8 points]
Must: Email verification fix [3 points]
Should: Progress indicator [5 points]
Won't: Dark mode [deferred to Q3]
Risks: Design handoff delayed — escalate by March 8
```

**Board/Investor View**
```
Q2 Milestone: 1,000 paying customers
Theme 1: Activation — reduce time-to-value from 2 days to 2 hours
Theme 2: Retention — launch customer health scoring
Theme 3: Expansion — release team tier pricing
Key bets: Enterprise pilot with [Company X] closes by May
Key risks: Hiring 2 engineers by April 1 is on the critical path
```

**Customer-Facing View**
```
In Progress: Faster onboarding (shipping this month)
Coming Soon: Team collaboration features (Q2)
Exploring: Mobile app (no commitment yet)
Recently Shipped: Bulk export, API v2, SSO
```

Never put dates on customer-facing roadmaps unless you are 90%+ confident. Use quarters or "coming soon."

---

## Example Usage

**User:** I need to roadmap the next 6 months for our B2B SaaS. We have a backlog of 23 items and no idea what to cut.

**Claude (following the skill):**

Before we touch the backlog, I need to understand the context. Let's start with Phase 1:

1. What are the 1-3 business goals that absolutely must be achieved in the next 6 months? (Examples: reach $1M ARR, launch enterprise tier, reduce churn below 3%)

2. What constraints are we working with?
   - How many engineers/designers? Full-time or split capacity?
   - Any hard deadlines (conference, contract, fundraise)?
   - Significant technical debt that limits velocity?

3. Who will see this roadmap? Just your team, or also board/investors/customers?

Share those, then paste your 23 items and we'll score and sort them together.

---

**User:** Goals: reach $500K ARR, reduce churn to under 5%. Team: 3 engineers, 1 designer. Board sees this. Here are the 23 items: [list]

**Claude:** Perfect. Let me run a first-pass MoSCoW sort based on your ARR and churn goals, then ICE-score the Should/Could items to find the hidden gems...

[Continues with structured analysis]

---

## When to Use This Skill

**Use it when:**
- You have a backlog larger than your capacity to execute
- The team is arguing about priorities without a shared framework
- You need to present a roadmap to the board, investors, or customers
- You're starting a new quarter and need to align on what gets built
- Scope creep is threatening a current delivery
- You're joining a new team and need to make sense of existing commitments

**Do not use it when:**
- You need day-to-day sprint management (use a project management tool)
- You're looking for product strategy direction (use the CEO Thinking Partner skill first)
- You don't yet know what problem you're solving (use Problem Validation first)
- Your team is fewer than 2 people — keep it in a simple doc, not a framework

**Pair it with:**
- `ceo-thinking-partner.md` — to set the strategic direction before roadmapping
- `problem-validation.md` — to validate that items on the backlog solve real problems
- `investor-prep.md` — to translate the roadmap into investor-ready milestone language
- `gtm-playbook.md` — to align the roadmap with launch and go-to-market timing

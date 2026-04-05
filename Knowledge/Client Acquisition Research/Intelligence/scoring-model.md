# Lead Scoring Model

> This model self-evolves. Weights adjust based on actual deal outcomes. Last calibrated: Not yet (no conversion data). Updated with Hormozi frameworks: 2026-04-01.

## Scoring Dimensions

### FIT SCORE (Weight: 40%)

Measures how well a company matches Veyu AI's ideal client profile.

| Criterion | 0 | 10 | 20 | 30 |
|-----------|---|----|----|-----|
| Industry match | No AI need | Some AI potential | Strong AI use cases | Perfect vertical fit |
| Company size | Too small (<5) or too large (>500) | Marginal fit | Good fit (20-200) | Sweet spot (20-100, funded startup) |
| Budget likelihood | Bootstrapped, pre-revenue | Some revenue, tight budget | Funded or profitable | Recently funded, actively spending |
| Tech alignment | No-code only, no dev team | Basic tech team | Modern stack, some AI | AI-first or AI-adjacent product |

**Max FIT score: 100** (Industry 0-30, Size 0-20, Budget 0-20, Tech 0-30)

### INTENT SCORE (Weight: 35%)

Measures signals that indicate readiness to buy AI services NOW.

| Signal | 0 | Low | Medium | High |
|--------|---|-----|--------|------|
| Recent funding | No funding known | Funded 12+ months ago | Funded 6-12 months ago | Funded in last 6 months |
| Hiring signals | No AI/tech hiring | General tech hiring | Hiring data/ML roles | Actively hiring AI/ML engineers |
| Tech changes | No visible changes | Minor updates | New product launches | Major tech overhaul or AI initiative announced |

**Scoring**: Funding (0/20/40), Hiring (0/15/30), Tech changes (0/15/30). **Max: 100**

### ACCESSIBILITY SCORE (Weight: 25%)

Measures how easy it is to reach decision-makers.

| Factor | 0 | Low | Medium | High |
|--------|---|-----|--------|------|
| Founder on LinkedIn | No LinkedIn presence | Profile exists, inactive | Active, posts occasionally | Very active, engages with content |
| Mutual connections | None | 1-2 distant | 3-5 or 1 strong | Direct connection or warm intro available |
| Geography/timezone | Asia/Pacific (hard to sync) | Europe (some overlap) | US East Coast | US West Coast or flexible |

**Scoring**: LinkedIn (0/20/40), Mutual connections (0/15/30), Geography (0/15/30). **Max: 100**

### COMPOSITE SCORE

```
COMPOSITE = (Fit × 0.40) + (Intent × 0.35) + (Access × 0.25)
```

### Tier Classification

| Tier | Score Range | Action |
|------|------------|--------|
| Tier 1 | 80-100 | Priority target — research, outreach, and LTGP:CAC analysis immediately |
| Tier 2 | 60-79 | Strong prospect — research when Tier 1 is covered |
| Tier 3 | Below 60 | Low priority — monitor for signal changes |

---

## LTGP:CAC Tracking

### Per-Deal LTGP:CAC

| Deal | Contract Value | Expected Retention | Gross Margin | LTGP | CAC | Ratio | Verdict |
|------|---------------|-------------------|-------------|------|-----|-------|---------|
| (no deals yet) | | | | | | | |

### Ratio Benchmarks (Service Business)

| Ratio | Meaning | Action |
|-------|---------|--------|
| 12:1+ | Excellent | Scale this channel/niche aggressively |
| 9:1 - 12:1 | Healthy | Meets service business minimum |
| 6:1 - 9:1 | Marginal | Investigate: can we increase LTV or reduce CAC? |
| 3:1 - 6:1 | Concerning | Re-evaluate pricing, targeting, or delivery model |
| Below 3:1 | Unsustainable | Stop pursuing this segment |

### CAC by Channel

| Channel | Avg Time Cost | Avg Tool Cost | Avg Total CAC | Deals Closed | Avg LTGP:CAC |
|---------|--------------|--------------|---------------|-------------|-------------|
| Cold email | — | — | — | 0 | — |
| LinkedIn | — | — | — | 0 | — |
| Warm intro | — | — | — | 0 | — |
| Content/inbound | — | — | — | 0 | — |
| Paid ads | — | — | — | 0 | — |

---

## Close Rate ↔ Pricing Calibration

| Period | Proposals Sent | Deals Closed | Close Rate | Pricing Signal |
|--------|---------------|-------------|------------|----------------|
| (no data yet) | | | | |

### Calibration Table

| Close Rate | What It Means | Action |
|-----------|---------------|--------|
| 80%+ | Underpriced 3-4x | Raise prices immediately — you're leaving money on table |
| 60% | Underpriced 2-3x | Raise prices. You can afford to lose some deals. |
| 40% | Underpriced 1.5-2x | Test 20-30% price increase |
| 20-30% | About right | Optimize offer, not price |
| 10-20% | Slightly over market or offer needs work | Review positioning and perceived value |
| <10% | Major problem | Fix offer/positioning, not price |

### Current Close Rate: N/A
### Current Pricing Signal: N/A (starts tracking with first proposal)

---

## Payback Period Tracking

| Deal | Setup Fee | Month 1 Payment | Total Day-1 Cash | CAC | Payback Days | Target Met? |
|------|----------|-----------------|------------------|-----|-------------|-------------|
| (no deals yet) | | | | | | |

**Target**: CAC recovered within 30 days of first payment. If setup fee + month 1 > CAC, target is met.

---

## 30-Day Cash Collected Metric

| Deal | First 30 Days Collected | Total CAC + COGS | 30-Day Cash Ratio | Healthy? |
|------|------------------------|------------------|-------------------|----------|
| (no deals yet) | | | | |

**Target**: 30-day cash ratio > 1.0x (break even within first month)

---

## Weight Evolution Log

| Date | Change | Reason | Evidence |
|------|--------|--------|----------|
| 2026-04-01 | Added LTGP:CAC, close rate calibration, payback tracking | Hormozi frameworks integration | Business fundamentals knowledge base |
| (future calibrations after deal outcomes) | | | |

## Calibration Notes

- Initial weights (40/35/25) are hypothesis-based. After 10+ deal outcomes, run calibration.
- Calibration method: compare predicted scores vs actual outcomes. Increase weight of dimensions that predicted wins. Decrease weight of dimensions that didn't differentiate winners from losers.
- If a specific criterion consistently doesn't predict conversion, consider removing or replacing it.
- Geography scoring updated to reflect US/UK focus (was India-proximity based).
- LTGP:CAC and payback period tracking added to catch economic viability issues BEFORE they become cash flow problems.

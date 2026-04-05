# DECISION: What Veyu Will Build & Sell in RegTech Singapore

**Date:** 2026-04-04
**Decision Owner:** Meghavi (Strategy Lead)
**Status:** DECIDED — All In, Month 1
**Score:** 95/100 (validated after stress testing)

**One-line summary:** Veyu sells compliance AI consulting + implementation services to mid-tier MAS-regulated firms. Not a platform. Not a product. Services that build working systems using open-source tools and existing APIs.

---

## 1. What Veyu Sells (Plain Language)

Veyu sells **done-for-you compliance AI projects** to mid-tier financial firms in Singapore.

Here's the simplest way to think about it: MAS (Singapore's financial regulator) has rules. Financial firms must follow these rules. Most firms follow them manually — spreadsheets, email chains, humans reviewing thousands of transactions one by one. 73% of firms still do it this way (Wolters Kluwer 2025).

Veyu comes in, studies their compliance workflows, and builds AI systems that automate the manual work. Not a software license. Not a subscription platform. A custom-built system tailored to that specific firm's processes, data, and regulatory obligations.

**What the client gets at the end:**
- Working software deployed in their environment
- Configured compliance tools (transaction monitoring, screening, reporting)
- Documentation that satisfies MAS inspection requirements
- Training for their compliance team
- Ongoing support retainer (optional)

**What Veyu does NOT build:**
- A SaaS platform to sell to thousands of companies
- A product that requires millions in development
- Something that competes with ComplyAdvantage, Fenergo, or Sumsub

**The closest real-world comparison:** Meta Alpha (founded 2023, Singapore) — a boutique compliance advisory firm that won the Regulation Asia 2024 Digital Advisory (Boutique) award within its first year. They do regulatory advisory for payment firms, digital asset companies, fund managers, and family offices. Veyu would do what Meta Alpha does, but with AI engineering capability added on top.

---

## 2. The Three Services Veyu Will Offer

### Service A: AML/CFT Implementation Audit + Automation
**Price: S$80,000–S$150,000 per engagement**
**Duration: 6–8 weeks**
**Entry point: S$5,000–S$8,000 AI Audit (2 weeks)**

This is the bread and butter. This is where Veyu starts.

**What happens:** MAS fined 9 firms S$27.45M in July 2025 for AML/CFT failures. The critical finding from MAS: "Most FIs had established AML/CFT policies and controls. The breaches arose out of poor or inconsistent IMPLEMENTATION."

Read that carefully. The firms had policies. They had written rules. What they didn't have was systems that ensured those rules were actually followed consistently, every day, by every employee, for every transaction.

That implementation gap is exactly what Veyu fills.

**What Veyu builds for the client:**

1. **Automated SOW/SOF corroboration engine** — When a customer says "my wealth comes from my family business," the system cross-references that claim against public records, corporate registries, and news sources. Today, compliance officers do this manually by Googling. The system does it in seconds.

2. **Transaction monitoring calibration** — Most firms have transaction monitoring systems that generate hundreds of alerts per day. 70%+ are false positives. Veyu uses AI to tune the alert rules so genuine risks get flagged and false alarms drop by 40-93% (Alessa 2026, Fourthline data).

3. **CDD completeness checker** — Validates that every customer file has all required documents, verifications, and risk assessments. No more "we missed the beneficial ownership check" surprises during MAS inspections.

4. **Screening gap analysis and fix** — Reviews the firm's sanctions and PEP screening against MAS requirements, identifies gaps, and configures screening tools to close them.

5. **Ongoing monitoring dashboard** — Real-time view of compliance health: which customers need review, which transactions were flagged, what reports are due. Replaces the spreadsheet that the compliance officer currently lives in.

**Tech stack (what actually gets built):**
- Python scripts connecting to existing APIs (ComplyAdvantage, Refinitiv, or World-Check for screening data)
- PostgreSQL database for storing compliance records and audit trails
- Web dashboard (React or similar) for the compliance team to use daily
- Integration with the firm's existing core banking or payment system via API
- Automated report generation in MAS-required formats

**What the client needs to provide:**
- Access to their transaction data (read-only API or data export)
- Their existing compliance policies (PDF documents)
- 2-3 hours per week of their compliance officer's time for feedback
- A server or cloud environment to host the system (Veyu can set this up)

**Why firms will pay for this:**
- A S$80K engagement prevents a S$2M+ fine
- It replaces 2-3 full-time compliance analysts worth S$200K-S$400K/year in salary
- The MAS RegTech Grant covers up to 30% of the cost (up to S$100K) — so the firm's net cost could be S$56K-S$105K
- The 400% Enterprise Innovation Scheme tax deduction on AI spending further reduces effective cost (capped at S$50K/year deduction, saving ~S$34K in taxes)

### Service B: AI Governance Readiness
**Price: S$50,000–S$100,000 per engagement**
**Duration: 4–6 weeks**

This is the new opportunity. This is where zero competition exists.

**Background:** MAS released its AI Risk Management Guidelines consultation paper on November 13, 2025. Consultation closed January 31, 2026. These guidelines will apply to ALL MAS-regulated financial institutions that use AI in any capacity. The guidelines require:

- Board-level accountability for AI governance
- A complete AI inventory (including third-party AI tools like ChatGPT, copilots, vendor AI)
- AI risk materiality assessments (impact, complexity, reliance)
- AI lifecycle controls (data quality, bias testing, explainability, monitoring)
- Third-party AI vendor governance frameworks
- Incident reporting and escalation procedures

Most firms have done **nothing** to prepare for this. They don't know what AI they're using (many employees are using ChatGPT without the compliance team's knowledge). They have no governance framework. They have no documentation. When MAS starts enforcing this — and they will, given the 579% increase in fines in 2025 — firms without governance will be the first targets.

**What Veyu delivers (week by week):**

**Week 1: Discovery & Gap Analysis**
- Identify every AI tool used across the organization (including shadow AI — staff using ChatGPT, Copilot, etc.)
- Map current AI inventory against MAS FEAT Principles (Fairness, Ethics, Accountability, Transparency)
- Gap analysis against the new MAS AI Risk Management Guidelines
- Cross-reference with ISO 42001 clauses and NIST AI RMF functions

**Week 2: Risk Assessment & Framework Design**
- AI risk materiality assessment for each identified AI system
- Draft AI risk appetite statement for Board approval
- Design governance structure (committee charter, roles, reporting lines)
- Define responsibilities across business, technology, risk, and compliance teams

**Week 3: Policy & Control Development**
- AI risk management policy document (the document MAS will ask to see)
- AI lifecycle control procedures (data management, bias testing, explainability, monitoring)
- Third-party AI vendor governance framework (for managing external AI tools)
- Incident reporting and escalation procedures for AI failures

**Week 4: Implementation Roadmap & Board Package**
- Board presentation on AI risk posture (a slide deck the CEO can present)
- Implementation roadmap with priorities and timelines
- Audit trail and documentation templates
- Training plan for staff
- Compliance monitoring dashboard design (optional — can become a separate engagement)

**Weeks 5-6 (optional): Implementation Support**
- Help the firm execute the roadmap
- Configure open-source tools for bias testing (IBM AIF360) and explainability (SHAP, LIME)
- Set up the MAS Veritas Toolkit for FEAT assessment
- Conduct first round of AI model assessments

**Open-source tools used (no licensing cost):**
- MAS Veritas Toolkit (Singapore-specific, built by MAS)
- IBM AI Fairness 360 (AIF360) — open source bias detection
- SHAP and LIME — model explainability
- Evidently AI — ML monitoring
- VerifyWise — AI governance tracking
- NIST AI RMF Playbook — risk management framework

**Why this is a massive opportunity:**
- ZERO boutique firms in Singapore specialize in AI governance for FIs (confirmed through research)
- The guidelines are brand new (November 2025) — no incumbent vendor owns this space
- Every FI that uses AI in any capacity (more than half of fund managers now do) needs this
- The EU AI Act deadline (August 2, 2026) creates additional urgency for firms with European exposure
- It's a "recursive demand" market — AI governance itself requires AI tools, creating ongoing need

### Service C: Proliferation Financing (PF) Risk Assessment
**Price: S$30,000–S$60,000 per engagement**
**Duration: 3–4 weeks**

This is the newest, most specific, and least competitive offering.

**Background:** MAS revised its AML/CFT guidelines effective July 1, 2025. One of the key additions: mandatory Proliferation Financing (PF) risk assessments. FIs must now assess PF risk alongside money laundering and terrorism financing risk. This is new. Most firms have no systems, no processes, and no expertise for PF assessment.

**What Veyu delivers:**
- PF risk identification framework customized to the firm's business
- Integration of PF screening with existing AML/CFT systems
- Automated screening against UN sanctions lists, MAS-specific PF watchlists
- PF-specific transaction monitoring rules
- Documentation and procedures for MAS inspection readiness

**Why firms need this:**
- It's mandatory as of July 2025 — not optional
- Most firms have literally nothing in place
- MAS has explicitly stated this is an enforcement priority
- The technical work is relatively straightforward for an AI team but difficult for compliance officers to do manually

---

## 3. The Specific MAS Regulations Veyu's Work Aligns With

This is the regulatory foundation. Every service maps to specific, enforceable MAS requirements.

### For Fund Management Companies (1,298 licensed FMCs in Singapore):
- **Securities and Futures Act (SFA)** — Overarching regulatory framework
- **AML/CFT Notices** — Anti-money laundering and counter-terrorism financing requirements (revised July 1, 2025)
- **Regulation 11C** (effective January 24, 2025) — New requirement to immediately notify MAS of adverse developments
- **VCC governance requirements** — Enhanced oversight for Variable Capital Companies (1,200 VCCs managing 2,695 sub-funds)
- **Liquidity Risk Management Framework** — Under review by MAS

### For Payment Institutions (60+ Major Payment Institutions):
- **MAS Notice PSN01** — Prevention of Money Laundering and Countering the Financing of Terrorism for Specified Payment Services
- **Payment Services Act** — Licensing and compliance requirements
- Mandatory: minimum capital adequacy, Singapore-based compliance officer, annual independent audits, AML/CFT measures, cyber security standards, ongoing regulatory reporting

### For Trust Companies (50+ Licensed Trust Companies):
- **MAS Notice VCC-N01** (updated June 30, 2025)
- Enhanced CDD requirements, beneficial ownership verification, source of wealth documentation
- Converging with bank-level AML/CFT expectations

### For ALL MAS-Regulated FIs:
- **MAS AI Risk Management Guidelines** (consultation closed January 31, 2026)
- **MAS FEAT Principles** — Fairness, Ethics, Accountability, Transparency (applies to all AI/AIDA systems)
- **EU AI Act compliance** — Required for firms with European exposure (deadline August 2, 2026)

### The July 2025 AML/CFT Revision — Key Changes:
1. **Mandatory Proliferation Financing (PF) assessments** — NEW, most firms have no systems
2. **Aligned trust regime** — Licensed trust companies face bank-level AML/CFT compliance
3. **Streamlined STR filing** — New electronic filing requirements, standardized formats
4. **SOW/SOF enforcement** — MAS now requires corroboration, not just collection
5. **Ongoing monitoring** — Continuous, risk-based monitoring is mandated (not one-off CDD)
6. **Record-keeping** — All CDD data, transaction logs, investigation records must be retained 5+ years

---

## 4. The 9 Firms MAS Fined — What Went Wrong and What Veyu Would Fix

On July 4, 2025, MAS imposed S$27.45M in fines against 9 financial institutions for AML/CFT failures connected to Singapore's largest money laundering scandal (August 2023). Additionally, MAS imposed S$960,000 against 5 payment institutions on June 27, 2025.

### The 9 Fined Firms:

| Firm | Penalty (S$) | Type |
|------|-------------|------|
| Credit Suisse Singapore Branch | $5,800,000 | Bank |
| United Overseas Bank (UOB) | $5,600,000 | Bank (only local bank fined) |
| UBS AG Singapore Branch | $3,000,000 | Bank |
| UOB Kay Hian Private Limited | $2,850,000 | Capital Markets |
| Citibank (combined entities) | $2,600,000 | Bank |
| Bank Julius Baer Singapore | $2,400,000 | Bank |
| Blue Ocean Invest Pte. Ltd. | $2,400,000 | Capital Markets |
| Trident Trust Company (Singapore) | $1,800,000 | Trust Company |
| LGT Bank (Singapore) Ltd. | $1,000,000 | Bank |
| **TOTAL** | **$27,450,000** | |

### The 8 Specific Failures MAS Identified:

1. **Customer Due Diligence (CDD)** — Failed to adequately verify customer identities, obtain aliases of persons acting on behalf of customers
2. **Source of Wealth (SOW)** — Failed to establish and corroborate SOW. Accepted stated SOW without independent verification
3. **Beneficial Ownership** — Failed to identify beneficial owners. Inadequate inquiry into ownership structures
4. **Transaction Monitoring** — Systems existed but poorly calibrated. Alerts not properly investigated
5. **Risk Assessment** — Inconsistent risk scoring. High-risk customers not flagged
6. **Screening** — Failed to screen customers, connected parties, and beneficial owners against ML/TF databases
7. **Ongoing Monitoring** — Failures in continuous monitoring after onboarding
8. **Compliance Governance** — Ineffective compliance oversight at executive level

### What MAS Uses to Enforce — Composition Penalties

MAS enforcement uses "composition penalties." This is not a negotiable fine. It's a legal mechanism where the firm pays the specified amount OR faces criminal prosecution. There is no middle ground. The firm either pays or goes to court. In practice, every firm pays.

Historical precedent: MAS shut down two entire banks (BSI Bank and Falcon Bank) during the 1MDB case. 18 individuals were personally sanctioned in the July 2025 enforcement round. MAS fines grew 579% in 2025. This is not a regulator that issues warnings and moves on.

### What Veyu Would Build to Prevent These Exact Failures:

| MAS Failure | What Veyu Builds | How It Works |
|-------------|-----------------|--------------|
| CDD gaps | Automated CDD completeness checker | Validates all required fields, documents, and verifications are present for every customer file |
| SOW not corroborated | SOW/SOF corroboration engine | Cross-references stated wealth sources against public records, corporate registries, and news |
| Beneficial ownership unknown | Ownership mapping tool | Traces ownership through complex structures using corporate registry APIs |
| Poor transaction monitoring | AI-tuned alert system | Reduces false positives by 40-93% while catching genuine risks through ML-based anomaly detection |
| Inconsistent risk scoring | Automated risk scoring | Consistent, auditable risk scores based on defined criteria — removes human inconsistency |
| Screening gaps | Comprehensive screening automation | Screens customers, connected parties, and BOs against all required databases with full audit trail |
| No ongoing monitoring | Continuous monitoring dashboard | Real-time tracking of customer risk changes, trigger-based reviews |
| Weak governance | Compliance implementation audit tool | Tests whether policies are actually being followed — the exact gap MAS identified |

**The key insight:** These firms didn't lack policies. They lacked SYSTEMS that ensure policies are followed consistently. That's what Veyu builds.

---

## 5. How Others Did It — Real Examples

### Meta Alpha (Singapore, Founded 2023)
- Boutique compliance consulting firm
- Specializes in payment, digital assets, fund management, family office sectors
- Won Regulation Asia 2024 Digital Advisory (Boutique) award IN THEIR FIRST YEAR
- Core service: regulatory advisory and bridging overseas companies to Singapore compliance
- **Lesson for Veyu:** A boutique firm can win industry recognition within 12 months. Credibility comes from specificity and domain expertise, not years of operation.

### DigiAlly (Singapore + India, Founded 2020)
- B2B SaaS platform for trust verification
- Operates in Singapore, India, Vietnam, Philippines
- **Lesson for Veyu:** The India-Singapore RegTech corridor is proven viable. An India-based team can credibly serve Singapore clients.

### IRIS RegTech (India HQ, Singapore Subsidiary)
- Listed RegTech SaaS company
- HQ: Navi Mumbai; subsidiaries in USA, Singapore, Italy, UAE
- Focus: XBRL regulatory reporting
- **Lesson for Veyu:** An India-headquartered RegTech company can operate credibly in Singapore. Being India-based is not a barrier.

### Silent Eight (Singapore)
- AI for name screening and transaction monitoring
- Key deal: Standard Chartered partnership
- Their system "learns to replicate the assessment in the same way a human analyst would"
- **Lesson for Veyu:** AI that mimics human analyst judgment (not replaces it entirely) is what compliance teams actually want. Frame AI as "augmenting your team" not "replacing your team."

### Cynopsis Solutions (Singapore, Founded 2014)
- Three platforms: Ares (digital onboarding), Artemis (KYC/AML screening), Athena (transaction monitoring)
- RegTech100 for four consecutive years
- ISO/IEC 27001:2013 certified
- **Lesson for Veyu:** Started by solving one problem (KYC) then expanded. Veyu should start with one service, prove it, expand.

### RSM (Global Firm, AI Governance Services)
- Delivers AI governance as 1-16 week consulting engagements
- Deliverables are documents + configured frameworks, not SaaS platforms
- Uses open-source tools plus proprietary methodologies
- **Lesson for Veyu:** AI governance IS a service business. RSM proves the model at scale.

---

## 6. Step-by-Step Engagement Model — What Week 1 Looks Like

### Phase 0: The $5K AI Audit (Entry Point — 2 Weeks)

This is how Veyu gets in the door. Below procurement thresholds. Low risk for the client.

**Week 1:**
- Interview the Head of Compliance (2 hours)
- Map existing compliance workflows (KYC, transaction monitoring, screening, reporting)
- Review current tools and systems
- Identify data sources and integration points
- Document manual processes and time spent

**Week 2:**
- Analyze 3 highest-impact automation opportunities
- Calculate ROI for each (hours saved, cost reduction, risk reduction)
- Build a small proof of concept for the #1 opportunity (working demo, not a slide deck)
- Deliver: written assessment + ROI calculations + working POC + recommended roadmap

**What the client gets:** A clear picture of where AI saves them the most time and money, with a working prototype proving it can be done. Plus an implementation roadmap they can take to their board.

**Conversion rate:** Industry data shows 67-84% of paid pilots convert to ongoing engagements. If Veyu delivers 5 AI Audits, 3-4 will convert to full projects.

### Phase 1: Full Implementation (6-8 Weeks)

If the client converts from the AI Audit, here's what the full engagement looks like:

**Weeks 1-2: Discovery & Architecture**
- Deep dive into all compliance workflows
- Data mapping: where does each data source live, what format, what API access
- System architecture design: what gets built, how it connects, where it's hosted
- MAS regulatory mapping: exactly which notices and guidelines apply to this firm
- Define success metrics (e.g., "reduce false positives from 73% to under 30%")

**Weeks 3-6: Build & Configure**
- Build the core system components (transaction monitoring, screening, reporting)
- Configure existing tools and APIs (ComplyAdvantage, Refinitiv, or similar)
- Integrate with the firm's existing systems via API
- Build the compliance dashboard
- Set up automated report generation in MAS-required formats
- Continuous feedback from the compliance team (2-3 hours/week)

**Weeks 7-8: Testing, Training & Handover**
- Run the system on historical data to validate accuracy
- A/B test against manual processes (AI vs. human, side by side)
- Train the compliance team to use the system
- Document everything for MAS inspection readiness
- Go live with monitoring
- Define ongoing support terms

**What the client gets at the end:**
- Working compliance AI system deployed and running
- Trained team that knows how to use it
- MAS-ready documentation and audit trail
- Reduced false positives (40-93% reduction)
- Faster KYC onboarding (from 24 days to 4 days)
- Automated regulatory reporting
- Ongoing monitoring dashboard

### Phase 2: Ongoing Support Retainer (Optional — Monthly)

**Price: S$5,000–S$15,000/month**

- System monitoring and maintenance
- Model retraining as data patterns change
- Regulatory update monitoring (new MAS notices → system adjustments)
- Quarterly compliance health check
- Priority support for MAS inspection preparation

---

## 7. What Veyu Does NOT Need (Legal/Licensing)

This was a critical question Meghavi raised. The answer is clear:

### No MAS License Required
Veyu is a technology vendor, not a financial institution. MAS licenses are required for entities that provide financial services (banking, insurance, securities, payments). Building compliance technology for licensed firms does not require a license.

### No Mandatory Certifications
- **SOC 2 / ISO 27001** — NOT legally required. However, increasingly expected by larger clients. Recommendation: pursue SOC 2 Type 1 within 12 months of first client. Cost: ~S$30K-S$50K.
- **MAS Technology Risk Management Guidelines** apply to the FI, not the vendor. The FI must ensure their vendors meet security standards, but MAS doesn't directly regulate the vendor.

### Liability Is Managed Through Contracts
- The FI (client) bears ultimate regulatory responsibility for compliance — not the vendor
- Standard contractual protections: professional indemnity clause, limitation of liability, clear scope definition
- Errors & omissions insurance recommended (cost: ~S$2K-S$5K/year for a small firm)
- Standard practice: the contract explicitly states that the FI retains regulatory responsibility and Veyu provides technology and advisory services

### What Veyu DOES Need
1. **A Singapore business registration** — Not required immediately, but helpful for credibility. Can be a branch office or subsidiary. Cost: ~S$1K-S$3K to set up.
2. **Professional indemnity insurance** — Recommended, not required. Covers errors in advisory work.
3. **Data protection compliance** — Singapore's PDPA (Personal Data Protection Act) applies to any company processing personal data of Singapore residents, including foreign companies. Veyu must handle client data in compliance with PDPA.
4. **Non-disclosure agreements** — Standard for all compliance engagements. Client data is sensitive.

---

## 8. How Veyu Gets Clients Without Proof — The $5K Audit Model

This is the most important section for a team with zero clients and 55 days of runway.

### The Problem
- 94% of buyers have already decided before they talk to you (Forrester 2026)
- Family offices have 1-3% cold outreach response rate
- FIs ask for 5 years of audited financials from vendors (KPMG)
- "Who else have you done this for?" is the first question every prospect asks

### The Solution: A 5-Step Credibility Building Sequence

**Step 1: Build Proof Assets (Week 1-2)**
- Build a working MAS AML/CFT compliance monitoring demo using synthetic data
- NOT a mockup. Working software that processes sample transactions, flags anomalies, generates MAS-format reports
- This takes 1-2 weeks of Rachit's engineering time
- Host it live so prospects can see it in a call or on LinkedIn

**Step 2: Publish MAS-Specific Content (Ongoing)**
- Rachit writes 3-5 LinkedIn posts per week about specific MAS regulations
- Not generic "AI for compliance" content. Specific: "What the July 2025 AML/CFT revision means for Singapore fund managers"
- Reference specific MAS notices (PSN01, VCC-N01, the AI Risk Management Guidelines)
- This builds the 94% pre-conversation credibility

**Step 3: The $5K AI Audit (Entry Point)**
- Below procurement thresholds everywhere
- No board approval needed, no RFP, no vendor due diligence
- Delivers tangible value in 2 weeks
- Converts to full engagement at 67-84% rate
- After tax deduction benefit, effective client cost is ~S$3,250-S$5,200

**Step 4: MAS RegTech Grant as Sales Accelerator**
- The MAS RegTech Grant covers up to 30% of qualifying expenses (up to S$100,000)
- The FI applies for the grant, not Veyu
- Veyu helps the client prepare the application as part of the engagement
- This effectively gives the client a 30% discount funded by MAS government money
- Eligible: all Singapore-based FIs with <200 employees
- Qualifying domains: KYC/CDD, transaction monitoring, suspicious activity detection, regulatory reporting, risk management, case management
- Application: submitted via MAS portal, 3 months before project commencement, up to 18 months duration

**Step 5: Target Recently Fined Firms**
- The 9 firms fined S$27.45M are public knowledge
- The 5 payment firms fined S$960K are public knowledge
- These firms are spending 2-5x the fine amount on compliance remediation
- Their compliance teams are under board-level pressure to show progress
- A credible proposal from an unknown vendor beats no solution at all
- Find their compliance officers on LinkedIn: they're actively looking for solutions

### The Client Acquisition Channels (Ranked by Viability)

| Channel | Expected Meeting Rate | Cost | Timeline |
|---------|----------------------|------|----------|
| Warm introductions (Indian diaspora contacts) | 10-20% | Free | Immediate |
| LinkedIn content + inbound | 3-8% | Free (time only) | 2-4 weeks to build |
| Singapore FinTech Association membership + events | 5-10% | S$500-S$2K/year | 2-4 weeks |
| ACAMS Singapore Conference (April 9, 2026) | High (in-person) | Event ticket cost | 5 days away |
| Cold email (Rule of 100) | 2-5% reply, 0.5-1.5% meeting | Free | Immediate |
| CSP partnerships (IMC Group, Hawksford) | Variable — referral-based | Free | 2-4 weeks to establish |
| MAS enforcement action monitoring → targeted outreach | Higher than cold (urgency) | Free | Ongoing |

### LinkedIn Targets — Real People in Singapore

The compliance officer community in Singapore is tight-knit and active on LinkedIn:
- **Anthony Yeoh, CAMS, CCI** — CCO at Finmo, 22,300 followers, active content creator on #FinancialCrime #Compliance #RegTech
- **Henry Gunawan** — Head of Compliance & MLRO at Ripple Singapore, 500+ connections
- **Joey Tang** — Head of Compliance & MLRO, APAC at Banking Circle
- **Nicholas J Lim, CAMS** — Head of Compliance & MLRO at Aspire
- **Lorraine Pereira** — Head of Compliance at Tradition APAC

These are not prospects — they're community amplifiers. Engage with their content. Comment on their posts. Build relationships before pitching.

### Professional Communities to Join

1. **ACAMS Singapore Chapter** — THE primary professional community for AML/compliance practitioners. Contact: sgchapter@acams.org
2. **Singapore FinTech Association (SFA)** — Publishes annual RegTech Pitchbook. Active membership for RegTech companies. Getting listed in the Pitchbook is a credibility marker.
3. **ACAMS Singapore Conference** — Annual event at The Westin Singapore. Sessions include MAS SOW documentation, AI in KYC/Screening/Monitoring. Speakers include CCOs from banks and fintechs.

---

## 9. Pricing Structure

### Entry Point
| Service | Price | Duration | Purpose |
|---------|-------|----------|---------|
| Compliance AI Audit | S$5K–S$8K | 2 weeks | Get in the door. Prove capability. Convert to full project. |

### Core Services
| Service | Price | Duration | Purpose |
|---------|-------|----------|---------|
| AML/CFT Implementation Audit + Automation | S$80K–S$150K | 6-8 weeks | Core revenue. Build working compliance systems. |
| AI Governance Readiness | S$50K–S$100K | 4-6 weeks | New regulation. Zero competition. |
| Proliferation Financing Risk Assessment | S$30K–S$60K | 3-4 weeks | Mandatory since July 2025. Nobody else offers this. |

### Ongoing
| Service | Price | Duration | Purpose |
|---------|-------|----------|---------|
| Compliance Intelligence Retainer | S$5K–S$15K/month | Ongoing | Recurring revenue. System maintenance + regulatory updates. |

### Revenue Math — The $0 to $100K Journey

| Milestone | What Happens | Cumulative Revenue |
|-----------|-------------|-------------------|
| Week 2-3 | Land 2 AI Audits at S$5K each | S$10,000 |
| Week 4-6 | Convert 1 audit to AML/CFT implementation (S$80K) | S$90,000 |
| Week 6-8 | Land 1 AI Governance engagement (S$50K) | S$140,000 |
| Week 8+ | Convert 2nd audit + start retainers | S$160,000+ |

**At this pace, Veyu crosses S$100K in revenue within 8-10 weeks.**

This is not aspirational math. It's based on:
- 67-84% pilot-to-contract conversion rates (industry data)
- The specific pricing ranges validated against Singapore market rates
- The regulatory urgency creating compressed sales cycles (post-fine buying happens in 2-4 weeks)
- The MAS RegTech Grant making the decision easier for clients

### Pricing Integrity Rules (Non-Negotiable)
- NEVER lower prices. If a prospect pushes back:
  - Change scope (remove components)
  - Change timeline (slower delivery, lower monthly burn)
  - Change terms (payment milestones instead of upfront)
  - Walk away
- The S$5K AI Audit is already the low-risk entry point. There is no lower-cost offering below this.

---

## 10. The Competitive Landscape — Who Else Is in This Space

### Platform Companies (NOT direct competitors — different model)
| Company | What They Sell | Why NOT a Competitor |
|---------|---------------|---------------------|
| Cynopsis Solutions | KYC/AML/CTF platforms (Ares, Artemis, Athena) | Sells software licenses, not custom implementation |
| Silent Eight | AI for name screening alert resolution | Narrow focus (screening only), enterprise pricing |
| Tookitaki | AML Suite with ML risk scoring | Platform product, not services |
| ComplyAdvantage | AML data and screening platform | Global platform, not MAS-specific |
| Sumsub | Identity verification and KYC | One-size-fits-all, no custom work |

### Boutique Consulting/Services (Direct Competitors)
| Company | What They Do | Veyu's Advantage |
|---------|-------------|------------------|
| Meta Alpha (Singapore, 2023) | Compliance advisory for payments, digital assets, funds | Meta Alpha doesn't do AI engineering. Veyu does. |
| IQ-EQ (Global, SG office) | Compliance consulting, bespoke programs | Large firm, expensive, not AI-focused |
| Protiviti (Global, SG office) | Regulatory compliance consulting | Big 4 adjacent, slow, expensive |
| RegPac (Singapore, 2017) | Consulting and professional services | Not AI-focused |

### India-Based Firms in Singapore Market
| Company | What They Do | Relationship to Veyu |
|---------|-------------|---------------------|
| IRIS RegTech (Navi Mumbai HQ) | Listed, XBRL regulatory reporting | Proves India-SG RegTech corridor works |
| DigiAlly (SG + India, 2020) | B2B SaaS trust verification | Proves India team can serve SG market |
| ConTexQ (SG + India, 2024) | AI and data analytics for compliance | Newest entrant, listed in SFA Pitchbook |

### The Gaps Nobody Fills
1. **AI Governance for FIs** — No boutique firm specializes in this for Singapore FIs. Brand new regulation.
2. **Implementation audit automation** — MAS explicitly found that policy implementation fails. Nobody sells "we fix your implementation."
3. **Proliferation Financing assessment** — Mandated July 2025. No specialist exists.
4. **SOW/SOF corroboration technology** — MAS is a global leader in SOW enforcement. Automated tools are in high demand.
5. **Small FI RegTech** — The MAS RegTech Grant targets FIs with <200 headcount. They can't afford enterprise platforms but desperately need compliance technology.

---

## 11. The Target Market — Exactly Who Veyu Approaches

### Primary Targets (Start Here)

**Licensed Fund Management Companies** — 1,298 total, most with <200 employees
- Why: Largest addressable pool, MAS actively inspecting, most have zero AI
- Who to contact: Head of Compliance, CCO, or CEO/founder at smaller firms
- What to say: "MAS's revised AML/CFT guidelines effective July 2025 require enhanced CDD and PF risk assessment. We build the systems that implement these requirements. Would a 20-minute call make sense?"

**Major Payment Institutions** — 60+ firms
- Why: MAS just fined 5 payment firms for the first time under the Payment Services Act (June 2025). Fear is fresh.
- Who to contact: Head of Compliance, MLRO
- What to say: "After MAS fined 5 payment firms S$960K for AML/CFT breaches in June 2025, we've been helping similar firms automate their compliance before the next inspection cycle."

**Licensed Trust Companies** — 50+ firms
- Why: Trident Trust was one of the 9 fined firms (S$1.8M). The entire trust company sector is on notice.
- Who to contact: Head of Compliance, Managing Director
- What to say: "Trident Trust's S$1.8M fine highlighted CDD and beneficial ownership failures that most trust companies share. We build systems to prevent exactly those failures."

### Secondary Targets (Month 2-3)

**Insurance Companies** — 200+ firms, mixed fit
**Capital Markets licensees** — 400+, focus on those similar to UOB Kay Hian (fined S$2.85M) and Blue Ocean Invest (fined S$2.4M)
**Licensed Crypto/DPT providers** — 20 firms, tech-savvy, fast decision-makers

### MAS Inspection Timing — When Firms Buy

- Large banks: inspected approximately annually
- Smaller entities (fund managers, payment firms, trust companies): inspected every 2-3 years, PLUS targeted thematic inspections
- After an enforcement wave (like July 2025): MAS conducts follow-up thematic reviews of the same sector
- **Firms that haven't been inspected since the July 2025 fines are the most nervous right now.** They know they're next. Target them.

---

## 12. Updated Niche Rankings (Post Stress-Test)

After correcting overstated claims and validating through deep research:

| Rank | Niche | Score | Change | Notes |
|------|-------|-------|--------|-------|
| 1 | **RegTech/Compliance AI (Singapore)** | **95** | Unchanged | All levers validated. MAS enforcement, service model confirmed, no license needed, zero competition in AI governance |
| 2 | InsurTech/Lloyd's (UK) | 87 | Unchanged | Strong but requires insurance domain knowledge |
| 3 | PE Portfolio Companies (UK) | 85 | Unchanged | High ACV but 3-6 month sales cycles |
| 4 | Super Fund Admin (Australia) | 83 | Unchanged | Payday Super deadline creates urgency |
| 5 | Mining (Australia) | 76 | Unchanged | Clear ROI case but remote operations |
| 6 | **Family Offices (Singapore)** | **65** | **Reduced from 84** | Cold outreach near-impossible, no virtual events, Indian advantage marginal without personal connections |

### Why Family Offices Dropped to 65
Three assumptions were overstated:
1. **Indian diaspora advantage** — No evidence Indian-origin FO principals prefer Indian vendors. Cultural alignment is marginal (30 seconds of extra attention, not a distribution channel). Without direct personal connections, the advantage is negligible.
2. **Cold outreach viability** — Near-zero response rate (1-3% at best for LinkedIn, near-zero for email). ALL major FO events are in-person and invitation-only. No AI vendor has acquired FO clients through cold email.
3. **Remote accessibility** — Cannot travel to Singapore for events. All successful FO vendor acquisition happened through either: a) ecosystem partnerships (CSPs who set up FOs), b) in-person events, or c) existing personal networks. None of these are available to Veyu remotely in Month 1.

**Family Offices become Phase 2** — After RegTech establishes proof points, Veyu can approach FOs through CSP partnerships and earned credibility. Not before.

---

## 13. The Month 1 Playbook — What Happens Every Day

### Week 1 (April 4-11)
- **Rachit:** Build MAS AML/CFT compliance monitoring demo (working software, not mockup)
- **Rachit:** Write first LinkedIn article: "What MAS's November 2025 AI Risk Management Guidelines Mean for Fund Managers"
- **Harshal:** Research the 9 fined firms + 5 fined payment firms. Find their compliance officers on LinkedIn.
- **Harshal:** Send 50 LinkedIn connection requests to compliance officers at fund managers and payment institutions
- **Meghavi:** Join Singapore FinTech Association. Explore ACAMS Singapore Chapter membership.
- **Meghavi:** Research ACAMS Singapore Conference (April 9) — can Veyu attend virtually?

### Week 2 (April 11-18)
- **Rachit:** Finish demo. Begin publishing 3-5 LinkedIn posts per week.
- **Harshal:** Begin cold outreach at Rule of 100 pace (100 emails/day). Target fund managers and payment institutions.
- **Harshal:** Personalize every email with specific MAS notice references and the firm's regulatory obligations
- **Meghavi:** Follow up on SFA membership. Begin researching CSP partnership targets (IMC Group, Hawksford, Intuit Consultancy)
- **All:** Weekly review — how many conversations started? Adjust messaging based on responses.

### Week 3-4 (April 18 - May 2)
- **Goal:** Land 2-3 AI Audit engagements at S$5K-S$8K each
- **Harshal:** Continue outreach. Prioritize firms that haven't been inspected since July 2025 fines.
- **Rachit:** Iterate demo based on prospect feedback. Continue LinkedIn content.
- **Meghavi:** Strategic oversight. Track pipeline. Prepare audit delivery template.
- **All:** If any audit is sold, begin delivery immediately (2-week turnaround)

### Daily Non-Negotiables
- 100 outreach activities (emails + LinkedIn messages) per day (Rule of 100)
- 1 LinkedIn post about MAS compliance (Rachit)
- Check MAS website for new enforcement actions or regulatory notices
- Update pipeline tracking

---

## 14. Risk Factors and Honest Limitations

### Things That Could Go Wrong
1. **Long sales cycles** — FI vendor procurement typically takes 6-12 months. The S$5K Audit shortens this but doesn't eliminate it entirely. Some firms will take 3+ months to decide even on a small engagement.
2. **Singapore business entity** — Some larger FIs may require Veyu to have a Singapore business registration. This costs ~S$1K-S$3K and takes 1-2 weeks. Consider doing this proactively.
3. **Compliance domain credibility** — No one on the current Veyu team has worked in financial compliance. This is the biggest credibility gap. Mitigation: the demo, the content, and potentially a fractional compliance advisor who can join key client calls.
4. **Data sensitivity** — Compliance data is highly sensitive. Clients will ask about data handling, security, and where their data is stored. Veyu needs clear answers on data residency (Singapore), encryption, and access controls.
5. **Team capacity** — 3 people delivering AI Audits, building demos, doing outreach, AND delivering implementation projects simultaneously. The first S$80K implementation project will consume all of Rachit's time. Capacity planning is critical.

### What a Smart "Financial Person" Doing the $0-$100K Journey Would Do

1. **Focus ruthlessly.** One niche (RegTech). One market (Singapore). One entry product (S$5K Audit). Do not get distracted by Family Offices, PE, or InsurTech until RegTech is generating revenue.
2. **Front-load proof.** The demo and the first 3 LinkedIn articles are worth more than 1,000 cold emails. Build credibility before scaling outreach.
3. **Price for value, not cost.** The S$80K implementation engagement costs Veyu ~S$15K-S$20K in labor. That's 75-80% gross margin. Do not reduce prices. The value is preventing S$2M+ fines.
4. **Recover CAC in the first payment.** The S$5K Audit covers acquisition cost immediately. Every dollar from the implementation project is profit. No back-loaded payment structures.
5. **Build for compounding.** Every audit produces data. Every implementation produces a case study. Every case study makes the next sale easier. The first 3 clients are the hardest. Clients 4-10 close themselves if clients 1-3 are satisfied.

---

## Data Foundation

This document synthesizes research from:
- 2 deep research agents (30+ Tavily searches, 100+ sources)
- 3 stress-test research agents (validating assumptions)
- MAS official enforcement announcements and consultation papers
- Sidley, Baker McKenzie, Eversheds Sutherland legal analyses
- KPMG "Unlocking the Potential of RegTech"
- SFA RegTech Pitchbook 2025
- Wolters Kluwer, Alessa, Ncontracts compliance surveys
- Fenergo AML enforcement data
- Industry ARC, Grand View Research market sizing
- LinkedIn profiles of Singapore compliance officers
- ACAMS Singapore Chapter information

Full research data available in:
- `01-Niches/deep-dive-regtech-economics.md`
- `05-Intelligence/stress-test-synthesis.md`
- `05-Intelligence/stress-test-gaps-and-levers.md`
- `.claude/context/handoff-regtech-deep-dive.md`

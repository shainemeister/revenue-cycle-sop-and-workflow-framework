# Revenue Cycle SOP & Workflow Framework - Plan

**Version**: 1.7  
**Last Updated**: May 14, 2026  
**Owner**: Shaine Meister

## Project Goals

The primary objectives of this framework are to:

- Establish a reusable, modular system for revenue cycle SOPs and workflows.
- Create portable intellectual property that can be adapted across different organizations and systems.
- Maintain strong alignment with industry standards and regulatory requirements.
- Support ongoing process optimization and continuous improvement with a strong focus on usability and reduced mental friction.
- **New in v2**: Enable autonomous feedback loops and structured data collection for future RCM system integration and contract intelligence.

## 3×3 Matrix v2 Vision (Core Concept)

The framework is built around a **3×3 Revenue Cycle Matrix** that organizes all SOPs and Workflows into three categories with exactly three items each (Rule of 3 for low mental load):

**Category 1 – Front-End**
1. Patient Intake
2. Scheduling
3. Registration

**Category 2 – Provider**
1. Service
2. Diagnosis / Notation (Charting)
3. Coding

**Category 3 – Back-End**
1. Billing (including patient billing)
2. Follow-up (Insurance AR + Denials)
3. Payment Posting / Collections

**Key v2 Enhancement**: A **Cross-Cutting Feedback Loop Orchestration Layer** that makes the matrix self-improving.

### Feedback Loop Orchestration Layer (`feedback-loop-framework.md`)

This new top-level document defines the standardized interface for autonomous feedback. It has three core responsibilities:

**A. Standardized Feedback Data Capture**  
Every SOP (especially the critical Registration → Provider Service → Notation/Charting → Coding chain) includes a dedicated `## Feedback Loop & Data Collection Framework` section at the bottom. This section is **completely separate** from operational steps and serves as the mapping layer for future RCM platforms.

**B. Closed-Loop Handoff Protocol** (Critical Chain)

- **Registration** captures insurance, demographics, and authorization data → sends structured summary to Provider Service.
- **Provider Service** captures encounter details and clinical notes → sends to Notation/Charting with required elements checklist.
- **Notation/Charting** enforces documentation completeness → sends structured data package to Coding.
- **Coding** validates against documentation and payer rules → sends discrepancy report + denial pattern data back to Notation + Registration (and ultimately to Contract Intelligence).

**C. Contract Intelligence Module** (New Model Pair)

A dedicated SOP + Workflow pair (`feedback-loop-contract-intelligence.md` + workflow) that aggregates data from the entire matrix and produces clean, actionable reports for legal/contract teams. Key data points include:

- Payer-specific denial rates and CARC/RARC codes by contract
- Reimbursement rate variances vs. contracted terms
- Documentation/coding patterns that trigger downcoding or bundling denials
- Timely filing and authorization failures linked to contract language
- High-volume services with poor payment performance

This turns every denial and payment into **contract negotiation intelligence**.

**3×3 Matrix Overview Diagram**  
A single Mermaid diagram (to be maintained in `structure-enhancement-implementation-guide.md` or a dedicated overview file) showing the full 3×3 grid with **bidirectional feedback arrows** looping from Back-End back to Front-End and Mid-Cycle.

## Development Roadmap

```yaml
phases:
  - phase: 1
    name: Foundation & Core Framework
    focus:
      - Define core principles and philosophy
      - Establish modular structure and regulatory foundations
      - Create optimization standards
      - Build reusable templates
    status: Complete
    completed: May 2026
    target: Q2 2026

  - phase: 2
    name: Initial SOP & Workflow Development
    focus:
      - Develop foundational SOPs for key revenue cycle areas (Registration, Visit Filing Order, Demand Claim as model pairs)
      - Create supporting companion workflows
      - Test and refine templates in real use
    status: In Progress
    target: Q2 - Q3 2026

  - phase: 3
    name: Structure Enhancement & Feedback Layer Rollout (v2)
    focus:
      - Introduce modern YAML front matter
      - Add completely separate Feedback Loop & Data Collection Framework section to every SOP and Workflow
      - Create `feedback-loop-framework.md` (governing document)
      - Create Contract Intelligence model pair
      - Migrate all existing model pairs to v2
      - Update 3×3 Matrix Overview with bidirectional feedback arrows
    status: In Progress
    target: May - June 2026

  - phase: 4
    name: Expansion & Optimization
    focus:
      - Expand into Billing, Denials, Appeals, Prior Auth, Coding, Patient Financial Services, etc.
      - Refine optimization and continuous improvement
      - Develop adoption guides
    status: Future
    target: Q3 2026 onward
```

## Current Status

**Overall Status**: In Development — Foundational framework complete. Three model pairs (Registration, Visit Filing Order, Demand Claim) developed. **Phase 3 (v2) now active** — introducing YAML front matter, standalone Feedback Loop sections, and the Feedback Layer Orchestration Layer.

### Framework Documents

| Document                                      | Status     | Version | Notes / Priority                                      |
|-----------------------------------------------|------------|---------|-------------------------------------------------------|
| core-principles.md                            | Complete   | 1.0     | Strong philosophical foundation                       |
| modular-structure.md                          | Complete   | 1.0     | Excellent modularity and pairing guidance             |
| regulatory-foundations.md                     | Complete   | 1.0     | Well-balanced, risk-based integration                 |
| optimization-standards.md                     | Complete   | 1.0     | Practical focus on mental friction & flow             |
| structure-enhancement-implementation-guide.md | Active     | 1.0     | Authoritative v2 rollout guide (new May 2026)         |
| feedback-loop-framework.md                    | Planned    | 1.0     | **High Priority** – Governing document for data standards, JSON schemas, handoff protocols, and contract intelligence mapping |

### Templates (v2 – In Progress)

| Template                  | Status          | Notes                                                                 |
|---------------------------|-----------------|-----------------------------------------------------------------------|
| sop-template.md           | Needs Update    | Must add YAML front matter + standalone `## Feedback Loop & Data Collection Framework` section at bottom |
| workflow-template.md      | Needs Update    | Must add YAML front matter + standalone `## Feedback Loop & Data Collection Framework` section at bottom |

### SOPs (Planned / In Development) – 3×3 Matrix v2

| SOP                                      | Status          | Priority | Category     | Matrix Pos | Notes / v2 Migration Required                                      |
|------------------------------------------|-----------------|----------|--------------|------------|--------------------------------------------------------------------|
| front-end-patient-intake.md              | Planned         | Medium   | Front-End    | 1.1        | New – to follow v2 template                                        |
| front-end-scheduling.md                  | Planned         | Medium   | Front-End    | 1.2        | New – to follow v2 template                                        |
| registration.md                          | Complete        | High     | Front-End    | 1.3        | **Model** – Migrate to v2 (add YAML + Feedback section)            |
| provider-service.md                      | Planned         | High     | Provider     | 2.1        | New – Critical for closed-loop handoff                             |
| provider-diagnosis-notation.md           | Planned         | High     | Provider     | 2.2        | New – Critical for closed-loop handoff                             |
| provider-coding.md                       | Planned         | High     | Provider     | 2.3        | New – Critical for closed-loop handoff                             |
| back-end-billing.md                      | Planned         | High     | Back-End     | 3.1        | New – Includes patient billing                                     |
| back-end-insurance-denial-follow-up.md   | Planned         | High     | Back-End     | 3.2        | New – Aligns with Contract Intelligence module                     |
| back-end-payment-posting-collections.md  | Planned         | Medium   | Back-End     | 3.3        | New                                                            |
| feedback-loop-contract-intelligence.md   | Planned         | **Critical** | Cross-Cutting | 0.0      | **New Model Pair** – Aggregates data for legal/contract teams      |

### Workflows (Planned / In Development) – 3×3 Matrix v2

| Workflow                                      | Status          | Priority | Category     | Matrix Pos | Notes / v2 Migration Required                                      |
|-----------------------------------------------|-----------------|----------|--------------|------------|--------------------------------------------------------------------|
| front-end-patient-intake-workflow.md          | Planned         | Medium   | Front-End    | 1.1        | New – Mermaid decision trees                                       |
| front-end-scheduling-workflow.md              | Planned         | Medium   | Front-End    | 1.2        | New                                                            |
| registration-workflow.md                      | Complete        | High     | Front-End    | 1.3        | **Model** – Migrate to v2                                          |
| provider-service-workflow.md                  | Planned         | High     | Provider     | 2.1        | New – Must show closed-loop handoffs                               |
| provider-diagnosis-notation-workflow.md       | Planned         | High     | Provider     | 2.2        | New                                                            |
| provider-coding-workflow.md                   | Planned         | High     | Provider     | 2.3        | New                                                            |
| back-end-billing-workflow.md                  | Planned         | High     | Back-End     | 3.1        | New                                                            |
| back-end-insurance-denial-follow-up-workflow.md | Planned       | High     | Back-End     | 3.2        | New                                                            |
| back-end-payment-posting-collections-workflow.md | Planned      | Medium   | Back-End     | 3.3        | New                                                            |
| feedback-loop-contract-intelligence-workflow.md | Planned       | **Critical** | Cross-Cutting | 0.0      | **New** – Visual contract intelligence reports                     |

> **Note**: All new SOPs and Workflows created after May 14, 2026 must use the v2 template (YAML front matter + standalone Feedback Loop section). Existing model pairs (Registration, Visit Filing Order, Demand Claim) will be migrated as part of Phase 3.

## Phase 3: Structure Enhancement & Feedback Layer Rollout (v2) – Detailed Implementation Plan

This phase directly addresses the #1 revenue cycle failure point (lack of autonomous feedback from Registration → Notation → Coding) and prepares the framework for future RCM system integration and contract optimization.

### Step-by-Step Process

1. **Finalize v2 Structure & Documentation** (Completed)
   - Created `structure-enhancement-implementation-guide.md` (authoritative reference)
   - Updated this `plan.md` to v1.7 with full 3×3 Matrix v2 vision, tables, and Closed-Loop Handoff Protocol

2. **Update Core Templates to v2 Format**
   - Add modern YAML front matter to `sop-template.md` and `workflow-template.md`
   - Add the standalone `## Feedback Loop & Data Collection Framework` section at the very bottom of both templates (completely separate from operational content)

3. **Migrate Existing Model Pairs to v2**
   - Apply v2 structure to: `registration.md`, `registration-workflow.md`, `visit-filing-order.md`, `visit-filing-order-workflow.md`, `demand-claim.md`, `demand-claim-workflow.md`
   - Preserve 100% of original operational content
   - Add YAML metadata + Feedback Loop section with initial data capture points

4. **Create Feedback Layer Governing Document**
   - Develop `feedback-loop-framework.md`
   - Define standardized data fields, JSON schemas, handoff triggers, and contract intelligence mapping
   - Include the Closed-Loop Handoff Protocol for the critical four processes

5. **Create Contract Intelligence Model Pair**
   - Create `feedback-loop-contract-intelligence.md` + companion workflow
   - Focus on aggregating denial, payment variance, and documentation pattern data for legal/contract teams

6. **Update 3×3 Matrix Overview Diagram**
   - Create or update the master Mermaid diagram showing the full 3×3 grid with bidirectional feedback arrows
   - Reference it from `structure-enhancement-implementation-guide.md` and this plan

7. **Team Onboarding & Validation**
   - Brief team on v2 structure, purpose of Feedback Layer, and how to maintain separation between operational content and data collection sections
   - Review all migrated files for consistency

**Target Completion for Phase 3**: End of May 2026

## Next Priorities

### Immediate (Next 7 Days)
- Complete Steps 2–4 above (templates + migration of 6 model files + `feedback-loop-framework.md`)
- Create the Contract Intelligence model pair

### Short-Term (Q2 2026)
- Update the 3×3 Matrix Overview diagram with bidirectional feedback arrows
- Begin real-world testing of v2 files
- Gather feedback on the new Feedback Loop sections

### Longer-Term (Q3 2026+)
- Expand to remaining 3×3 cells (Patient Intake, Scheduling, Billing, Payment Posting, etc.)
- Develop adoption guide for new organizations

## Metrics, Review Cadence & Continuous Improvement

This framework prioritizes **lightweight, actionable measurement** that supports improvement without adding mental friction.

### Recommended Approach
- Per SOP/Workflow: Task completion time, error/rework rate, exception frequency, user-reported mental friction (1–5 scale)
- Framework Level: Number of SOPs created, adoption, reduction in process variation
- Feedback Mechanisms: Built-in “Friction / Improvement Notes” section + trigger-based reviews

### Review Cadence
- Framework documents & templates: Quarterly or on major change
- Individual SOPs: 30–60 days after use, then annually
- Workflows: More frequent informal review

## Open Items & Notes

- Visual workflow standards (Mermaid depth, styling)
- Lightweight metrics that fit naturally into daily work
- Guidance for high-variability / payer-specific processes
- Glossary of key revenue cycle terms
- **Phase 3 v2 items**: Templates update, 6 model pair migrations, `feedback-loop-framework.md`, Contract Intelligence pair, 3×3 Matrix Overview diagram with feedback arrows

## Version History

| Version | Date          | Changes                                                                 | Author          |
|---------|---------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 2026      | Initial plan created                                                    | Shaine Meister  |
| 1.1–1.5 | May 6–9, 2026 | Multiple refinements to model pairs and priorities                      | Shaine Meister  |
| 1.6     | May 14, 2026  | Added Phase 3 v2 with 7-step plan and created `structure-enhancement-implementation-guide.md` | Shaine Meister  |
| 1.7     | May 14, 2026  | **Major expansion**: Added full 3×3 Matrix v2 vision, Feedback Loop Orchestration Layer, Closed-Loop Handoff Protocol, Contract Intelligence Module, detailed tables for all SOPs/Workflows, and comprehensive Phase 3 implementation plan. This version serves as the single source of truth for the entire v2 initiative. | Shaine Meister  |

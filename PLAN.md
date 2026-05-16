---
title: "Revenue Cycle SOP & Workflow Framework - Master Plan"
short_title: "PLAN"
version: "2.0"
last_updated: "2026-05-16"
owner: "Shaine Meister"
status: "Active"
current_phase: 3
phase_focus: "Structure Enhancement & Feedback Layer Rollout (v2)"
tags:
  - planning
  - roadmap
  - v2
  - governance
---

# Revenue Cycle SOP & Workflow Framework - Master Plan

**Version**: 2.0  
**Last Updated**: 2026-05-16  
**Owner**: Shaine Meister

> **v2.0 Update**: Refactored for improved chronological flow and v2 YAML front matter while preserving full original context and detail. Single source of truth maintained — no separate phase files.

---

## Executive Summary & Current Status

**Overall Status**: In Development — Foundational framework complete. Three model pairs (Registration, Visit Filing Order, Demand Claim) developed. **Phase 3 (v2) now active** — introducing YAML front matter, standalone Feedback Loop sections, and the Feedback Layer Orchestration Layer.

This is the single authoritative master plan for the Revenue Cycle SOP & Workflow Framework. All planning content lives here.

---

## Project Goals

The primary objectives of this framework are to:

- Establish a reusable, modular system for revenue cycle SOPs and workflows.
- Create portable intellectual property that can be adapted across different organizations and systems.
- Maintain strong alignment with industry standards and regulatory requirements.
- Support ongoing process optimization and continuous improvement with a strong focus on usability and reduced mental friction.
- **New in v2**: Enable autonomous feedback loops and structured data collection for future RCM system integration and contract intelligence.

---

## Development Timeline

The framework follows a deliberate phased approach.

```yaml
phases:
  - phase: 1
    name: Foundation & Core Framework
    status: Complete
    completed: May 2026
    focus:
      - Define core principles and philosophy
      - Establish modular structure and regulatory foundations
      - Create optimization standards
      - Build reusable templates
  - phase: 2
    name: Initial SOP & Workflow Development
    status: Complete
    completed: May 2026
    focus:
      - Foundational model pairs (Registration, Visit Filing Order, Demand Claim)
      - Companion workflows
  - phase: 3
    name: Structure Enhancement & Feedback Layer Rollout (v2)
    status: Active
    target: May - June 2026
    focus:
      - YAML front matter + standalone Feedback Loop sections
      - feedback-loop-framework.md
      - Contract Intelligence model pair
      - Migrate model pairs to v2 + enhance with examples/pitfalls
      - Standardized Mermaid visualizations
  - phase: 4
    name: Expansion & Optimization
    status: Future
    target: Q3 2026 onward
    focus:
      - Expand to remaining 3×3 areas
      - Tactical adoption resources
      - Payer-variability guidance
      - Contributor onboarding
```

**Chronological Narrative**: Phase 1 built the foundation. Phase 2 delivered initial model pairs. Phase 3 focuses on making the system self-improving through structured feedback.

---

## 3×3 Matrix v2 Vision (Core Concept)

The framework is built around a **3×3 Revenue Cycle Matrix** that organizes all SOPs and Workflows into three categories with exactly three items each (Rule of 3 for low mental load).

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

### Feedback Loop Orchestration Layer

This defines the standardized interface for autonomous feedback with three core responsibilities:

**A. Standardized Feedback Data Capture**  
Every SOP includes a dedicated `## Feedback Loop & Data Collection Framework` section (completely separate from operational steps).

**B. Closed-Loop Handoff Protocol** (Critical Chain)
- Registration → Provider Service
- Provider Service → Notation/Charting
- Notation/Charting → Coding
- Coding → back to Notation + Registration + Contract Intelligence

**C. Contract Intelligence Module**
A dedicated SOP + Workflow pair that turns operational data (denials, variances, patterns) into actionable intelligence for legal/contract teams.

**3×3 Matrix Overview Diagram**  
Maintained in `structure-enhancement-implementation-guide.md` showing the full grid with bidirectional feedback arrows.

---

## Current Status

### Framework Documents

| Document | Status | Version | Notes / Priority |
|----------|--------|---------|------------------|
| core-principles.md | Complete | 1.0 | Strong philosophical foundation |
| modular-structure.md | Complete | 1.0 | Excellent modularity and pairing guidance |
| regulatory-foundations.md | Complete | 1.0 | Well-balanced, risk-based integration |
| optimization-standards.md | Complete | 1.0 | Practical focus on mental friction & flow |
| structure-enhancement-implementation-guide.md | Active | 1.0 | Authoritative v2 rollout guide (new May 2026) |
| feedback-loop-framework.md | Planned | 1.0 | **High Priority** – Governing document for data standards, JSON schemas, handoff protocols, and contract intelligence mapping |

### Templates (v2 – In Progress)

| Template | Status | Notes |
|----------|--------|-------|
| sop-template.md | Needs Update | Must add YAML front matter + standalone Feedback Loop section |
| workflow-template.md | Needs Update | Must add YAML front matter + standalone Feedback Loop section |

### SOPs (Planned / In Development) – 3×3 Matrix v2

| SOP | Status | Priority | Category | Matrix Pos | Notes / v2 Migration Required |
|-----|--------|----------|----------|------------|-------------------------------|
| front-end-patient-intake.md | Planned | Medium | Front-End | 1.1 | New – to follow v2 template |
| front-end-scheduling.md | Planned | Medium | Front-End | 1.2 | New – to follow v2 template |
| registration.md | Complete | High | Front-End | 1.3 | **Model** – Migrate to v2 + enhance with real-world examples, exception tables, pitfalls (priority #1) |
| provider-service.md | Planned | High | Provider | 2.1 | New – Critical for closed-loop handoff |
| provider-diagnosis-notation.md | Planned | High | Provider | 2.2 | New – Critical for closed-loop handoff |
| provider-coding.md | Planned | High | Provider | 2.3 | New – Critical for closed-loop handoff |
| back-end-billing.md | Planned | High | Back-End | 3.1 | New – Includes patient billing |
| back-end-insurance-denial-follow-up.md | Planned | High | Back-End | 3.2 | New – Aligns with Contract Intelligence module |
| back-end-payment-posting-collections.md | Planned | Medium | Back-End | 3.3 | New |
| feedback-loop-contract-intelligence.md | Planned | **Critical** | Cross-Cutting | 0.0 | **New Model Pair** – Aggregates data for legal/contract teams |

### Workflows (Planned / In Development) – 3×3 Matrix v2

| Workflow | Status | Priority | Category | Matrix Pos | Notes / v2 Migration Required |
|----------|--------|----------|----------|------------|-------------------------------|
| front-end-patient-intake-workflow.md | Planned | Medium | Front-End | 1.1 | New – Mermaid decision trees |
| front-end-scheduling-workflow.md | Planned | Medium | Front-End | 1.2 | New |
| registration-workflow.md | Complete | High | Front-End | 1.3 | **Model** – Migrate to v2 + apply standardized Mermaid styling (priority #2) |
| provider-service-workflow.md | Planned | High | Provider | 2.1 | New – Must show closed-loop handoffs |
| provider-diagnosis-notation-workflow.md | Planned | High | Provider | 2.2 | New |
| provider-coding-workflow.md | Planned | High | Provider | 2.3 | New |
| back-end-billing-workflow.md | Planned | High | Back-End | 3.1 | New |
| back-end-insurance-denial-follow-up-workflow.md | Planned | High | Back-End | 3.2 | New |
| back-end-payment-posting-collections-workflow.md | Planned | Medium | Back-End | 3.3 | New |
| feedback-loop-contract-intelligence-workflow.md | Planned | **Critical** | Cross-Cutting | 0.0 | **New** – Visual contract intelligence reports |

> **Note**: All new SOPs and Workflows created after May 14, 2026 must use the v2 template. Existing model pairs will be migrated as part of Phase 3 **and enhanced with real-world examples, exception handling tables, and "common pitfalls" callouts**.

---

## Phase 3: Structure Enhancement & Feedback Layer Rollout (v2) – Detailed Implementation Plan

This phase directly addresses the #1 revenue cycle failure point (lack of autonomous feedback from Registration → Notation → Coding) and prepares the framework for future RCM system integration and contract optimization.

### Step-by-Step Process

1. **Finalize v2 Structure & Documentation** (Completed)
   - Created `structure-enhancement-implementation-guide.md`
   - Updated plan to include full 3×3 Matrix v2 vision, tables, and Closed-Loop Handoff Protocol

2. **Update Core Templates to v2 Format**
   - Add modern YAML front matter to `sop-template.md` and `workflow-template.md`
   - Add the standalone `## Feedback Loop & Data Collection Framework` section at the very bottom of both templates

3. **Migrate Existing Model Pairs to v2**
   - Apply v2 structure to registration, visit-filing-order, and demand-claim pairs
   - Preserve 100% of original operational content
   - Add YAML metadata + Feedback Loop section with initial data capture points

4. **Create Feedback Layer Governing Document**
   - Develop `feedback-loop-framework.md`
   - Define standardized data fields, JSON schemas, handoff triggers, and contract intelligence mapping

5. **Create Contract Intelligence Model Pair**
   - Create `feedback-loop-contract-intelligence.md` + companion workflow

6. **Update 3×3 Matrix Overview Diagram**
   - Create master Mermaid diagram with bidirectional feedback arrows

7. **Team Onboarding & Validation**
   - Brief team on v2 structure and Feedback Layer purpose

**Target Completion for Phase 3**: End of May 2026

---

## Next Priorities

### Immediate (Next 7 Days) — Enhancement Priorities #1–2 (v1.8)
- **#1 Enhance model SOP content depth**: Add real-world examples, exception handling tables, and "common pitfalls" callouts during v2 migration
- **#2 Standardize Mermaid visualizations**: Define consistent styling in workflow-template.md
- Complete template updates + model pair migrations + `feedback-loop-framework.md`
- Create the Contract Intelligence model pair

### Short-Term (Q2 2026) — Enhancement Priorities #3–5 + Phase 3 wrap
- Update 3×3 Matrix Overview diagram with bidirectional feedback arrows
- Begin real-world testing of v2 files
- **#3 Create tactical adoption resources**: Pilot Checklist + Adoption Guide
- **#4 Provide modular guidance for variability**: Payer-Specific Variation templates
- **#5 Strengthen contributor onboarding**: Add subsection to README

### Longer-Term (Q3 2026+)
- Expand to remaining 3×3 cells

---

## Metrics, Review Cadence & Continuous Improvement

Lightweight, actionable measurement:
- Per SOP/Workflow: task completion time, error/rework rate, exception frequency, user-reported mental friction (1–5 scale)
- Review cadence: Framework documents quarterly; Individual SOPs 30–60 days after use

---

## Open Items & Notes

### Enhancement Backlog (v1.8 — Prioritized)

1. **Enhance model SOP content depth** (High priority) — Add examples, exception tables, pitfalls
2. **Standardize Mermaid visualizations** (High priority)
3. **Create tactical adoption resources** (Medium)
4. **Provide modular guidance for variability** (Medium)
5. **Strengthen contributor onboarding** (Medium)

**Remaining open items**:
- Lightweight metrics
- Glossary of key revenue cycle terms
- Phase 3 v2 items still active

---

## Version History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | May 2026 | Initial plan created | Shaine Meister |
| 1.1–1.5 | May 6–9, 2026 | Multiple refinements to model pairs and priorities | Shaine Meister |
| 1.6 | May 14, 2026 | Added Phase 3 v2 with 7-step plan and created structure-enhancement-implementation-guide.md | Shaine Meister |
| 1.7 | May 14, 2026 | Major expansion: full 3×3 Matrix v2 vision, Feedback Loop Orchestration Layer, Closed-Loop Handoff Protocol, Contract Intelligence Module, detailed tables, comprehensive Phase 3 plan | Shaine Meister |
| 1.8 | May 14, 2026 | Integrated 5 recommended enhancements from repo review into plan | Shaine Meister |
| **2.0** | 2026-05-16 | Refactored with v2 YAML front matter and improved chronological structure while preserving full original context and detail | Shaine Meister + Grok (orchestrator) |

---

*This document is the single source of truth for all planning. New content is tracked here.*

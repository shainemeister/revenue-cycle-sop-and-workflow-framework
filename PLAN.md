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

> **v2.0 Update**: Refactored for improved chronological flow, v2 YAML front matter, and enhanced readability while preserving all content and the single-source-of-truth design. No separate phase files introduced.

---

## Executive Summary & Current Status

This is the single authoritative master plan for the Revenue Cycle SOP & Workflow Framework.

**Overall Status**: In Development — Foundational framework complete. Three model pairs developed. **Phase 3 (v2)** is active.

**Current Focus**: Completing v2 structure enhancements (YAML front matter, standalone Feedback Loop sections) and rolling out the Feedback Layer Orchestration Layer.

**Key Principle**: All planning content lives in this single file to maintain low friction, clarity, and maintainability.

---

## Development Timeline

The framework has followed a deliberate, phased approach with a strong emphasis on modularity, usability, and preparing for autonomous feedback loops.

```yaml
phases:
  - phase: 1
    name: Foundation & Core Framework
    status: Complete
    completed: May 2026
    focus:
      - Core principles, modular structure, regulatory foundations, optimization standards
      - Reusable templates
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

**Chronological Narrative**:
Phase 1 established the philosophical and structural foundation. Phase 2 delivered the first concrete model pairs. Phase 3 is now focused on making the entire system self-improving through structured feedback loops and preparing for future RCM system integration.

---

## Core Vision

### 3×3 Revenue Cycle Matrix v2

Organized into three categories with exactly three items each (Rule of 3 for low mental load):

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

**Cross-Cutting**: Feedback Loop Orchestration Layer + Contract Intelligence

### Feedback Loop Orchestration Layer

Every SOP includes a dedicated `## Feedback Loop & Data Collection Framework` section (completely separate from operational steps). This enables:
- Standardized data capture
- Closed-loop handoffs (Registration → Provider Service → Notation → Coding)
- Contract Intelligence Module that turns operational data into negotiation leverage

---

## Active Phase: Phase 3 – Structure Enhancement & Feedback Layer Rollout (v2)

**Target Completion**: End of May 2026

### Key Deliverables
- Update templates to v2 (YAML + separated Feedback Loop section) — In Progress
- Migrate model pairs (registration, visit-filing-order, demand-claim) to v2 + add real-world examples, exception tables, and common pitfalls
- Create `feedback-loop-framework.md`
- Create Contract Intelligence model pair
- Standardize Mermaid visualizations
- Update 3×3 overview diagram with bidirectional feedback arrows

### Current Status Tables

#### Framework Documents
| Document | Status | Version | Notes |
|----------|--------|---------|-------|
| core-principles.md | Complete | 1.0 | Strong foundation |
| modular-structure.md | Complete | 1.0 | Excellent modularity |
| regulatory-foundations.md | Complete | 1.0 | Risk-based |
| optimization-standards.md | Complete | 1.0 | Mental friction focus |
| structure-enhancement-implementation-guide.md | Active | 1.0 | v2 rollout guide |
| feedback-loop-framework.md | Planned | 1.0 | High priority |

#### Templates (v2)
| Template | Status | Notes |
|----------|--------|-------|
| sop-template.md | Needs Update | Add YAML + Feedback Loop section |
| workflow-template.md | Needs Update | Add YAML + Feedback Loop section |

#### SOPs & Workflows (3×3 Matrix v2)
**High Priority Model Pairs (Migration + Enhancement in progress)**
- registration.md + registration-workflow.md
- visit-filing-order.md + visit-filing-order-workflow.md
- demand-claim.md + demand-claim-workflow.md

All new content after May 14, 2026 must use v2 template.

---

## Priorities, Enhancement Backlog & Roadmap

### Immediate (Next 7 Days)
1. Enhance model SOP content depth (real-world examples, exception tables, pitfalls)
2. Standardize Mermaid visualizations
3. Complete Phase 3 template updates + model pair migrations

### Short-Term (Q2 2026)
- Create tactical adoption resources (Pilot Checklist + Adoption Guide)
- Provide modular payer-variability guidance
- Strengthen contributor onboarding in README

### Longer-Term (Q3 2026+)
- Expand to remaining 3×3 cells
- Real-world testing and feedback loops

### Enhancement Backlog (Prioritized)
1. Enhance model SOP content depth
2. Standardize Mermaid visualizations
3. Create tactical adoption resources
4. Provide modular guidance for variability
5. Strengthen contributor onboarding

---

## Governance, Metrics & Continuous Improvement

Lightweight, actionable measurement focused on reducing mental friction:
- Per SOP/Workflow: task completion time, error/rework rate, exception frequency, user-reported mental friction (1–5 scale)
- Review cadence: Framework documents quarterly; Individual SOPs 30–60 days after use

---

## Version History

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0–1.8 | May 2026 | Initial development, v1.8 integrated 5 enhancements from repo review | Shaine Meister |
| **2.0** | 2026-05-16 | Full refactor: v2 YAML front matter, improved chronological structure & flow, single-file design confirmed, feature branch implementation | Shaine Meister + Grok (orchestrator) |

---

*This document is the single source of truth for all planning. New SOPs and workflows are tracked here. No separate phase files are used.*

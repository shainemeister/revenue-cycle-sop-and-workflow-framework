---
title: "Revenue Cycle SOP & Workflow Framework - Master Plan"
short_title: "PLAN"
version: "2.2"
last_updated: "2026-05-16"
owner: "Shaine Meister"
status: "Active"
current_phase: 3
phase_focus: "Structure Enhancement & Feedback Layer Rollout (v2) - Content Deepening & Contract Intelligence"
tags:
  - planning
  - roadmap
  - v2
  - governance
  - yaml-hybrid
  - numerical-order
---

# Revenue Cycle SOP & Workflow Framework - Master Plan

**Version**: 2.2 (Hybrid YAML + Markdown)  
**Last Updated**: 2026-05-16  
**Owner**: Shaine Meister

> This is the single authoritative master plan. It uses a **hybrid structure**: YAML blocks provide structured, ordered, machine- and agent-friendly data (phases with order_of_operations, matrix, backlog). Markdown provides narrative context, formatting, and self-maintenance templates. All target dates and timelines have been removed to minimize friction during agentic workflows.

**Active Development Branch**: `phase-3-enhancements` (created for executing Phase 3 backlog items 1, 2, and 3).

---

## Executive Summary & Guiding Principles

**Overall Status**: In Development. Foundational framework complete. Three model pairs (Registration, Visit Filing Order, Demand Claim) developed and migrated to v2. **Phase 3 (v2) active** — Content deepening (registration.md enhanced), Mermaid standardization in progress, and Contract Intelligence model pair under development on feature branch.

This document serves as the single source of truth for planning, status, priorities, and clear order of operations for the Revenue Cycle SOP & Workflow Framework. It is designed to be highly instructive, numerically ordered, and suitable for both human contributors and agentic/Copilot-assisted workflows.

**Core Goals** (unchanged):
- Reusable, modular system for revenue cycle SOPs and workflows.
- Portable intellectual property adaptable across organizations and systems.
- Strong regulatory alignment and process optimization with emphasis on usability and reduced mental friction.
- Enable autonomous feedback loops and structured data collection for future RCM integration and contract intelligence.

## Phases & Order of Operations

The framework follows a deliberate phased approach with explicit numerical ordering and detailed order_of_operations for each phase.

```yaml
phases:
  - id: 1
    name: "Foundation & Core Framework"
    status: "Complete"
    order: 1
    description: "Define core principles and philosophy, establish modular structure and regulatory foundations, create optimization standards, and build reusable templates."
    order_of_operations:
      - step: "1.1"
        action: "Define and document core principles (modularity, clarity & consistency, regulatory alignment, optimization focus, reduced mental friction)"
        references: ["framework/core-principles.md"]
      - step: "1.2"
        action: "Establish modular directory structure and companion SOP + Workflow pairing model"
        references: ["framework/modular-structure.md"]
      - step: "1.3"
        action: "Create optimization standards focused on usability and predictable navigation"
        references: ["framework/optimization-standards.md"]
      - step: "1.4"
        action: "Document regulatory foundations with risk-based, light-touch integration"
        references: ["framework/regulatory-foundations.md"]
      - step: "1.5"
        action: "Build reusable v1 templates for SOPs and workflows"
        references: ["templates/"]
    key_deliverables:
      - "Core framework documents (principles, modular structure, optimization, regulatory)"
      - "Initial templates"
    references:
      - "framework/"
      - "templates/"

  - id: 2
    name: "Initial SOP & Workflow Development (Model Pairs)"
    status: "Complete"
    order: 2
    description: "Develop foundational model pairs and companion workflows for key revenue cycle functions."
    order_of_operations:
      - step: "2.1"
        action: "Develop Registration model pair (SOP + Workflow) as first high-priority model"
        references: ["sops/registration.md", "workflows/registration-workflow.md"]
      - step: "2.2"
        action: "Develop Visit Filing Order model pair"
        references: ["sops/visit-filing-order.md", "workflows/visit-filing-order-workflow.md"]
      - step: "2.3"
        action: "Develop Demand Claim model pair"
        references: ["sops/demand-claim.md", "workflows/demand-claim-workflow.md"]
    key_deliverables:
      - "Three complete model SOP + Workflow pairs"
    references:
      - "sops/"
      - "workflows/"

  - id: 3
    name: "Structure Enhancement & Feedback Layer Rollout (v2)"
    status: "Active"
    order: 3
    description: "Introduce YAML front matter and standalone Feedback Loop sections across templates and model pairs. Create feedback-loop-framework.md. Standardize Mermaid visualizations. Enhance model content depth. Create Contract Intelligence model pair. This phase makes the framework self-improving."
    order_of_operations:
      - step: "3.1"
        action: "Finalize v2 structure documentation and implementation guide"
        status: "Complete"
        references: ["structure-enhancement-implementation-guide.md"]
      - step: "3.2"
        action: "Update sop-template.md and workflow-template.md with YAML front matter + standalone ## Feedback Loop & Data Collection Framework section + comprehensive Mermaid styling standards"
        status: "Complete"
        references: ["templates/sop-template.md", "templates/workflow-template.md"]
      - step: "3.3"
        action: "Migrate existing model pairs to v2 format (preserve 100% original operational content, add YAML metadata and Feedback Loop section)"
        status: "Complete"
        references: ["sops/registration.md", "sops/visit-filing-order.md", "sops/demand-claim.md"]
      - step: "3.4"
        action: "Create feedback-loop-framework.md (governs standardized data capture, JSON schemas, closed-loop handoff protocols, and contract intelligence mapping)"
        status: "Complete"
        references: ["framework/feedback-loop-framework.md"]
      - step: "3.5"
        action: "Enhance model SOP content depth: add real-world examples, exception handling tables, and common pitfalls callouts (priority #1)"
        status: "In Progress"
        priority: "High"
        references: ["sops/registration.md"]
      - step: "3.6"
        action: "Apply standardized Mermaid styling to existing model workflows for visual consistency and closed-loop handoff clarity (priority #2)"
        status: "Planned"
        priority: "High"
        references: ["workflows/registration-workflow.md", "workflows/visit-filing-order-workflow.md", "workflows/demand-claim-workflow.md"]
      - step: "3.7"
        action: "Create Contract Intelligence model pair (feedback-loop-contract-intelligence.md + companion workflow) — critical for self-improving matrix"
        status: "In Progress"
        priority: "Critical"
        references: ["framework/feedback-loop-framework.md"]
    key_deliverables:
      - "v2 templates (YAML + Feedback sections + Mermaid standards)"
      - "feedback-loop-framework.md"
      - "v2-migrated and enhanced model pairs"
      - "Contract Intelligence model pair"
    references:
      - "PLAN.md (this file)"
      - "README.md"
      - "structure-enhancement-implementation-guide.md"
```

**Notes on Phase Execution**:
- Phases are strictly ordered (1 → 2 → 3 → 4).
- Within active phases, numbered steps (3.1, 3.2...) provide clear sequence for execution.
- Status and priority fields enable easy filtering for agents or humans.
- Work is being executed on feature branch `phase-3-enhancements`.

## 3×3 Revenue Cycle Matrix v2 Vision

The framework organizes work around a **3×3 Revenue Cycle Matrix** (Rule of 3 for low mental load) with a Cross-Cutting Feedback Loop Orchestration Layer.

**Categories**:
- **Front-End**: Patient Intake, Scheduling, Registration
- **Provider**: Service, Diagnosis/Notation (Charting), Coding
- **Back-End**: Billing (incl. patient billing), Follow-up (Insurance AR + Denials), Payment Posting / Collections

**Feedback Loop Orchestration Layer** (makes the matrix self-improving):
- Every SOP includes a dedicated standalone `## Feedback Loop & Data Collection Framework` section.
- Closed-Loop Handoff Protocol: Registration → Provider Service → Notation/Charting → Coding → back to Notation + Registration + Contract Intelligence.
- Contract Intelligence Module: Dedicated SOP + Workflow pair that converts operational data (denials, variances) into actionable intelligence.

Full visual overview maintained in `structure-enhancement-implementation-guide.md`.

```yaml
matrix:
  front_end:
    - position: "1.1"
      item: "Patient Intake"
      status: "Planned"
      priority: "Medium"
      sop_file: null
      workflow_file: null
      references: []
    - position: "1.2"
      item: "Scheduling"
      status: "Planned"
      priority: "Medium"
      sop_file: null
      workflow_file: null
      references: []
    - position: "1.3"
      item: "Registration"
      status: "Complete (v2) — Enhanced v2.1"
      priority: "High"
      sop_file: "sops/registration.md"
      workflow_file: "workflows/registration-workflow.md"
      references: ["framework/feedback-loop-framework.md"]
  provider:
    - position: "2.1"
      item: "Service"
      status: "Planned"
      priority: "High"
      sop_file: null
      workflow_file: null
      references: []
    - position: "2.2"
      item: "Diagnosis / Notation (Charting)"
      status: "Planned"
      priority: "High"
      sop_file: null
      workflow_file: null
      references: []
    - position: "2.3"
      item: "Coding"
      status: "Planned"
      priority: "High"
      sop_file: null
      workflow_file: null
      references: []
    - position: "2.0"
      item: "Contract Intelligence (Cross-Cutting)"
      status: "In Progress"
      priority: "Critical"
      sop_file: "feedback-loop-contract-intelligence.md (in development)"
      workflow_file: "feedback-loop-contract-intelligence-workflow.md (in development)"
      references: ["framework/feedback-loop-framework.md"]
  back_end:
    - position: "3.1"
      item: "Billing (incl. patient billing)"
      status: "Planned"
      priority: "High"
      sop_file: null
      workflow_file: null
      references: []
    - position: "3.2"
      item: "Insurance Denial Follow-up"
      status: "Planned"
      priority: "High"
      sop_file: null
      workflow_file: null
      references: []
    - position: "3.3"
      item: "Payment Posting / Collections"
      status: "Planned"
      priority: "Medium"
      sop_file: null
      workflow_file: null
      references: []
```

## Current Status & Structured Data

Framework documents, templates, SOPs, and Workflows are tracked in structured YAML for easy parsing and maintenance.

```yaml
framework_documents:
  - name: "core-principles.md"
    status: "Complete"
    version: "1.0"
    notes: "Strong philosophical foundation"
  - name: "modular-structure.md"
    status: "Complete"
    version: "1.0"
    notes: "Excellent modularity and pairing guidance"
  - name: "regulatory-foundations.md"
    status: "Complete"
    version: "1.0"
    notes: "Well-balanced, risk-based integration"
  - name: "optimization-standards.md"
    status: "Complete"
    version: "1.0"
    notes: "Practical focus on mental friction & flow"
  - name: "structure-enhancement-implementation-guide.md"
    status: "Active"
    version: "1.0"
    notes: "Authoritative v2 rollout guide"
  - name: "feedback-loop-framework.md"
    status: "Complete"
    version: "1.0"
    notes: "Governing document for data standards, JSON schemas, handoff protocols, and contract intelligence mapping"

templates_v2:
  - name: "sop-template.md"
    status: "Complete (v2)"
    notes: "YAML front matter + standalone Feedback Loop section + Mermaid standards"
  - name: "workflow-template.md"
    status: "Complete (v2)"
    notes: "YAML front matter + standalone Feedback Loop section + Mermaid standards"

sops:
  - name: "registration.md"
    status: "Enhanced (v2.1)"
    priority: "High"
    category: "Front-End"
    matrix_position: "1.3"
    notes: "Model pair — v2 migrated + v2.1 content enhancement complete (real-world examples, exception table, pitfalls). On phase-3-enhancements branch."
    references: ["workflows/registration-workflow.md", "framework/feedback-loop-framework.md"]
  - name: "visit-filing-order.md"
    status: "Complete (v2)"
    priority: "High"
    category: "Front-End"
    matrix_position: "1.3 (related)"
    notes: "Model pair — v2 migrated. Pending Mermaid standardization."
    references: ["workflows/visit-filing-order-workflow.md"]
  - name: "demand-claim.md"
    status: "Complete (v2)"
    priority: "High"
    category: "Front-End / Demand"
    matrix_position: "N/A (model)"
    notes: "Model pair — v2 migrated. Pending Mermaid standardization."
    references: ["workflows/demand-claim-workflow.md"]
  # Additional planned SOPs follow the same structure when created

workflows:
  - name: "registration-workflow.md"
    status: "Complete (v2)"
    priority: "High"
    category: "Front-End"
    matrix_position: "1.3"
    notes: "Model pair — v2 migrated. Pending standardized Mermaid styling (priority #2)."
    references: ["sops/registration.md"]
  - name: "visit-filing-order-workflow.md"
    status: "Complete (v2)"
    priority: "High"
    category: "Front-End"
    matrix_position: "1.3 (related)"
    notes: "Model pair — v2 migrated. Pending standardized Mermaid styling."
    references: ["sops/visit-filing-order.md"]
  - name: "demand-claim-workflow.md"
    status: "Complete (v2)"
    priority: "High"
    category: "Front-End / Demand"
    matrix_position: "N/A (model)"
    notes: "Model pair — v2 migrated. Pending standardized Mermaid styling."
    references: ["sops/demand-claim.md"]
  # Additional planned workflows follow the same structure
```

## Prioritized Backlog & Action Items (Numerical)

```yaml
backlog:
  - id: 1
    title: "Enhance model SOP content depth with real-world examples, exception tables, and common pitfalls"
    status: "In Progress / Complete on feature branch"
    priority: "High"
    category: "Content Enhancement"
    description: "Add concrete real-world examples, exception handling tables, and 'common pitfalls' callouts to model SOPs (starting with registration.md)."
    why: "Elevates models from structural references to immediately usable, high-adoption documents. Directly reduces mental friction and onboarding time."
    impact: "High — improves practical value and adoption speed for users and future contributors."
    order_of_operations:
      - "Review current model SOP content for key decision points and exceptions"
      - "Draft dedicated examples and pitfalls sections"
      - "Ensure cross-references to feedback-loop-framework.md where relevant"
      - "Update this PLAN.md backlog status and version history"
    references:
      - "sops/registration.md"
      - "PLAN.md (backlog section)"
    next_action: "Complete enhancement and merge to main. Then proceed to Mermaid standardization."

  - id: 2
    title: "Apply standardized Mermaid styling to model workflows"
    status: "Planned"
    priority: "High"
    category: "Visual Consistency"
    description: "Update existing model workflows to fully adhere to the v2 Mermaid standards defined in workflow-template.md (direction, node types, simplicity, theming)."
    why: "Ensures visual consistency across all workflows and improves clarity of closed-loop handoffs."
    impact: "High — better day-to-day usability and professional appearance."
    order_of_operations:
      - "Review current model workflows"
      - "Apply standardized Mermaid patterns and styling"
      - "Verify closed-loop handoff visualization"
      - "Update PLAN.md status"
    references:
      - "workflows/registration-workflow.md"
      - "templates/workflow-template.md"
    next_action: "Apply to registration-workflow.md and other models after SOP enhancement."

  - id: 3
    title: "Create Contract Intelligence model pair"
    status: "In Progress on feature branch"
    priority: "Critical"
    category: "Feedback Layer Completion"
    description: "Develop feedback-loop-contract-intelligence.md (SOP) + companion workflow. Leverage the new feedback-loop-framework.md."
    why: "Completes the v2 self-improving Feedback Loop Orchestration Layer and Cross-Cutting module."
    impact: "Critical — enables the matrix to turn operational data into actionable contract/legal intelligence."
    order_of_operations:
      - "Review feedback-loop-framework.md for data standards and schemas"
      - "Draft Contract Intelligence SOP and workflow using v2 templates"
      - "Ensure proper cross-references and handoff protocol alignment"
      - "Update PLAN.md and matrix YAML"
    references:
      - "framework/feedback-loop-framework.md"
    next_action: "Finalize pair and update matrix/PLAN.md."

  - id: 4
    title: "Create tactical adoption resources (Pilot Checklist + Adoption Guide)"
    status: "Planned"
    priority: "Medium"
    category: "Adoption Support"
    description: "Develop lightweight resources to help teams adopt the framework."
    why: "Supports practical rollout and contributor onboarding."
    impact: "Medium — accelerates real-world usage."
    references: []

  - id: 5
    title: "Provide modular guidance for payer-specific variability"
    status: "Planned"
    priority: "Medium"
    category: "Variability Handling"
    description: "Create templates or guidance for handling payer-specific variations."
    why: "Increases framework portability across different organizations and payers."
    impact: "Medium — improves adaptability."
    references: []
```

## How to Maintain & Update This Plan (Self-Referential Guidance)

This section provides clear, repeatable instructions so the plan remains accurate and low-friction to maintain.

**When adding a new SOP or Workflow**:
1. Create the file in `sops/` or `workflows/` using the current v2 template.
2. Append a new structured entry to the relevant YAML block in this PLAN.md (use the exact key structure from the examples above).
3. Update the Markdown narrative summary only if the change has broad impact.
4. Bump the `version` in the YAML front matter.
5. Commit with a clear message that references the numerical id or step (e.g., "Backlog item 1 — enhanced registration.md").

**Copy-paste YAML template for new backlog item**:
```yaml
  - id: X
    title: "New item title"
    status: "Planned"
    priority: "High | Medium | Low"
    category: "..."
    description: "..."
    why: "..."
    impact: "..."
    order_of_operations:
      - "Step one"
      - "Step two"
    references: []
    next_action: "..."
```

**Numerical & YAML conventions**:
- Phases are strictly ordered by `order`.
- Steps within phases use dotted numbering (3.1, 3.2...).
- Backlog items use sequential `id`.
- Always include `references` and `order_of_operations` where applicable.

## Metrics, Review Cadence & Continuous Improvement

Lightweight, actionable measurement:
- Per SOP/Workflow: task completion time, error/rework rate, exception frequency, user-reported mental friction (1–5 scale).
- Review cadence: Framework documents quarterly; individual SOPs 30–60 days after initial use.

## Version History

| Version | Changes | Author |
|---------|---------|--------|
| 1.0 | Initial plan created | Shaine Meister |
| 1.1–1.5 | Multiple refinements to model pairs and priorities | Shaine Meister |
| 1.6 | Added Phase 3 v2 with 7-step plan and created structure-enhancement-implementation-guide.md | Shaine Meister |
| 1.7 | Major expansion: full 3×3 Matrix v2 vision, Feedback Loop Orchestration Layer, Closed-Loop Handoff Protocol, Contract Intelligence Module, detailed tables | Shaine Meister |
| 1.8 | Integrated 5 recommended enhancements from repo review into plan | Shaine Meister |
| 2.0 | Refactored with v2 YAML front matter and improved chronological structure while preserving full original context and detail | Shaine Meister |
| 2.1 | Hybrid YAML + Markdown restructure: numerical ordering, explicit order_of_operations in YAML blocks, date-free design, self-maintenance templates, preserved all substantive content and references | Shaine Meister |
| **2.2** | Updated on phase-3-enhancements branch: Marked 3.5 In Progress / enhanced registration.md v2.1; 3.7 In Progress for Contract Intelligence pair; updated matrix, sops/workflows YAML, backlog statuses, and added branch note. | Shaine Meister |

---

*This document is the single source of truth for all planning. New content is tracked here using the hybrid structure.*

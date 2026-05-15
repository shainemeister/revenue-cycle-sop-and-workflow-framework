---
title: "Demand Claim Workflow"
short_title: "Demand Claim Workflow"
version: "2.0"
status: "Draft"
owner: "Shaine Meister"
last_updated: "2026-05-14"
category: "Back-End"
matrix_position: "3.2"
related_sops:
  - "demand-claim.md"
related_workflows: []
feedback_layer: "v1.0"
tags:
  - demand_claim
  - retro
  - cob
  - back_end
  - billing
  - mermaid
---

# Demand Claim Workflow

**Version**: 2.0  
**Last Updated**: 2026-05-14  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this workflow, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This workflow is the **simplified, visual quick-reference companion** to the Demand Claim SOP.

## Process Overview

This workflow provides a streamlined process for handling **Demand Claims** triggered by VFO updates and retro claims. It emphasizes the critical insurance payment pending credit review gate to prevent improper actions.

## Visual Process Flow

```mermaid
flowchart TD
    A[VFO Updated<br>Claim Retro'd]

    A --> B{Insurance Payment Pending Credit Review?}

    B -->|No| End1[DO NOT PROCEED<br>Make Note<br>Allow Credit Team Review]

    B -->|Yes| C[Initiate Demand Claim<br>AND<br>Select Payer If Appropriate<br>THEN<br>Select Dummy Printer or Test Mode]

    C --> D[Distribute Insurance Payment<br>AND<br>Move Balance to Next Responsible Party]

    D --> End2[END]
```

**Key Decision Points**
- Is there an Insurance Payment Pending Credit Review?
- Has the VFO been updated and claim retro'd?

**Critical Validation Notes**
- Only proceed if payment is pending credit review.
- Demand Claims are high-impact actions — always ensure proper sequencing.

**Notes / Tips**
- Use this workflow immediately after VFO updates that trigger retro claims.
- Coordinate with Credit Team when payment review is pending.
- Document all actions thoroughly.
- Adapt system-specific steps (e.g. Dummy Printer) to your organization's equivalent process or tool.

## Parent / Related Documents

- **Parent SOP**: [demand-claim.md](../sops/demand-claim.md)
- **Related Processes**: [Visit Filing Order SOP & Workflow](../sops/visit-filing-order.md) (main trigger) and [visit-filing-order-workflow.md](../workflows/visit-filing-order-workflow.md)

## Version History

| Version | Date       | Changes                                      | Author         |
|---------|------------|----------------------------------------------|----------------|
| 1.0     | May 9, 2026| Initial concise workflow created             | Shaine Meister |
| 1.1     | May 9, 2026| Simplified to match updated minimal Mermaid flow. Removed complex conditions gate for streamlined decision process. | Shaine Meister |
| 1.2     | May 9, 2026| Implemented Areas for Improvement and Recommendations: added full markdown links to Parent SOP and Related Processes (including Visit Filing Order pair), updated Mermaid node text for clarity on output method, added system adaptation note in Notes/Tips, updated Version, Last Updated, and Version History with implementation details. | Shaine Meister |
| 2.0     | 2026-05-14 | Migrated to v2 structure: Added YAML front matter and standalone Feedback Loop & Data Collection Framework section. Preserved 100% of original operational content and Mermaid diagram. | Shaine Meister |

## Feedback Loop & Data Collection Framework

> **Purpose of This Section**  
> This section is intentionally separated from operational steps. It serves as the standardized interface and data mapping layer for future autonomous Revenue Cycle Management systems, analytics platforms, RPA tools, and AI-driven decision engines. It enables clean integration without altering core clinical or administrative workflows.

### Data Capture Points (Structured Fields)
- `payment_review_gate_passed` (boolean, required) — Confirmation that insurance payment was pending credit review before demand
- `demand_initiated` (boolean, required) — Whether demand claim was successfully initiated
- `balance_transferred` (boolean, required) — Confirmation of balance movement to next responsible party

### Handoff Triggers & Destinations
- **Trigger**: Demand Claim completed
  - **Destination**: `feedback-loop-contract-intelligence.md` (contract performance data)
- **Trigger**: Extended payment review pending
  - **Destination**: Credit team queue

### Contract Intelligence Mapping
- Demand Claim success rate and volume by contract
- Frequency of payment review gate blocks (prevented improper actions)
- Secondary payer patterns following VFO-driven retro claims

### Automation Readiness Notes
- Highly automatable process with clear decision gate
- Simple data model ideal for RPA and analytics integration
- System-agnostic notes preserved for portability

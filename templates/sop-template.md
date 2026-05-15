---
title: "[Full SOP Title]"
short_title: "[Concise Name]"
version: "2.0"
status: "Draft"                    # Draft | In Review | Active | Deprecated
owner: "Shaine Meister"
last_updated: "2026-05-14"
category: "Front-End"              # Front-End | Provider | Back-End | Cross-Cutting
matrix_position: "1.3"             # e.g., 1.1, 1.2, 1.3, 2.1, etc.
related_sops:
  - "related-sop.md"
related_workflows:
  - "companion-workflow.md"
feedback_layer: "v1.0"             # Version of the Feedback Layer this file participates in
tags:
  - denial_prevention
  - eligibility
  - front_end
---

# [SOP Title]

**Version**: 2.0  
**Last Updated**: 2026-05-14  
**Owner**: Shaine Meister  
**Status**: Draft / In Review / Active

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> **Consider whether a companion Workflow should be created** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing).

## Purpose

Explain the business or regulatory outcome this SOP supports. Keep this concise (1–2 sentences).

## Scope

**In Scope**  
- [What this SOP covers]

**Out of Scope**  
- [What this SOP deliberately excludes]

## Roles & Responsibilities

| Role                  | Responsibilities                                      |
|-----------------------|-------------------------------------------------------|
| [Role Name]           | [Key responsibilities]                                |
| [Role Name]           | [Key responsibilities]                                |

## Prerequisites

- [Required knowledge, access, tools, or prior steps]
- [Any regulatory or compliance prerequisites]

## Step-by-Step Procedure

Use clear, numbered steps. Keep language concise and focused on the essential action. Include decision points where relevant. Avoid unnecessary detail — the goal is predictable navigation with minimal mental friction.

1. **Step Name**  
   - Action description (keep brief).  
   - Decision point: If [condition] → go to Step X. Otherwise → continue.

2. **Step Name**  
   - Action description.

**Notes / Tips** (optional)  
- [Any practical guidance that reduces friction or clarifies intent]

## Quality Checks & Common Pitfalls

- [Key validation step or check]
- [Common error or misunderstanding to avoid]
- [How to confirm the process was followed correctly]

## Optimization Notes (Optional)

- [How this SOP was designed to reduce mental friction and support intuitive flow]
- [Any text reduction or simplification choices made during development]
- [How this SOP supports predictable navigation for daily use]

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

[Brief context on relevant regulatory drivers or risk points. Do **not** reproduce full regulatory text. Focus on intent and practical implications.]

> See `regulatory-foundations.md` for the broader regulatory integration approach used in this framework.

## Related Documents

- [Link to related SOPs or workflows]
- [Link to supporting resources or references]

**Companion Workflow**  
If a companion Workflow exists for this SOP, link to it here. The Workflow serves as the simplified, visual quick-reference version for day-to-day use, while this SOP remains the authoritative documented source.

- Companion Workflow: [Link to the corresponding workflow file in `workflows/`]

## Version History

| Version | Date       | Changes                     | Author          |
|---------|------------|-----------------------------|-----------------|
| 1.0     | [Date]     | Initial version created     | Shaine Meister  |
| 2.0     | 2026-05-14 | Converted to v2 structure: Added YAML front matter and standalone Feedback Loop & Data Collection Framework section | Shaine Meister  |

## Feedback Loop & Data Collection Framework

> **Purpose of This Section**  
> This section is intentionally separated from operational steps. It serves as the standardized interface and data mapping layer for future autonomous Revenue Cycle Management systems, analytics platforms, RPA tools, and AI-driven decision engines. It enables clean integration without altering core clinical or administrative workflows.

### Data Capture Points (Structured Fields)
- Field 1: `field_name` (type, required/optional) — Description and business rule
- Field 2: ...

### Handoff Triggers & Destinations
- **Trigger**: [Specific condition or event]
  - **Destination**: `target-file.md` + Feedback Layer repository
- **Trigger**: ...

### Contract Intelligence Mapping
- Specific data points useful for legal/contract teams (payer patterns, reimbursement variances, denial root causes linked to contract terms)

### Automation Readiness Notes
- Recommended integration patterns (real-time vs batch)
- Suggested data export format (JSON schema reference)
- Error handling and retry considerations
- Notes on avoiding vendor-specific implementations

# Revenue Cycle SOP & Workflow Framework - Plan

**Version**: 1.4  
**Last Updated**: May 8, 2026  
**Owner**: Shaine Meister

## Project Goals

The primary objectives of this framework are to:

- Establish a reusable, modular system for revenue cycle SOPs and workflows.
- Create portable intellectual property that can be adapted across different organizations and systems.
- Maintain strong alignment with industry standards and regulatory requirements.
- Support ongoing process optimization and continuous improvement with a strong focus on usability and reduced mental friction.

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
    notes: All four core framework documents and both templates have been created with substantial content aligned to the principles.

  - phase: 2
    name: Initial SOP & Workflow Development
    focus:
      - Develop foundational SOPs for key revenue cycle areas (starting with Registration as the model/example)
      - Create supporting companion workflows using the established pairing pattern
      - Test and refine templates in real use
      - Establish lightweight metrics, feedback mechanisms, and review cadence
    status: In Progress
    target: Q2 - Q3 2026

  - phase: 3
    name: Expansion & Optimization
    focus:
      - Expand into additional revenue cycle functions (Billing, Denials, Appeals, Prior Auth, Coding, Patient Financial Services, etc.)
      - Refine optimization, measurement, and continuous improvement practices
      - Develop adoption guides and examples for new organizations
      - Improve documentation quality, usability, and cross-referencing
    status: Future
    target: Q3 2026 onward
```

## Current Status

**Overall Status**: In Development — Foundational framework and templates complete. Registration model pair and Visit Filing Order pair have been developed and refined. Shifting focus to Demand Claims as the next priority.

### Framework Documents

| Document                  | Status     | Notes                                      |
|---------------------------|------------|--------------------------------------------|
| core-principles.md        | Complete   | Strong philosophical foundation            |
| modular-structure.md      | Complete   | Excellent modularity and pairing guidance  |
| regulatory-foundations.md | Complete   | Well-balanced, risk-based integration      |
| optimization-standards.md | Complete   | Practical focus on mental friction & flow  |

### Templates

| Template                  | Status     | Notes                                      |
|---------------------------|------------|--------------------------------------------|
| sop-template.md           | Complete   | Comprehensive yet concise; includes alignment checks |
| workflow-template.md      | Complete   | Lightweight companion focused on visual flow |

### SOPs (Planned / In Development)

| SOP                       | Status     | Priority | Notes                                      |
|---------------------------|------------|----------|--------------------------------------------|
| registration.md           | Complete   | High     | Foundational revenue cycle entry point. **Model SOP + Companion Workflow pair completed and refined (v1.6)** |
| visit-filing-order.md     | Complete   | High     | Critical for accurate claims processing and COB resolution. **Completed as model pair (v1.2)** |
| demand-claims.md          | Planned    | Medium   | Important for denial management and follow-up |

### Workflows (Planned / In Development)

| Workflow                  | Status     | Priority | Notes                                      |
|---------------------------|------------|----------|--------------------------------------------|
| registration-workflow.md  | Complete   | High     | Companion to Registration SOP (visual quick-reference). **Completed as model pair (v1.7)** |
| visit-filing-order-workflow.md | Complete | High     | Companion to Visit Filing Order SOP. **Completed (v1.2)** |

> **Note**: Registration and Visit Filing Order pairs were developed using the established SOP + Companion Workflow pattern. Both have been refined and aligned with the core framework documents.

## Next Priorities

### Immediate Priorities (Next 1–2 Weeks)
- Mark Visit Filing Order pair as Complete / Active.
- Begin development of **Demand Claims SOP + Companion Workflow** (next priority after Visit Filing Order).

### Short-Term Priorities (Q2 2026)
- Develop **Demand Claims SOP + Companion Workflow**.
- Establish lightweight metrics/feedback mechanisms and a simple review cadence.
- Begin documenting real-world usage notes and friction points from the Registration and Visit Filing Order models.

### Longer-Term Priorities (Q3 2026+)
- Expand SOP coverage to additional high-impact revenue cycle functions (Billing & Charge Capture, Denials Management & Appeals, Prior Authorization, Coding & Documentation, Patient Access & Financial Counseling, etc.).
- Develop an "Adoption & Getting Started" guide for implementing the framework in new organizations.
- Introduce more advanced optimization practices, measurement, and continuous improvement loops.
- Create guidance for handling high-variability processes (e.g., payer-specific rules).

## Metrics, Review Cadence & Continuous Improvement

This framework prioritizes **lightweight, actionable measurement** that supports improvement without adding mental friction (per `optimization-standards.md`).

### Recommended Approach
- **Per SOP/Workflow**: 
  - Leading indicators: Task completion time, error/rework rate, exception frequency, user-reported mental friction (simple 1–5 scale or qualitative notes).
  - Compliance: Audit readiness / pass rate on relevant controls.
- **Framework Level**: Number of SOPs created, adoption across contexts, reduction in process variation, user feedback on usability.
- **Feedback Mechanisms**: Built-in "Friction / Improvement Notes" section in each SOP; periodic team huddles or simple surveys; trigger-based reviews (recurring exceptions, regulatory changes, or performance drift).

### Review Cadence
- **Framework documents & templates**: Quarterly review or triggered by major regulatory/organizational changes.
- **Individual SOPs**: Initial review after 30–60 days of use; then annually or on trigger.
- **Workflows**: More frequent informal review (as they are day-to-day tools).

> See `optimization-standards.md` for the guiding philosophy on measurement and continuous small improvements.

## Open Items & Notes

- Populate **Demand Claims** as the next high-priority SOP + Workflow.
- Decide on visual workflow standards (Mermaid diagram depth, styling conventions).
- Develop lightweight metrics and simple feedback capture mechanisms that fit naturally into daily work.
- Create guidance for handling high-variability / payer-specific processes.
- Develop a short "Adoption / Getting Started" guide and example metrics templates.
- Establish a sustainable review cadence and ownership model as the library grows.
- Consider adding a glossary of key revenue cycle terms for consistency.

## Version History

| Version | Date          | Changes                                                                 | Author          |
|---------|---------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 2026      | Initial plan created                                                    | Shaine Meister  |
| 1.1     | May 6, 2026   | Updated statuses to reflect completed framework and templates; refined priorities and added Metrics section | Shaine Meister  |
| 1.2     | May 6, 2026   | Added Registration SOP + Companion Workflow as completed model pair (status changed to Draft) | Shaine Meister  |
| 1.3     | May 7, 2026   | Updated Registration SOP (v1.6) and Workflow (v1.7) to Complete status after multiple refinements and successful framework integrity check. Updated immediate priorities and notes. | Shaine Meister  |
| 1.4     | May 8, 2026   | Updated Visit Filing Order SOP (v1.2) and Workflow (v1.2) to Complete status. Added visit-filing-order-workflow.md to tracking. Updated Next Priorities to focus on Demand Claims development. | Shaine Meister  |

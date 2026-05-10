# Revenue Cycle SOP & Workflow Framework - Plan

**Version**: 1.5  
**Last Updated**: May 9, 2026  
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

**Overall Status**: In Development — Foundational framework and templates complete. Registration model pair, Visit Filing Order pair, and Demand Claims pair have been developed and refined. All three model pairs now follow the SOP + Companion Workflow pattern with recent improvements applied.

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
| visit-filing-order.md     | Complete   | High     | Critical for accurate claims processing and COB resolution. **Completed as model pair (v1.3)** |
| demand-claim.md           | Complete   | High     | Important for denial management, secondary billing, and follow-up after VFO/retro. **Completed as model pair (v1.2)** |

### Workflows (Planned / In Development)

| Workflow                  | Status     | Priority | Notes                                      |
|---------------------------|------------|----------|--------------------------------------------|
| registration-workflow.md  | Complete   | High     | Companion to Registration SOP (visual quick-reference). **Completed as model pair (v1.7)** |
| visit-filing-order-workflow.md | Complete | High     | Companion to Visit Filing Order SOP. **Completed (v1.3)** |
| demand-claim-workflow.md  | Complete   | High     | Companion to Demand Claim SOP. **Completed (v1.2)** |

> **Note**: All model pairs (Registration, Visit Filing Order, Demand Claims) were developed using the established SOP + Companion Workflow pattern. Recent refinements include standardized structures, improved cross-referencing, cleaned Mermaid diagrams, added Notes/Tips sections, and better handling of system-specific elements while maintaining portability.

## Next Priorities

### Immediate Priorities (Next 1–2 Weeks)
- Monitor real-world usage and gather feedback on the Demand Claims pair (now complete).
- Mark all current model pairs as Active / In Use where appropriate.
- Begin documenting real-world usage notes and friction points from the Registration, Visit Filing Order, and Demand Claims models.

### Short-Term Priorities (Q2 2026)
- Establish lightweight metrics/feedback mechanisms and a simple review cadence across implemented pairs.
- Refine any identified friction points from initial usage.
- Continue testing templates in real operational contexts.

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

- Decide on visual workflow standards (Mermaid diagram depth, styling conventions) — partially addressed with recent Mermaid cleanups.
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
| 1.5     | May 9, 2026   | Updated to reflect completion of Demand Claims (demand-claim.md + demand-claim-workflow.md) as model pair. Fixed SOP table filename reference (demand-claims.md → demand-claim.md). Updated Current Status, Next Priorities, Open Items, and added new workflow to tracking. Incorporated outcomes from implementing Areas for Improvement and Recommendations across all model files (standardized structures, improved links/cross-references, cleaned diagrams, added Notes/Tips, generalized system-specific guidance). Updated Version and Last Updated. | Shaine Meister  |
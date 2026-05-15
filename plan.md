# Revenue Cycle SOP & Workflow Framework - Plan

**Version**: 1.6  
**Last Updated**: May 14, 2026  
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
    name: Structure Enhancement & Feedback Layer Rollout (v2)
    focus:
      - Introduce modern YAML front matter for metadata and dependency mapping
      - Add completely separate Feedback Loop & Data Collection Framework section to every SOP and Workflow
      - Create governing implementation guide and data standards
      - Apply v2 structure to all existing model pairs
      - Enable future autonomous RCM system integration and contract intelligence
    status: In Progress
    target: May - June 2026
    notes: This phase addresses the critical gap in autonomous feedback loops (especially Registration → Notation → Coding) and prepares the framework for future RCM platform mapping.

  - phase: 4
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
| structure-enhancement-implementation-guide.md | Active | New v2 instructional extension (May 2026) |

### Templates

| Template                  | Status     | Notes                                      |
|---------------------------|------------|--------------------------------------------|
| sop-template.md           | Complete   | To be updated to v2 (YAML + Feedback section) |
| workflow-template.md      | Complete   | To be updated to v2 (YAML + Feedback section) |

### SOPs (Planned / In Development)

| SOP                       | Status     | Priority | Notes                                      |
|---------------------------|------------|----------|--------------------------------------------|
| registration.md           | Complete   | High     | Foundational revenue cycle entry point. **Model SOP + Companion Workflow pair completed and refined (v1.6)** — To be migrated to v2 structure |
| visit-filing-order.md     | Complete   | High     | Critical for accurate claims processing and COB resolution. **Completed as model pair (v1.3)** — To be migrated to v2 |
| demand-claim.md           | Complete   | High     | Important for denial management, secondary billing, and follow-up after VFO/retro. **Completed as model pair (v1.2)** — To be migrated to v2 |

### Workflows (Planned / In Development)

| Workflow                  | Status     | Priority | Notes                                      |
|---------------------------|------------|----------|--------------------------------------------|
| registration-workflow.md  | Complete   | High     | Companion to Registration SOP (visual quick-reference). **Completed as model pair (v1.7)** — To be migrated to v2 |
| visit-filing-order-workflow.md | Complete | High     | Companion to Visit Filing Order SOP. **Completed (v1.3)** — To be migrated to v2 |
| demand-claim-workflow.md  | Complete   | High     | Companion to Demand Claim SOP. **Completed (v1.2)** — To be migrated to v2 |

> **Note**: All model pairs (Registration, Visit Filing Order, Demand Claims) were developed using the established SOP + Companion Workflow pattern. Recent refinements include standardized structures, improved cross-referencing, cleaned Mermaid diagrams, added Notes/Tips sections, and better handling of system-specific elements while maintaining portability. **Phase 3 (v2) will migrate all existing pairs to the new YAML + Feedback Layer structure.**

## Phase 3: Structure Enhancement & Feedback Layer Rollout (v2) – Step-by-Step Implementation Plan

This phase introduces the modern v2 structure to address the critical feedback loop gap and prepare the framework for future autonomous RCM systems and contract intelligence. All changes are documented in detail in the new `structure-enhancement-implementation-guide.md` file.

### Step-by-Step Process

1. **Create v2 Implementation Guide**  
   Create `structure-enhancement-implementation-guide.md` as the authoritative reference for YAML front matter, the new Feedback Loop section format, and rationale. *(Completed – May 14, 2026)*

2. **Update Core Templates to v2**  
   Modify `sop-template.md` and `workflow-template.md` to include:
   - Modern YAML front matter block at the top
   - New standalone `## Feedback Loop & Data Collection Framework` section at the very bottom (completely separate from operational content)
   - Updated cross-reference and matrix_position fields

3. **Migrate Existing Model Pairs to v2**  
   Apply the new v2 structure to all six existing files:
   - `registration.md` + `registration-workflow.md`
   - `visit-filing-order.md` + `visit-filing-order-workflow.md`
   - `demand-claim.md` + `demand-claim-workflow.md`
   - Preserve all original operational content while adding YAML metadata and the new Feedback section

4. **Create Feedback Layer Governing Document**  
   Develop `feedback-loop-framework.md` to define:
   - Standardized data capture fields and JSON schemas
   - Handoff protocols and trigger conditions
   - Contract intelligence data mapping
   - Automation readiness guidelines (generic, no vendor IP)

5. **Update All Future Development**  
   From this point forward, every new SOP and Workflow must be created using the v2 templates only. All new files must include the Feedback Loop section and proper YAML front matter.

6. **Team Onboarding & Documentation**  
   Update team on the new structure, purpose of the Feedback Layer (future RCM system mapping + contract intelligence), and how to maintain the separation between operational content and data collection sections.

7. **Validation & Continuous Improvement**  
   After migration, review all v2 files for consistency. Add any refinements to the `structure-enhancement-implementation-guide.md` based on real usage.

**Target Completion**: End of May 2026 (parallel with ongoing Phase 2 usage and feedback collection).

## Next Priorities

### Immediate Priorities (Next 1–2 Weeks)
- Complete Phase 3 v2 migration of all existing model pairs.
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
- **Phase 3 v2 items**: Complete template updates, migrate 6 existing files, create `feedback-loop-framework.md`.

## Version History

| Version | Date          | Changes                                                                 | Author          |
|---------|---------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 2026      | Initial plan created                                                    | Shaine Meister  |
| 1.1     | May 6, 2026   | Updated statuses to reflect completed framework and templates; refined priorities and added Metrics section | Shaine Meister  |
| 1.2     | May 6, 2026   | Added Registration SOP + Companion Workflow as completed model pair (status changed to Draft) | Shaine Meister  |
| 1.3     | May 7, 2026   | Updated Registration SOP (v1.6) and Workflow (v1.7) to Complete status after multiple refinements and successful framework integrity check. Updated immediate priorities and notes. | Shaine Meister  |
| 1.4     | May 8, 2026   | Updated Visit Filing Order SOP (v1.2) and Workflow (v1.2) to Complete status. Added visit-filing-order-workflow.md to tracking. Updated Next Priorities to focus on Demand Claims development. | Shaine Meister  |
| 1.5     | May 9, 2026   | Updated to reflect completion of Demand Claims (demand-claim.md + demand-claim-workflow.md) as model pair. Fixed SOP table filename reference (demand-claims.md → demand-claim.md). Updated Current Status, Next Priorities, Open Items, and added new workflow to tracking. Incorporated outcomes from implementing Areas for Improvement and Recommendations across all model files (standardized structures, improved links/cross-references, cleaned diagrams, added Notes/Tips, generalized system-specific guidance). Updated Version and Last Updated. | Shaine Meister  |
| 1.6     | May 14, 2026  | Added Phase 3: Structure Enhancement & Feedback Layer Rollout (v2) with detailed 7-step implementation plan. Created new `structure-enhancement-implementation-guide.md` as the authoritative extension document. Updated roadmap YAML, tables, and Version History. This phase directly addresses the critical feedback loop gap in the Registration → Notation → Coding chain and prepares the framework for future autonomous RCM system integration and contract intelligence. | Shaine Meister  |

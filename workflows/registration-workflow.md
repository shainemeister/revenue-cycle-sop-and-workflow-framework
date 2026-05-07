# Registration Verification & Follow-Up Workflow (Back-End)

**Version**: 1.6  
**Last Updated**: May 6, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this workflow, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This workflow is intended as the **simplified, visual quick-reference companion** to its parent SOP (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing).

## Process Overview

This workflow provides a practical visual reference for back-end Revenue Cycle teams. The Eligibility section has been simplified for better readability while retaining the key real-world distinctions. Use alongside the full Registration Verification & Follow-Up SOP.

## Visual Process Flow

```mermaid
flowchart TD
    A[Denial / Edit / Work Queue Received] --> B[Review Denial Code<br/>or Remark]
    B --> C{Is this a<br/>Registration Issue?}
    C -->|No| D[Handoff to Billing,<br/>Coding or Denials Team]
    C -->|Yes| E[Identify Root Cause Category]
    
    %% === ELIGIBILITY PATH ===
    E --> F{Eligibility Issue?}
    F -->|Yes| G[Check Eligibility Type]
    
    G --> G1[Patient Active / Coverage Issue]
    G1 --> G1a[Re-verify Eligibility<br/>Update Registration]
    
    G --> G2[Demographic / Registration Error]
    G2 --> G2a[Correct Demographics<br/>Re-verify Eligibility]
    
    G --> G3[Newborn Scenario<br/>(30-day Grace Period)]
    G3 --> G3a[Send Notification Letter<br/>(Regulatory / Courtesy)]
    
    G --> G4[Patient Involvement Needed]
    G4 --> G4a[Send Letter to Patient/Guarantor<br/>Move to Self-Pay<br/>(Exception: Medicaid/Medicare)]
    
    %% === COB PATH ===
    F -->|No| H{COB Issue?}
    H -->|Yes| I[COB Follow-up Path]
    I --> I1[Update Registration<br/>and/or Fix Filing Order]
    I --> I2[Contact Payer<br/>to Verify / Reprocess]
    I --> I3[Send Patient/Guarantor<br/>Letter for COB Update]
    
    %% === AUTHORIZATION PATH ===
    H -->|No| J{Authorization Issue?}
    J -->|Yes| K[Verify / Obtain<br/>or Update Authorization]
    J -->|No| L[Research & Correct<br/>Other Registration Data]
    
    %% Convergence to Document
    G1a --> M[Document Changes<br/>& Rationale]
    G2a --> M
    G3a --> M
    G4a --> M
    I1 --> M
    I2 --> M
    I3 --> M
    K --> M
    L --> M
    
    M --> N[Resubmit Claim<br/>or Continue Follow-up]
    N --> O{Recurring Issue<br/>or Trend?}
    O -->|Yes| P[Report to Supervisor<br/>/ Quality Team]
    O -->|No| Q[Monitor for Recurrence]
    P --> Q
    D --> R[End]
    Q --> R
```

**Key Decision Points**  
- Is this a Registration Issue? → Triage for back-end ownership.  
- Under Eligibility: Four distinct scenarios with dedicated resolution paths.  
- COB and Authorization remain separate categories.  
- Recurring issues → Escalate for trend analysis.

**Notes**  
- Eligibility path covers: Patient active/coverage, demographic errors, newborn 30-day grace period, and patient involvement decisions.  
- COB path shows three common outcomes.  
- Diagram prioritizes clarity of categories while remaining usable as a quick reference.

## Parent SOP

- [registration.md](../sops/registration.md) — Full procedures, roles, quality checks, optimization guidance, and version history.

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial front-end focused version created                               | Shaine Meister  |
| 1.1     | May 6, 2026| Revised to align with back-end SOP focus                                | Shaine Meister  |
| 1.2     | May 6, 2026| Denial-driven flow with triage and root cause                           | Shaine Meister  |
| 1.3     | May 6, 2026| Added COB variability with three resolution outcomes                    | Shaine Meister  |
| 1.4     | May 6, 2026| Separated Eligibility, COB, and Authorization into distinct categories  | Shaine Meister  |
| 1.5     | May 6, 2026| Expanded Eligibility with granular scenarios                            | Shaine Meister  |
| 1.6     | May 6, 2026| Fixed Mermaid syntax error in Visual Process Flow (line 11 area). Restructured Eligibility paths with separate lines for clarity and reduced overlap. Version kept at 1.6 per request. | Shaine Meister  |

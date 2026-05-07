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
    
    G --> G1[Patient Active / Coverage Issue] --> G1a[Re-verify Eligibility<br/>Update Registration]
    G --> G2[Demographic / Registration Error] --> G2a[Correct Demographics<br/>Re-verify Eligibility]
    G --> G3[Newborn Scenario<br/>(30-day Grace Period)] --> G3a[Send Notification Letter<br/>(Regulatory / Courtesy)]
    G --> G4[Patient Involvement Needed] --> G4a[Send Letter to Patient/Guarantor<br/>Move to Self-Pay<br/>(Exception: Medicaid/Medicare)]
    
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
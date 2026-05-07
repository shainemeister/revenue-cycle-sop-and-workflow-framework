# Registration Verification & Follow-Up Workflow (Back-End)

**Version**: 1.6  
**Last Updated**: May 6, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this workflow, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This workflow is intended as the **simplified, visual quick-reference companion** to its parent SOP (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing).

## Process Overview

This workflow is split into three focused Visual Process Flows to improve clarity and reduce complexity:
- **Eligibility**
- **Coordination of Benefits (COB)**
- **Authorization**

Each section can be referenced independently while still supporting the overall back-end registration follow-up process. Use alongside the full Registration Verification & Follow-Up SOP.

## Visual Process Flow: Eligibility

```mermaid
flowchart TD
    A[Eligibility Issue Identified] --> B{Check Eligibility Type}
    
    B -->|Patient Active / Coverage Issue| B1["Re-verify Eligibility<br>Update Registration"]
    B -->|Demographic / Registration Error| B2["Correct Demographics<br>Re-verify Eligibility"]
    B -->|Newborn Scenario - 30-day Grace Period| B3["Send Notification Letter<br>(Regulatory / Courtesy)"]
    B -->|Patient Involvement Needed| B4["Send Letter to Patient/Guarantor"]
    
    B4 --> B4a{3 Contact Attempts Completed?}
    B4a -->|Yes| B4b["Move Balance to Self-Pay<br>(Exception: Medicaid/Medicare)"]
    B4a -->|No| B4c[Continue Outreach Attempts]
    
    B1 --> C["Document Changes<br>& Rationale"]
    B2 --> C
    B3 --> C
    B4b --> C
    B4c --> C
    
    C --> D["Resubmit Claim<br>or Continue Follow-up"]
```

## Visual Process Flow: Coordination of Benefits (COB)

```mermaid
flowchart TD
    A[COB Issue Identified] --> B[COB Follow-up Path]
    
    B --> B1["Update Registration<br>and/or Fix Filing Order"]
    B --> B2["Contact Payer<br>to Verify / Reprocess Claim"]
    B --> B3["Send Patient/Guarantor<br>Letter for COB Update"]
    
    B1 --> C["Document Changes<br>& Rationale"]
    B2 --> C
    B3 --> C
    
    C --> D["Resubmit Claim<br>or Continue Follow-up"]
```

## Visual Process Flow: Authorization

```mermaid
flowchart TD
    A[Authorization Denial Identified] --> Q1{Was Prior Authorization obtained and valid before service?}
    
    Q1 -->|Yes| CorrectClaim["Correct claim by adding authorization number/details and resubmit"]
    
    Q1 -->|No| Q2{Can retroactive authorization be requested?}
    
    Q2 -->|Yes| SubmitRetro["Submit retroactive PA request to payer"]
    Q2 -->|No| PrepareAppeal["Prepare formal appeal for lack of prior authorization"]
    
    SubmitRetro --> RetroResult{Retro PA approved?}
    RetroResult -->|Yes| CorrectClaim
    RetroResult -->|No| PrepareAppeal
    
    CorrectClaim --> Update["Update account and close follow-up"]
    
    PrepareAppeal --> Q3{Within timely filing / appeal deadline?}
    Q3 -->|Yes| FileAppeal["File formal appeal"]
    Q3 -->|No| PatientResp{Patient Responsibility?}
    
    FileAppeal --> Update
    
    PatientResp -->|Yes| SelfPay["Complete follow-up note and move balance to self-pay"]
    PatientResp -->|No| WriteOff["Submit or apply appropriate write-off"]
    
    SelfPay --> Update
    WriteOff --> Update
    
    Update --> Prevention["Document root cause and provide feedback to front-end authorization process"]
    Prevention --> End([Workflow Complete — Revenue Protected or Account Resolved])
```

**Key Decision Points**  
- Under **Eligibility**: Four distinct scenarios with clear resolution paths, including patient outreach rules.  
- Under **COB**: Three resolution outcomes based on required action.  
- Under **Authorization**: Structured decision tree covering prior auth validity, retroactive requests, appeals, timely filing, and patient responsibility vs. write-off.  
- All paths lead to documentation and account resolution.

**Notes**  
- The Eligibility diagram now clearly separates sending the patient letter from the decision to move the balance to self-pay after 3 contact attempts (with Medicaid/Medicare exception noted).  
- The Authorization diagram follows a logical real-world denial workflow while maintaining visual consistency with the other sections.  
- Each category remains independently usable.

## Parent SOP

- [registration.md](../sops/registration.md) — Full procedures, roles, quality checks, optimization guidance, and version history.

## Version History

| Version | Date       | Changes                                                                 | Author          |\n|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial front-end focused version created                               | Shaine Meister  |\n| 1.1     | May 6, 2026| Revised to align with back-end SOP focus                                | Shaine Meister  |\n| 1.2     | May 6, 2026| Denial-driven flow with triage and root cause                           | Shaine Meister  |\n| 1.3     | May 6, 2026| Added COB variability with three resolution outcomes                    | Shaine Meister  |\n| 1.4     | May 6, 2026| Separated Eligibility, COB, and Authorization into distinct categories  | Shaine Meister  |\n| 1.5     | May 6, 2026| Expanded Eligibility with granular scenarios                            | Shaine Meister  |\n| 1.6     | May 6, 2026| Refined Eligibility diagram (separated patient letter from self-pay move after 3 contact attempts). Updated Authorization diagram for better real-world flow while maintaining style consistency. Version kept at 1.6. | Shaine Meister  |
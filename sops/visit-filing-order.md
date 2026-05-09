# Visit Filing Order

**Version**: 1.0  
**Last Updated**: May 8, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This SOP is paired with a **Companion Workflow** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing). The workflow provides a visual decision tree for determining and correcting filing order.

## Purpose

To establish a clear, repeatable process for identifying multiple active insurances, determining the correct primary/secondary/tertiary payer filing order for a specific visit/encounter, and updating the registration system accordingly. 

This SOP serves as the detailed expansion of the “correct filing order (internal fix)” action within the Coordination of Benefits (COB) procedures in the Registration Verification & Follow-Up SOP. Accurate filing order prevents claim rejections and denials related to COB, ensures claims are routed to the correct primary payer first, and supports timely and compliant revenue capture.

## Scope

**In Scope**  
- Review of patient accounts with suspected or confirmed multiple insurance coverage on the date of service.
- Application of standard Coordination of Benefits (COB) rules to determine correct filing order (e.g., birthday rule, employer coverage rules, Medicare Secondary Payer rules).
- Verification of current insurance information and filing order in the registration system.
- Updating registration records with the correct primary, secondary, and tertiary payer sequence.
- Documentation of the rationale and sources used to determine filing order.
- Coordination with billing teams for reprocessing or clean claim submission.

**Out of Scope**  
- Front-end patient registration and insurance verification at point of service.
- Complex legal or contractual COB disputes requiring legal review.
- Payer-specific COB investigations beyond standard rules (escalate as needed).
- Final claim submission and payer follow-up (Billing team responsibility).

## Roles & Responsibilities

| Role                                      | Responsibilities                                                                 |
|-------------------------------------------|----------------------------------------------------------------------------------|
| Revenue Cycle Registration Specialist     | Review accounts, apply COB rules, verify and update filing order in registration system, document changes |
| Registration Quality / Denial Prevention Analyst | Audit filing order accuracy, identify trends in COB-related denials, provide feedback and training |
| Billing Coordinator / Specialist          | Flag COB/filing order related claim edits and coordinate resolution with Registration team |
| Revenue Cycle Supervisor                  | Oversee complex COB cases, approve escalations, monitor timely filing impact |

## Prerequisites

- Access to registration system, eligibility verification tools, and payer portals.
- Solid understanding of common Coordination of Benefits rules (birthday rule, employer vs. individual coverage, Medicare Secondary Payer guidelines).
- Ability to research patient insurance history across multiple sources.
- Familiarity with the Registration Verification & Follow-Up SOP (especially the COB section).
- Training on HIPAA and proper documentation standards for account changes.

## Step-by-Step Procedure

This procedure expands the high-level COB action from the Registration SOP. Use the companion **Visit Filing Order Workflow** for a visual quick-reference of the decision flow.

### 1. Identify Accounts Requiring Filing Order Review

- Review work queue items, claim edits, or denial reports flagged for COB or "incorrect primary payer" issues.
- Confirm the denial/edit is related to filing order rather than eligibility or authorization.

### 2. Confirm Multiple Active Insurances on Date of Service

- Check the patient’s insurance information in the registration system for the specific date of service.
- Verify coverage was active on the date of service for all listed insurances.
- **Decision Point**: If only one active insurance → No COB issue. Document and close.

### 3. Determine the Correct Primary Payer Using Applicable COB Rules

Apply the relevant Coordination of Benefits rule(s) based on the types of coverage:

- **Birthday Rule** (most common for dependents with two parent plans): The parent whose birthday falls earlier in the calendar year is primary.
- **Employer Coverage**: Coverage through the patient’s own employer is usually primary over a spouse’s or parent’s plan.
- **Medicare Secondary Payer (MSP) Rules**: Apply specific MSP guidelines (e.g., working aged, disability, ESRD) when Medicare is involved.
- **Other Rules**: Court order, military coverage, or specific payer contracts may override standard rules.

Document which rule(s) were applied and why.

### 4. Verify Current Filing Order in the System

- Compare the system’s current primary/secondary/tertiary designation against the correct order determined in Step 3.
- **Decision Point**: If current filing order is correct → Document verification and proceed to clean claim submission or reprocessing request.

### 5. Update the Registration System with Correct Filing Order

- Change the insurance sequence (primary → secondary → tertiary) to reflect the correct order.
- Ensure all related fields (subscriber ID, group number, relationship to insured, etc.) are accurate for the new primary payer.
- Save changes with clear before/after documentation.

### 6. Add Detailed Account Note

Include:
- Date and time of change
- User making the change
- Specific COB rule applied
- Sources used for verification (e.g., payer portal response, eligibility response, prior claims)
- Before and after filing order

### 7. Flag Account for Reprocessing or Clean Submission

- If a claim was already submitted to the incorrect primary payer: Coordinate with Billing to void/reprocess or request payer reprocessing.
- If no claim submitted yet: Release for clean claim submission to the correct primary payer.

### 8. Escalate When Necessary

Escalate to supervisor or COB specialist when:
- Payer-specific rules conflict with standard COB guidelines
- High-dollar accounts or complex multi-payer situations
- Uncertainty about which rule applies

## Quality Checks & Common Pitfalls

- Always verify insurance against the **exact date of service**, not current coverage.
- Confirm subscriber vs. patient relationship after any updates.
- Common pitfall: Applying the wrong COB rule (e.g., assuming employer coverage is always primary without checking).
- Common pitfall: Failing to document the specific rule and sources used.
- Common pitfall: Updating filing order without re-verifying eligibility for the new primary payer.
- Quality check: After update, re-run eligibility or scrubber to confirm the account is clean for submission.

## Optimization Notes (Optional)

- This SOP and its companion workflow are designed for predictable navigation with minimal mental friction by separating identification, rule application, verification, update, and documentation into clear sequential steps.
- The workflow provides the visual overview while this SOP supplies the necessary depth and examples.
- Text volume is kept focused on actionable decision points and common rules rather than exhaustive regulatory text.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **Coordination of Benefits**: Follow all applicable federal and state COB regulations and payer contracts.
- **Timely Filing**: Corrections to filing order must be completed within payer timely filing limits to avoid denials.
- **Audit Trail**: Every change to insurance order must be fully documented with rationale and sources (supports audit defensibility).
- **HIPAA**: Protect all patient health information during research and updates.
- **Medicare Secondary Payer**: Strict adherence to MSP rules is required; incorrect filing order can trigger overpayment recovery actions.

> See `regulatory-foundations.md` for broader regulatory guidance.

## Related Documents

- **Companion Workflow**: [visit-filing-order-workflow.md](../workflows/visit-filing-order-workflow.md) — Visual decision tree for quick daily reference.
- **Registration Verification & Follow-Up SOP**: [registration.md](../sops/registration.md) — COB section (specifically the “Update registration and/or correct filing order (internal fix)” action).
- Future: Denial Management SOP (planned)
- Organizational policies on Coordination of Benefits and timely filing

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 8, 2026| Initial version created as detailed expansion of COB filing order action from Registration SOP | Shaine Meister (with Grok) |
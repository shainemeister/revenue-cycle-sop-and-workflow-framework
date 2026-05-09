# Visit Filing Order

**Version**: 1.2  
**Last Updated**: May 8, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This SOP is paired with a **Companion Workflow** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing). The workflow provides a visual decision tree focused on validation gates and consequential VFO changes.

## Purpose

To establish a clear, repeatable process for determining whether a Visit Filing Order (VFO) update is required and supported by COB research, verifying the correct order, and safely applying changes — especially when claims have already been generated.

This SOP serves as the detailed expansion of the “correct filing order (internal fix)” action within the Coordination of Benefits (COB) procedures in the Registration Verification & Follow-Up SOP. It emphasizes validation before making consequential changes to the Visit Filing Order.

## Scope

**In Scope**  
- Review of patient accounts with suspected or confirmed multiple insurance coverage on the date of service.
- Validation that a VFO update is required **and** supported by documented COB research notes.
- Verification of the correct primary/secondary/tertiary payer sequence for a specific visit.
- Updating the Visit Filing Order in the registration system, with appropriate handling for retro review.
- Documentation of the rationale and sources supporting the VFO change.
- Coordination with billing for reprocessing, retro adjudication, or handoff to Demand Claims processes when primary claims have paid.

**Out of Scope**  
- Front-end patient registration and insurance verification at point of service.
- Complex legal or contractual COB disputes requiring legal review.
- Payer-specific COB investigations beyond standard rules (escalate as needed).
- Final claim submission and ongoing payer follow-up (Billing team responsibility).

## Roles & Responsibilities

| Role                                      | Responsibilities                                                                 |
|-------------------------------------------|----------------------------------------------------------------------------------|
| Revenue Cycle Registration Specialist     | Review accounts, validate VFO update requirement and COB research support, verify and update filing order, document changes |\\n| Registration Quality / Denial Prevention Analyst | Audit VFO accuracy and change documentation, identify trends, provide feedback |\\n| Billing Coordinator / Specialist          | Coordinate reprocessing, retro review, and Demand Claim handoffs related to VFO changes |\\n| Revenue Cycle Supervisor                  | Oversee complex VFO cases, approve escalations, monitor timely filing and financial impact |\\n
## Prerequisites

- Access to registration system, eligibility verification tools, payer portals, and work queues.
- Solid understanding of common Coordination of Benefits rules and how they apply to Visit Filing Order vs. Patient Filing Order.
- Ability to research and document COB rationale clearly.
- Familiarity with the Registration Verification & Follow-Up SOP (especially the COB section).
- Understanding of retro adjudication processes and Demand Claim workflows.
- Training on HIPAA and proper documentation standards for account changes.

## Step-by-Step Procedure

This procedure follows the companion **Visit Filing Order Workflow**. All changes to Visit Filing Order are consequential and require validation.

### 1. Triage: Determine if VFO Update is Required and Supported

- Review the COB / Visit Filing Order issue from work queue, claim edit, or denial.
- Confirm whether a VFO update is required.
- **Critical Validation Gate**: Verify that a COB Research Note exists and supports the proposed VFO change.
- **Decision**: If VFO update is **not** required **or** COB Research Note does **not** support the change → Refer to the Registration Verification & Follow-Up SOP and Workflow for alternative COB actions.

### 2. Verify the Correct Visit Filing Order

- Review all active insurances for the specific date of service.
- Apply applicable COB rules (Birthday Rule, Employer coverage rules, Medicare Secondary Payer guidelines, etc.) to determine the correct primary → secondary → tertiary order.
- Document which COB rules were applied and the supporting sources.

### 3. Check if Claims Have Been Generated for the Visit

- Determine whether claims have already been created and submitted for this visit.
- **Decision Point**: Claims Generated?

### 4a. If No Claims Generated Yet

- Update the Visit Filing Order in the registration system.
- Allow for retro review as applicable.
- Proceed to Step 5 (Documentation).

### 4b. If Claims Have Been Generated

- Check whether the primary payer has adjudicated/paid **and** there is a need to bill secondary.
- **If Yes (Primary Paid + Need to Bill Secondary)**:
  - Add a detailed account note documenting the VFO change rationale.
  - Proceed with the VFO update.
  - Force retro review/adjudication.
  - Handoff to the Demand Claim SOP / Workflow for secondary billing and follow-up.
- **If No**:
  - Proceed directly to documentation and update.

### 5. Add Detailed Account Note Supporting the VFO Change

The note must include:
- Date/time of change and user performing the update
- Confirmation that COB Research Note supported the change
- Specific COB rules applied and sources used
- Before and after Visit Filing Order
- Any retro review or Demand Claim actions triggered

### 6. Finalize and Advance the Account

- Flag the account appropriately for re-scrub, reprocessing, or retro work queue.
- Release the account for next steps (clean submission, NRP cascade, or Demand Claim process).

## Quality Checks & Common Pitfalls

- Always verify coverage against the **exact date of service**, not current coverage.
- Never update VFO without a supporting COB Research Note.
- Common pitfall: Updating VFO after primary has paid without forcing retro review and coordinating secondary billing.
- Common pitfall: Insufficient documentation of the rationale and COB rule applied.
- Quality check: After any VFO change, confirm the account note is complete and the appropriate downstream process (retro or Demand Claim) has been triggered if required.

## Optimization Notes (Optional)

- This SOP and workflow use clear validation gates to reduce unnecessary VFO changes and mental friction.
- The simplified decision flow prioritizes early validation (COB Research Note support) before investing effort in complex updates.
- Text is focused on decision points and consequential actions rather than exhaustive rule lists.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **Coordination of Benefits**: Follow all applicable federal and state COB regulations and payer contracts.
- **Timely Filing**: VFO corrections must be completed within payer timely filing limits.
- **Audit Trail**: Every VFO change must be fully documented with rationale, COB research support, and sources.
- **Medicare Secondary Payer**: Strict adherence required; incorrect VFO can trigger overpayment recovery.
- **Retro Adjudication**: When forcing retro review, ensure all actions comply with payer and organizational policies.

> See `regulatory-foundations.md` for broader regulatory guidance.

## Related Documents

- **Companion Workflow**: [visit-filing-order-workflow.md](../workflows/visit-filing-order-workflow.md)
- **Registration Verification & Follow-Up SOP**: [registration.md](../sops/registration.md) — COB section
- Future: Demand Claim SOP / Workflow (planned)
- Organizational policies on Coordination of Benefits, timely filing, and retro adjudication

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 8, 2026| Initial version created as detailed expansion of COB filing order action from Registration SOP | Shaine Meister  |
| 1.1     | May 8, 2026| Refined Purpose, Scope, and Prerequisites for better alignment with Visit Filing Order vs Patient Filing Order concepts and framework principles. Improved documentation requirements | Shaine Meister  |
| 1.2     | May 8, 2026| Major revision to align Step-by-Step Procedure with simplified decision flow. Added critical validation gate (VFO Update Required + COB Research Note support), claims-generated branching logic, Primary Paid + Secondary billing path with explicit Demand Claim handoff, and stronger emphasis on consequential nature of VFO changes | Shaine Meister  |

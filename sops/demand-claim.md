# Demand Claim SOP

**Version**: 1.2  
**Last Updated**: May 9, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.

## Purpose

To provide a clear, simplified process for initiating Demand Claims following VFO updates and retro claims, ensuring correct next-payer billing while coordinating with credit review.

## Scope

**In Scope**  
- Processing Demand Claims after VFO update and retro claim
- Insurance payment pending credit review validation
- System actions for demand initiation and balance movement

**Out of Scope**  
- Primary payer research / COB determination
- Complex multi-payer coordination (escalate)
- Full credit / payment posting

## Roles & Responsibilities

| Role                  | Responsibility |
|-----------------------|----------------|
| Registration / COB Specialist | Validate payment pending review, initiate demand, document |
| Credit / Billing Team     | Handle payment review when pending |
| Supervisor            | Escalate complex cases |

## Prerequisites

- VFO has been updated
- Claim has been retro'd
- Insurance payment is pending credit review (critical gate)

## Step-by-Step Procedure

1. **Receive Trigger**  
   VFO Updated + Claim Retro'd.

2. **Check Insurance Payment Pending Credit Review**  
   - If **No** → Do Not Proceed. Make note and allow Credit Team to review.
   - If **Yes** → Proceed.

3. **Initiate Demand Claim**  
   Select appropriate payer if needed.
   Select appropriate output method (e.g., dummy printer or test mode).

4. **Distribute Payment & Move Balance**  
   Apply insurance payment.
   Move remaining balance to next responsible party.

5. **Document & Close**  
   Add account notes. Confirm END status.

## Quality Checks

- Payment pending credit review confirmed before any demand action
- Proper output method used
- Clear documentation of actions and rationale
- No premature balance movement

## Notes / Tips

- This process is typically triggered immediately after VFO updates that result in retro claims requiring secondary/demand billing.
- Coordinate closely with the Credit / Billing Team for any cases where payment review is still pending.
- Document all actions thoroughly in account notes to support audit trails and smooth handoffs.
- **Note on system-specific actions**: "Dummy Printer" (or equivalent test output method) is an example from the organization's billing system. Adapt this step to the equivalent function in your EHR, claims management, or billing platform for initiating the demand claim or simulated output. See optimization-standards.md for guidance on balancing specificity with portability.

## Optimization Notes

- Keep process extremely lean — single critical decision gate.
- Strong handoff to Credit Team when needed.
- Minimize steps to reduce mental friction.

## Regulatory / Compliance Notes

- Ensure actions maintain correct Coordination of Benefits sequencing.
- Document justification for demand to support audit readiness.
- Adhere to payer-specific demand requirements.

## Related Documents

- **Companion Workflow**: [demand-claim-workflow.md](../workflows/demand-claim-workflow.md)
- **Visit Filing Order SOP & Workflow**: [visit-filing-order.md](../sops/visit-filing-order.md) and [visit-filing-order-workflow.md](../workflows/visit-filing-order-workflow.md)

## Version History

| Version | Date       | Changes | Author |
|---------|------------|---------|--------|
| 1.0     | May 9, 2026 | Initial SOP created | Shaine Meister |
| 1.1     | May 9, 2026 | Simplified Step-by-Step and validation to exactly mirror the updated minimal Mermaid flow. | Shaine Meister |
| 1.2     | May 9, 2026 | Implemented Areas for Improvement and Recommendations: standardized Scope section with subheadings for template consistency, added Notes / Tips subsection with system-specific guidance, added full markdown links to related documents, updated Quality Checks and procedure for clarity, standardized Framework Alignment Check phrasing, updated Version and Last Updated. | Shaine Meister |
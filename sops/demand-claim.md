# Demand Claim SOP

**Version**: 1.0  
**Last Updated**: May 9, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4, 6, and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.

## Purpose

To provide a standardized, compliant process for initiating and processing **Demand Claims** to the secondary or tertiary payer after primary adjudication, ensuring correct sequencing in the Visit Filing Order without risking duplicate billing to the primary payer.

## In Scope

- Validating mandatory conditions for Demand Claim
- Preparing and forcing demand submission in the system
- Documentation and audit trail requirements
- Handoffs to related processes (e.g., retro adjudication)

## Out of Scope

- Initial claim submission
- Primary payer research or COB determination (handled in Registration / Visit Filing Order)
- Full denial management or appeals

## Roles & Responsibilities

| Role                  | Responsibility |
|-----------------------|----------------|
| Registration / COB Specialist | Validate conditions, prepare demand, document rationale |
| Billing / Claims Team     | Review complex cases, monitor adjudication, coordinate payer contact if needed |
| Supervisor / Lead         | Escalate complex or high-risk demands |

## Prerequisites – Mandatory Validations

**All three conditions must be confirmed before proceeding:**

1. Primary payer has already adjudicated the claim (payment posted or denial received and worked).
2. A Demand Claim is required to prevent duplicate submission to the primary (normal resubmit would risk rebilling primary).
3. Secondary (or next responsible party) has remaining liability per the current Visit Filing Order.

## Step-by-Step Procedure

1. **Receive Demand Trigger**  
   Triggered from Visit Filing Order update or work queue.

2. **Validate 3 Mandatory Conditions**  
   - Confirm primary adjudication complete.
   - Confirm demand is necessary to avoid duplicate primary billing.
   - Confirm next payer has liability.  
   If any condition fails → Refer back to Visit Filing Order Workflow. Stop.

3. **Verify Visit Filing Order**  
   Confirm Primary → Secondary → Tertiary sequence supports next-party billing.

4. **Prepare Demand Claim**  
   In the system, select the appropriate demand/force-next-payer option.

5. **Document Thoroughly**  
   Add detailed account note with:  
   - All three conditions met (with evidence)  
   - Specific COB / VFO rationale  
   - Date/time of action

6. **Submit Demand Claim**  
   Force submission to the next responsible party.

7. **Monitor & Close**  
   Track acknowledgement and adjudication.  
   Document outcome and advance balance per NRP rules.

## Quality Checks

- All three prerequisites documented before submission
- Clear audit trail in account notes
- No duplicate primary billing risk introduced
- Escalation performed for complex cases

## Optimization Notes

- Focus on validation gate to minimize errors and compliance risk.
- Keep notes concise but sufficient for audit.
- Use templates for common demand scenarios when available.

## Regulatory / Compliance Notes

- Demand claims must align with payer contracts and Coordination of Benefits rules.
- Maintain records supporting the justification for demand submission.
- Follow timely filing requirements for secondary payers.

## Related Documents

- **Companion Workflow**: `../workflows/demand-claim-workflow.md`
- Visit Filing Order SOP & Workflow (primary trigger)
- Registration SOP (COB section)

## Version History

| Version | Date       | Changes | Author |
|---------|------------|---------|--------|
| 1.0     | May 9, 2026 | Initial SOP created as companion to Demand Claim Workflow | Shaine Meister |
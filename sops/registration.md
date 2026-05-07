# Registration Verification & Follow-Up (Back-End)

**Version**: 1.2  
**Last Updated**: May 6, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This SOP is paired with a **Companion Workflow** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing).

## Purpose

To systematically review, verify, correct, and update patient registration information **after the point of service**. This back-end Revenue Cycle process identifies and resolves discrepancies discovered through work queues, claim edits, eligibility responses, and denial analysis. Accurate post-service registration follow-up reduces claim denials, accelerates clean claim submission, prevents timely filing issues, and supports compliance and optimal revenue capture.

## Scope

**In Scope**  
- Post-service review and correction of registrations via work queues, billing edits, and denial reports.
- Re-verification of insurance eligibility and benefits after the encounter.
- Research and correction of demographic, guarantor, subscriber, and insurance information.
- Follow-up on missing, expired, or invalid authorizations and referrals.
- Documentation of changes and coordination with billing, coding, and front-end teams.
- Identification of systemic registration issues for feedback and process improvement.

**Out of Scope**  
- Front-end / point-of-service patient registration and collection activities.
- Clinical documentation, coding, or charge capture.
- Final claim submission and payer follow-up (Billing team).
- Long-term collections or patient financial assistance applications (Patient Financial Services).

## Roles & Responsibilities

| Role                              | Responsibilities                                                                 |
|-----------------------------------|----------------------------------------------------------------------------------|
| Revenue Cycle Registration Specialist | Review work queues, verify/correct registration data, resolve edits and authorization issues |n| Registration Quality / Denial Prevention Analyst | Analyze trends, perform quality audits, identify systemic issues, provide feedback to front-end teams |
| Billing Coordinator / Specialist  | Flag registration-related claim edits and coordinate resolution with Registration team |
| Revenue Cycle Supervisor          | Oversee work queue management, escalation handling, and process improvement initiatives |

## Prerequisites

- Access to registration work queues, claim scrubber reports, denial management system, and eligibility verification tools
- Understanding of payer-specific registration requirements and common denial root causes
- Ability to research patient information across multiple sources (EHR, payer portals, patient statements, prior accounts)
- Completed training on HIPAA, account documentation standards, and timely filing requirements

## Step-by-Step Procedure

Use clear, numbered steps. Keep language concise and focused on the essential action. Include decision points where relevant. This process occurs **after** the patient encounter and point-of-service registration, typically triggered by claim denials, billing edits, or work queue items.

1. **Triage Incoming Denial, Edit, or Work Queue Item**  
   - Review the denial code, edit reason, or work queue item.  
   - Identify whether the issue appears registration-related (common examples: eligibility issues, subscriber not found, invalid insurance, demographic mismatches, missing guarantor, authorization problems).  
   - **Decision point**: Is this primarily a registration issue? → If No, hand off to Billing, Coding, or Denials Management team. If Yes, proceed to analysis.  

2. **Analyze Root Cause and Denial Code**  
   - Examine the specific denial code and accompanying remarks.  
   - Determine the likely root cause category (Eligibility, Demographic/Guarantor error, Authorization/Referral issue, Subscriber mismatch, etc.).  
   - Pull the original registration information and compare against current payer data or claim details.  

3. **Research Registration Data**  
   - Investigate using multiple sources: original insurance card/registration documents, prior accounts, payer portals, patient contact (if appropriate), and third-party databases.  
   - Verify current vs. date-of-service information.  

4. **Perform Post-Service Eligibility Re-Verification**  
   - Re-run eligibility and benefits verification for the exact date of service.  
   - Confirm coverage status, subscriber details, and benefit alignment at the time of service.  
   - **Decision point**: Eligibility issues confirmed → proceed to correction (Step 5). If no eligibility issue found, re-evaluate if root cause is elsewhere (e.g., authorization).  

5. **Correct Registration Information**  
   - Update inaccurate or incomplete fields (demographics, guarantor, subscriber ID, group number, relationship to insured, etc.).  
   - Apply corrections in the system with clear, detailed audit notes explaining what was changed and the source used.  

6. **Address Related Authorization or Referral Issues**  
   - Verify authorization status for the services rendered.  
   - Attempt to obtain retro-authorization or update authorization information when permitted by payer policy.  
   - Attach supporting documentation.  
   - **Decision point**: Authorization cannot be resolved → escalate to supervisor or Denials Management for appeal consideration.  

7. **Document All Actions and Rationale**  
   - Record detailed notes on the account: what was researched, what was corrected, why, and any supporting evidence.  
   - Flag the account for re-scrubbing or re-submission.  

8. **Release for Reprocessing or Handoff**  
   - Release corrected accounts back into the billing/claims workflow for reprocessing.  
   - For complex or high-impact cases, prepare summary for Denials Management or Appeals team.  
   - Communicate systemic front-end issues to the appropriate supervisor or Quality team.  

9. **Monitor Trends and Drive Continuous Improvement**  
   - Track recurring registration error types, specific payers, or originating locations/departments.  
   - Summarize findings periodically and provide actionable feedback to front-end Registration teams and leadership.  
   - Recommend process, training, or system enhancements to reduce future occurrences.

**Notes / Tips** (optional)  
- Always document the "before" state and the source of corrections to maintain a strong audit trail.  
- Prioritize work by timely filing deadlines and financial impact.  
- Use compliant patient and payer communication scripts when outreach is required.

## Quality Checks & Common Pitfalls

- Always verify that corrections align with the actual date of service and services billed.  
- Double-check subscriber vs. patient relationship and policy numbers after any update.  
- Common pitfall: Making corrections without sufficient documentation or source citation → audit risk and downstream confusion.  
- Common pitfall: Failing to re-verify eligibility after corrections → claim may deny again on re-submission.  
- Common pitfall: Treating symptoms instead of root cause → recurring work queue volume from the same front-end issues.

## Optimization Notes (Optional)

- Designed around real-world A/R triggers (denials and edits) with clear decision points to reduce hesitation and rework.  
- Text volume kept concise while preserving necessary research, documentation, and escalation steps.  
- Supports predictable navigation through a logical sequence from triage to resolution and feedback.  
- Enables back-end teams to focus effort on high-impact registration issues that directly affect clean claim rates and timely reimbursement.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **Timely Filing**: All corrections and re-submissions must occur within payer timely filing limits.  
- **Audit Trail**: Every change to registration data must include date/time, user ID, before/after values, and rationale.  
- **HIPAA**: Protect all PHI during research, correction, and any patient or payer outreach.  
- **Authorization Compliance**: Retro-authorizations should only be pursued when permitted; document medical necessity and payer-specific rules.  
- **Billing Integrity**: Accurate registration data is foundational to compliant claims submission.

> See `regulatory-foundations.md` for the broader regulatory integration approach used in this framework.

## Related Documents

- **Companion Workflow**: [registration-workflow.md](../workflows/registration-workflow.md) — Dynamic visual flowchart for real-world registration denial and edit scenarios.  
- Denial Management SOP (planned)  
- Visit Filing Order SOP (planned)  
- Organizational timely filing and authorization policies

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial front-end focused version created as model                      | Shaine Meister  |\n| 1.1     | May 6, 2026| Revised to back-end Revenue Cycle focus (post-service verification and follow-up) | Shaine Meister  |\n| 1.2     | May 6, 2026| Refined Step-by-Step Procedure for real-world A/R follow-up scenarios triggered by claim denials and edits. Added explicit triage, root cause analysis, and decision points aligned with typical denial workflows. | Shaine Meister  |
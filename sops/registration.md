# Registration Verification & Follow-Up (Back-End)

**Version**: 1.1  
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
| Revenue Cycle Registration Specialist | Review work queues, verify/correct registration data, resolve edits and authorization issues |
| Registration Quality / Denial Prevention Analyst | Analyze trends, perform quality audits, identify systemic issues, provide feedback to front-end teams |
| Billing Coordinator / Specialist  | Flag registration-related claim edits and coordinate resolution with Registration team |
| Revenue Cycle Supervisor          | Oversee work queue management, escalation handling, and process improvement initiatives |

## Prerequisites

- Access to registration work queues, claim scrubber reports, denial management system, and eligibility verification tools
- Understanding of payer-specific registration requirements and common denial root causes
- Ability to research patient information across multiple sources (EHR, payer portals, patient statements, prior accounts)
- Completed training on HIPAA, account documentation standards, and timely filing requirements

## Step-by-Step Procedure

Use clear, numbered steps. Keep language concise and focused on the essential action. Include decision points where relevant. This process occurs **after** the patient encounter and point-of-service registration.

1. **Review Registration Work Queues and Edits**  
   - Access and prioritize registration-related work queues, claim edits, and denial reports flagged for registration issues.  
   - Sort by aging, dollar amount, or denial reason as appropriate.  
   - **Decision point**: High-volume or high-dollar items → prioritize; recurring issues → flag for trend analysis (Step 8).  

2. **Identify and Analyze Discrepancies**  
   - Review claim scrubber messages, eligibility responses, and denial codes related to demographics, insurance, guarantor, or authorization.  
   - Compare current account information against source documents (insurance cards, prior accounts, patient statements, payer portals).  

3. **Perform Post-Service Eligibility Re-Verification**  
   - Re-run eligibility and benefits verification for the date of service.  
   - Confirm coverage was active, subscriber information is correct, and benefits align with the services rendered.  
   - **Decision point**: Eligibility issues or coverage gaps identified → proceed to research and correction (Step 4) and document impact on claim.  

4. **Research and Correct Registration Information**  
   - Investigate and update inaccurate or incomplete demographics, guarantor details, subscriber ID, group number, or relationship to insured.  
   - Use multiple sources (patient contact, payer portals, prior encounters, third-party databases) as needed.  
   - Make corrections in the registration system with clear audit trail notes.  

5. **Address Authorization and Referral Issues**  
   - Verify authorization status for services rendered.  
   - Obtain retro-authorizations or referrals when possible and permitted by payer.  
   - Update authorization fields and attach supporting documentation.  
   - **Decision point**: Authorization cannot be obtained or is denied → escalate to supervisor or denial management team; document thoroughly for appeal potential.  

6. **Update Account and Document All Changes**  
   - Apply all corrections to the patient account.  
   - Add detailed notes explaining what was changed, why, and any supporting research.  
   - Flag the account for re-scrubbing or re-submission if it was previously held or denied.  

7. **Handoff or Escalate as Needed**  
   - Release corrected accounts back to billing/claims workflow.  
   - Escalate complex cases (e.g., coverage disputes, large dollar impact, recurring payer issues) to supervisor or specialized team.  
   - Communicate systemic front-end issues to Registration Supervisor or Quality team for training/ process improvement.  

8. **Monitor Trends and Drive Improvement**  
   - Track recurring registration error types, payers, or front-end locations.  
   - Summarize findings and provide actionable feedback to front-end teams or leadership.  
   - Recommend updates to front-end processes, training, or system edits when patterns emerge.

**Notes / Tips** (optional)  
- Always document the "before" state and the source used for corrections to maintain a clear audit trail.  
- Prioritize accounts based on timely filing deadlines and dollar impact.  
- When contacting patients or payers, use compliant scripting and document all outreach attempts.

## Quality Checks & Common Pitfalls

- Verify that corrections align with the actual date of service and services rendered.  
- Double-check subscriber vs. patient relationship and policy numbers after updates.  
- Common pitfall: Making changes without sufficient documentation → creates audit risk and confusion for downstream teams.  
- Common pitfall: Failing to re-verify eligibility after corrections → claim may still deny.  
- Common pitfall: Not escalating recurring issues → same errors continue to generate work queue volume.

## Optimization Notes (Optional)

- Designed for predictable navigation: clear sequencing from queue review through research, correction, and handoff.  
- Decision points and escalation paths are explicit to reduce hesitation and rework.  
- Text is minimized while preserving necessary regulatory and documentation standards.  
- Supports back-end workflow efficiency by focusing on high-impact registration issues that affect clean claim rates.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **Timely Filing**: Corrections must be completed within payer timely filing limits to protect revenue.  
- **Audit Trail**: All changes to registration data must be documented with date, time, user, and reason to support internal and external audits.  
- **HIPAA**: Protect PHI during research and when contacting patients or payers.  
- **Authorization Compliance**: Only obtain retro-authorizations when permitted; document medical necessity and payer requirements.  
- **Billing Integrity**: Accurate registration data is foundational to compliant claims and avoidance of false claims risk.

> See `regulatory-foundations.md` for the broader regulatory integration approach used in this framework.

## Related Documents

- **Companion Workflow**: [registration-workflow.md](../workflows/registration-workflow.md) — Simplified visual quick-reference for back-end registration follow-up activities.  
- Denial Management SOP (planned)  
- Visit Filing Order SOP (planned)  
- Organizational timely filing and authorization policies

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial front-end focused version created as model                      | Shaine Meister  |
| 1.1     | May 6, 2026| Revised to back-end Revenue Cycle focus: post-service verification, work queue management, eligibility re-verification, authorization follow-up, and trend identification. Tailored for back-end teams reviewing registration issues after point-of-service. | Shaine Meister  |
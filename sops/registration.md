# Registration Verification & Follow-Up (Back-End)

**Version**: 1.3  
**Last Updated**: May 6, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This SOP is paired with a **Companion Workflow** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing). The workflow is now organized into three focused sections (Eligibility, COB, and Authorization) for easier reference.

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

Use clear, numbered steps. Keep language concise and focused on the essential action. Include decision points where relevant. This process occurs **after** the patient encounter and point-of-service registration, typically triggered by claim denials, billing edits, or work queue items.

The workflow is organized into three focused categories. The procedures below follow the same structure for easier cross-reference with the companion workflow.

### 1. Triage and Root Cause Analysis (All Categories)

1. **Triage Incoming Denial, Edit, or Work Queue Item**  
   - Review the denial code, edit reason, or work queue item.  
   - Identify whether the issue appears registration-related.  
   - **Decision point**: Is this primarily a registration issue? → If No, hand off to Billing, Coding, or Denials Management team.

2. **Analyze Root Cause and Identify Category**  
   - Determine the primary category: **Eligibility**, **Coordination of Benefits (COB)**, or **Authorization**.  
   - Proceed to the relevant section below.

### 2. Eligibility Follow-up Procedures

3. **Identify Eligibility Issue Type**  
   - Determine the specific scenario: Patient Active/Coverage Issue, Demographic/Registration Error, Newborn 30-day Grace Period, or Patient Involvement Needed.

4. **Handle Specific Eligibility Scenarios**  
   - **Patient Active / Coverage Issue**: Re-verify eligibility and update registration data.  
   - **Demographic / Registration Error**: Correct demographics and re-verify eligibility.  
   - **Newborn Scenario (30-day Grace Period)**: Send notification letter per regulatory/courtesy requirements.  
   - **Patient Involvement Needed**: Send letter to patient/guarantor. For Medicare or Medicaid payers, complete 3 contact attempts before moving balance to self-pay (if attempts are exhausted).

5. **Document and Resubmit**  
   - Document all changes and rationale.  
   - Resubmit claim or continue follow-up as appropriate.

### 3. Coordination of Benefits (COB) Follow-up Procedures

6. **Execute COB Resolution Path**  
   - Choose the appropriate action based on the situation:  
     - Update registration and/or fix filing order (internal correction).  
     - Contact payer to verify information or request claim reprocessing.  
     - Send patient/guarantor letter when COB information needs to be updated by the patient.

7. **Document and Resubmit**  
   - Document all changes and rationale.  
   - Resubmit claim or continue follow-up.

### 4. Authorization Follow-up Procedures

8. **Evaluate Prior Authorization Status**  
   - Determine if valid prior authorization was obtained before service.  
   - **Decision point**: Was prior authorization obtained and valid? → If Yes, correct claim by adding authorization details and resubmit.

9. **Handle Retroactive Authorization or Appeals**  
   - If no valid prior authorization: Determine if retroactive authorization can be requested.  
   - If retroactive PA is possible → Submit request to payer.  
   - If retroactive PA is not possible or denied → Prepare and file formal appeal (if within timely filing/appeal deadline).

10. **Determine Final Account Resolution**  
    - If appeal is filed or not possible: Assess patient responsibility.  
    - Move balance to self-pay with proper documentation or apply appropriate write-off.  
    - Document & apply account note for all actions.

### 5. Documentation, Handoff, and Continuous Improvement (All Categories)

11. **Document All Actions and Rationale**  
    - Record detailed notes including before/after values, sources used, and rationale.  
    - Flag account for re-scrubbing or re-submission.

12. **Release or Handoff**  
    - Release corrected accounts for reprocessing.  
    - Escalate complex or high-impact cases to supervisor or Denials Management.

13. **Monitor Trends and Drive Improvement**  
    - Track recurring issues by category, payer, or location.  
    - Provide feedback to front-end teams and leadership.

**Notes / Tips** (optional)  
- Always maintain a clear audit trail by documenting the “before” state and sources used for corrections.  
- Prioritize work by timely filing deadlines and financial impact.  
- Use compliant scripting for all patient and payer outreach.

## Key Decision Points

- Triage: Is this primarily a registration issue?  
- Root cause category: Eligibility, COB, or Authorization?  
- **Eligibility**: Specific scenario type (coverage, demographic, newborn, patient involvement) and payer type (Medicare/Medicaid contact rules).  
- **COB**: Which of the three resolution paths is most appropriate?  
- **Authorization**: Was valid PA obtained? Can retro be requested? Within timely filing/appeal deadlines? Patient responsibility vs. write-off.  
- Recurring issues or high-impact cases → Escalate and report trends.

## Quality Checks & Common Pitfalls

- Verify corrections align with date of service and billed services.  
- Double-check subscriber vs. patient relationship and policy numbers.  
- Common pitfall: Insufficient documentation or missing source citation → audit risk.  
- Common pitfall: Failing to re-verify eligibility after corrections.  
- Common pitfall: Not following payer-specific rules (e.g., Medicare/Medicaid contact attempts).

## Optimization Notes (Optional)

- The SOP and companion workflow are now aligned around three clear categories (Eligibility, COB, Authorization) for faster navigation and decision-making.  
- Designed around real-world A/R denial triggers with explicit decision points.  
- Supports predictable navigation while preserving necessary regulatory and documentation standards.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **Timely Filing & Appeals**: All corrections, retro PA requests, and appeals must occur within payer deadlines.  
- **Audit Trail**: Every change must include date/time, user, before/after values, and rationale.  
- **HIPAA**: Protect PHI during all research and outreach.  
- **Authorization Compliance**: Retro-authorizations only when permitted; document thoroughly.  
- **Newborn Grace Periods & Medicare/Medicaid Rules**: Follow specific regulatory requirements for notification and contact attempts.

> See `regulatory-foundations.md` for the broader regulatory integration approach used in this framework.

## Related Documents

- **Companion Workflow**: [registration-workflow.md](../workflows/registration-workflow.md) — Now organized into three focused sections:  
  - Eligibility (with scenario-specific paths including newborn grace period and Medicare/Medicaid contact rules)  
  - Coordination of Benefits (COB) with three resolution outcomes  
  - Authorization (detailed decision tree including retro PA, appeals, and final resolution options)  
- Denial Management SOP (planned)  
- Visit Filing Order SOP (planned)  
- Organizational timely filing, authorization, and Medicare/Medicaid policies

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial front-end focused version created as model                      | Shaine Meister  |
| 1.1     | May 6, 2026| Revised to back-end Revenue Cycle focus (post-service verification and follow-up) | Shaine Meister  |
| 1.2     | May 6, 2026| Refined Step-by-Step for real-world A/R denial-driven scenarios         | Shaine Meister  |
| 1.3     | May 6, 2026| Restructured Step-by-Step Procedure into category-specific sections (Eligibility, COB, Authorization) to mirror the modular structure of the companion workflow. Added granular scenarios (newborn grace period, Medicare/Medicaid 3-contact rule, detailed authorization decision tree). Updated Key Decision Points, Quality Checks, Related Documents, and Version History for alignment. | Shaine Meister  |
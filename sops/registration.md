# Registration Verification & Follow-Up (Back-End)

**Version**: 1.6  
**Last Updated**: May 6, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This SOP is paired with a **Companion Workflow** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing). The workflow is organized into three focused sections (Eligibility, COB, and Authorization) for easier reference.

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

| Role                                      | Responsibilities                                                                 |
|-------------------------------------------|----------------------------------------------------------------------------------|
| Revenue Cycle Registration Specialist     | Review work queues, verify/correct registration data, resolve edits and authorization issues |\n| Registration Quality / Denial Prevention Analyst | Analyze trends, perform quality audits, identify systemic issues, provide feedback to front-end teams |\n| Billing Coordinator / Specialist          | Flag registration-related claim edits and coordinate resolution with Registration team |\n| Revenue Cycle Supervisor                  | Oversee work queue management, escalation handling, and process improvement initiatives |\n
## Prerequisites

- Access to registration work queues, claim scrubber reports, denial management system, and eligibility verification tools
- Understanding of payer-specific registration requirements and common denial root causes
- Ability to research patient information across multiple sources (EHR, payer portals, patient statements, prior accounts)
- Completed training on HIPAA, account documentation standards, and timely filing requirements

## Step-by-Step Procedure

This section follows the structure of the companion workflow. After initial triage, issues are classified into one of three categories: **Eligibility**, **Coordination of Benefits (COB)**, or **Authorization**.

### Triage (Common Starting Point)

**Triage determines whether the issue is registration-related and classifies it into one of the following categories:**

- **Eligibility**
- **Coordination of Benefits (COB)**
- **Authorization**

1. **Triage the Denial, Edit, or Work Queue Item**  
   - Review the denial code or edit reason.  
   - Determine if the issue is primarily registration-related.  
   - **Decision**: If not registration-related → hand off to Billing, Coding, or Denials team.

2. **Classify into Primary Category**  
   - Assign the issue to **Eligibility**, **COB**, or **Authorization**.  
   - Proceed to the corresponding section below.

---

### Eligibility Procedures

**This section applies when Triage has classified the issue as Eligibility.**

3. **Determine the Specific Eligibility Scenario**  
   - Identify which type applies:  
     - Patient Active / Coverage Issue  
     - Demographic or Registration Error  
     - Newborn 30-day Grace Period  
     - Patient Involvement Needed

4. **Resolve According to Scenario**  
   - **Patient Active / Coverage Issue**: Re-verify eligibility and update registration.  
   - **Demographic / Registration Error**: Correct demographics and re-verify eligibility.  
   - **Newborn 30-day Grace Period**: Send required notification letter.  
   - **Patient Involvement Needed**: Send letter to patient/guarantor. For Medicare or Medicaid payers, complete up to 3 contact attempts before moving balance to self-pay.

5. **Document and Advance the Account**  
   - Record changes with clear rationale.  
   - Resubmit the claim or continue follow-up.

---

### Coordination of Benefits (COB) Procedures

**This section applies when Triage has classified the issue as Coordination of Benefits (COB).**

6. **Select and Execute the Appropriate COB Action**  
   - Choose one of the following based on the situation:  
     - Update registration and/or correct filing order (internal fix).  
     - Contact the payer to verify information or request reprocessing.  
     - Send a letter to the patient/guarantor requesting COB update.

7. **Document and Advance the Account**  
   - Record the action taken and rationale.  
   - Resubmit the claim or continue follow-up.

---

### Authorization Procedures

**This section applies when Triage has classified the issue as Authorization.**

8. **Check Prior Authorization Validity**  
   - Determine whether valid prior authorization was obtained before the date of service.  
   - **Decision**: If Yes → Add authorization details to the claim and resubmit.

9. **Handle Cases Without Valid Prior Authorization**  
   - Check if retroactive authorization can be requested.  
     - If Yes → Submit retroactive PA request to the payer.  
     - If No or denied → Prepare formal appeal (only if within timely filing/appeal deadline).

10. **Determine Final Account Resolution**  
    - If within deadline: File appeal if appropriate.  
    - Assess patient responsibility.  
    - Move balance to self-pay with documentation **or** apply appropriate write-off.  
    - Add final account note documenting all actions.

---

### Common Closing Steps

11. **Final Documentation**  
    - Record all changes with before/after details and supporting sources.  
    - Flag the account for re-scrubbing or re-submission.

12. **Handoff or Escalate**  
    - Release the account for reprocessing.  
    - Escalate complex or high-dollar cases as needed.

13. **Monitor for Trends**  
    - Track recurring issues by category, payer, or location.  
    - Provide feedback to front-end teams for process improvement.

**Notes / Tips**  
- Maintain a strong audit trail by always documenting the source of corrections.  
- Prioritize accounts based on timely filing deadlines and financial impact.  
- Use compliant scripts for all patient and payer communication.

## Key Decision Points

- Triage: Is this a registration-related issue?  
- Category identification: Eligibility, COB, or Authorization?  
- **Eligibility**: Which specific scenario applies, and is it a Medicare/Medicaid case requiring 3 contact attempts?  
- **COB**: Which of the three actions is most appropriate?  
- **Authorization**: Was valid PA obtained? Can retro be requested? Within appeal deadline? Patient responsibility vs. write-off.  
- Recurring issues → Escalate and report trends.

## Quality Checks & Common Pitfalls

- Confirm all corrections match the date of service and billed services.  
- Verify subscriber vs. patient relationship after any updates.  
- Common pitfall: Incomplete documentation or missing source references.  
- Common pitfall: Skipping re-verification of eligibility after corrections.  
- Common pitfall: Ignoring payer-specific rules (especially Medicare/Medicaid contact requirements).

## Optimization Notes (Optional)

- The SOP and workflow are aligned around three distinct categories for faster reference and decision-making.  
- Clear separation between Eligibility, COB, and Authorization reduces cognitive load when working specific denial types.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **Timely Filing & Appeals**: Respect all payer deadlines for corrections, retro PA requests, and appeals.  
- **Audit Trail**: Every change must be fully documented with date, time, user, and rationale.  
- **HIPAA**: Protect PHI during research and all outreach.  
- **Authorization Rules**: Only pursue retro-authorization when permitted by payer policy.  
- **Newborn & Medicare/Medicaid Specific Rules**: Follow required notification and contact attempt protocols.

> See `regulatory-foundations.md` for broader regulatory guidance.

## Related Documents

- **Companion Workflow**: [registration-workflow.md](../workflows/registration-workflow.md) — Organized into three independent sections:  
  - Eligibility (scenario-specific paths)  
  - Coordination of Benefits (COB)  
  - Authorization (detailed decision tree)  
- Denial Management SOP (planned)  
- Visit Filing Order SOP (planned)  
- Organizational policies on timely filing, authorization, and Medicare/Medicaid requirements

## Version History

| Version | Date       | Changes                                                                 | Author          |
|---------|------------|-------------------------------------------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial front-end focused version created as model                      | Shaine Meister  |
| 1.1     | May 6, 2026| Revised to back-end Revenue Cycle focus                                 | Shaine Meister  |
| 1.2     | May 6, 2026| Refined for real-world A/R denial-driven scenarios                      | Shaine Meister  |
| 1.3     | May 6, 2026| Restructured into category-specific sections to mirror workflow         | Shaine Meister  |
| 1.4     | May 6, 2026| Simplified and visually separated the three category procedures         | Shaine Meister  |
| 1.5     | May 6, 2026| Fixed Roles & Responsibilities table. Made Eligibility, COB, and Authorization explicit sub-categories under Triage. | Shaine Meister  |
| 1.6     | May 6, 2026| Added linking sentences at the top of each category section to reinforce Triage as the parent process. Lightly tightened Authorization section for improved usability while preserving all key decision logic. | Shaine Meister  |
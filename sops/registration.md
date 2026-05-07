# Patient Registration

**Version**: 1.0  
**Last Updated**: May 6, 2026  
**Owner**: Shaine Meister  
**Status**: Draft

> **Framework Alignment Check**  
> Before finalizing this SOP, evaluate it against the principles in `core-principles.md` (especially Principles 1–4 and 7). Apply modular structure guidance from `modular-structure.md`, integrate regulatory foundations appropriately from `regulatory-foundations.md`, and optimize for predictable navigation with minimal mental friction per `optimization-standards.md`.  
> This SOP is paired with a **Companion Workflow** for day-to-day quick reference (see `modular-structure.md` – Recommended Design Patterns: SOP + Companion Workflow Pairing).

## Purpose

Ensure accurate, complete, and compliant capture of patient demographics, insurance information, consents, and financial responsibility at the initial point of service. This foundational process reduces downstream claim denials, rework, bad debt, and compliance risk while supporting a positive patient experience and optimal revenue capture.

## Scope

**In Scope**  
- All patient registrations including scheduled outpatient, inpatient pre-admission, emergency department, walk-in, and recurring visits.
- Demographic collection and verification, insurance eligibility checks, consent processes, financial responsibility estimation, and initial payment collection or arrangement.

**Out of Scope**  
- Clinical assessment, diagnosis, or treatment documentation (clinical teams).
- Final medical coding and claim submission (Revenue Cycle – Billing).
- Ongoing account follow-up, appeals, or collections (Patient Financial Services).

## Roles & Responsibilities

| Role                          | Responsibilities                                                                 |
|-------------------------------|----------------------------------------------------------------------------------|
| Patient Access Registrar      | Perform registration, verify demographics/insurance, obtain consents, generate estimates, collect payments or set up arrangements |
| Registration Supervisor / Lead| Oversee process accuracy and compliance, handle complex escalations, conduct quality reviews |
| Financial Counselor           | Manage complex estimates, payment plans, financial assistance screening, and hardship cases |
| Clinical / Nursing Staff      | Provide limited support for urgent/ED registrations and clinical context when needed |

## Prerequisites

- Active access to registration/EHR system and real-time eligibility tools
- Completion of required training (HIPAA/privacy, customer service, system navigation, financial assistance screening)
- Access to current payer fee schedules, contracts, and organizational financial assistance policy
- Patient communication scripts and estimate tools ready

## Step-by-Step Procedure

Use clear, numbered steps. Keep language concise and focused on the essential action. Include decision points where relevant.

1. **Prepare for Arrival (Pre-Registration)**  
   - Review upcoming appointments and pre-verify insurance information where possible.  
   - Flag any missing data or potential issues for quick resolution on arrival.  

2. **Greet & Confirm Patient Identity**  
   - Use two patient identifiers (e.g., full name + date of birth or government-issued photo ID).  
   - Confirm appointment details and reason for visit.  

3. **Collect or Update Demographics**  
   - Verify or enter current address, phone number(s), email, emergency contact, and guarantor information.  
   - **Decision point**: If patient is a minor, incapacitated, or has a legal guardian/power of attorney → collect and document appropriate legal documentation.  

4. **Insurance Verification & Eligibility**  
   - Enter or confirm insurance details (subscriber ID, group number, relationship to insured).  
   - Perform real-time eligibility and benefits check if the tool is available.  
   - **Decision point**: If eligibility returns issues, no active coverage, or high patient responsibility → proceed to Step 6 (Financial Responsibility) and consider escalation.  

5. **Obtain Required Consents & Authorizations**  
   - Present and secure signatures/acknowledgments for:  
     - Consent for treatment / services  
     - HIPAA Notice of Privacy Practices  
     - Assignment of benefits and release of information  
   - For Emergency Department registrations: Confirm EMTALA requirements are met (medical screening exam offered regardless of ability to pay).  

6. **Determine & Address Financial Responsibility**  
   - Generate and explain an estimate of the patient’s out-of-pocket responsibility (copay, deductible, coinsurance).  
   - Screen for financial assistance eligibility per organizational policy.  
   - Collect payment, set up payment plan, or document arrangement.  
   - **Decision point**: If patient expresses financial hardship or requests assistance → immediately escalate to Financial Counselor.  

7. **Complete Registration & Facilitate Next Steps**  
   - Print or provide patient with relevant documents (ID band, instructions, estimate summary, wayfinding).  
   - Direct patient to the appropriate clinical area or next location.  
   - Add any special notes, alerts, or follow-up items in the system for downstream teams.  

**Notes / Tips** (optional)  
- Prioritize accuracy on high-impact fields that drive claims and statements (subscriber ID, group number, guarantor relationship, current contact information).  
- Use plain, patient-friendly language during explanations.  
- Leverage system validation rules, auto-population, and dropdowns to reduce manual entry errors.

## Quality Checks & Common Pitfalls

- Always compare insurance card details against entered data (common errors: transposed numbers, outdated cards).  
- Confirm guarantor relationship and correct subscriber information.  
- Verify address and phone numbers — these are critical for statements and collections.  
- Common pitfall: Skipping or rushing financial screening on high-deductible health plans → leads to downstream bad debt and rework.  
- Common pitfall: Incomplete consent documentation → compliance and billing risk.

## Optimization Notes (Optional)

- Designed for predictable navigation with minimal mental friction: clear numbered steps, visible decision points, and logical sequencing that matches real-world workflow.  
- Text volume minimized while preserving necessary regulatory context and quality safeguards.  
- Escalation paths are explicit to reduce hesitation or rework.  
- Supports intuitive flow by handling the most common happy path first, then branching only when needed.

> See `optimization-standards.md` for the optimization approach used across this framework.

## Regulatory / Compliance Notes

- **HIPAA / Privacy**: Protect all protected health information (PHI) during collection and discussion. Provide and document acknowledgment of the Notice of Privacy Practices.  
- **Financial Assistance**: Screen patients for eligibility per organizational policy and applicable IRS/ACA requirements (especially for nonprofit hospitals).  
- **EMTALA (ED only)**: Medical screening examination must be provided regardless of the patient’s ability to pay or insurance status.  
- **Consent**: Must be informed, voluntary, and properly documented.  
- **Billing Integrity**: Accurate demographic and insurance capture is foundational to compliant claims.

> See `regulatory-foundations.md` for the broader regulatory integration approach used in this framework.

## Related Documents

- **Companion Workflow**: [registration-workflow.md](../workflows/registration-workflow.md) — The simplified visual quick-reference version for daily use.  
- Visit Filing Order SOP (planned)  
- Organizational Financial Assistance Policy  
- Payer-specific eligibility and authorization guidelines

## Version History

| Version | Date       | Changes                              | Author          |
|---------|------------|--------------------------------------|-----------------|
| 1.0     | May 6, 2026| Initial version created as the model SOP for the framework | Shaine Meister  |
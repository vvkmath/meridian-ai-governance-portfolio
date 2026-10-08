# AI Governance Portfolio: Meridian Automated Loan Underwriting System

**Author:** Vivek Korikanthimath · **Role:** AI Governance, Risk & Compliance Practitioner (portfolio project) · **Platform:** VerifyWise · **Date:** October 2026

> Meridian Financial Services is a fictional mid-sized lender. All organizations, systems, vendors and data in this project are fictional and used for educational purposes only.

## The governance question

**Should Meridian Financial Services approve production deployment of a 94% automated AI loan underwriting system?**

**Recommendation: Proceed with conditions.** Meridian should not approve unrestricted production deployment until the required fairness, explainability, human oversight, vendor, monitoring, privacy/security and governance controls are completed and evidenced. A limited, controlled pilot may follow once those conditions are met.

## The system

| | |
|---|---|
| System | Meridian Automated Loan Underwriting System |
| Vendor model | CrediSure Credit Decision Engine v2.3 (CrediSure AI) |
| Purpose | Faster, more consistent small business loan decisions |
| Outputs | Auto-approve · Auto-deny · Route to manual review |
| Automation | ~94% of applications decided automatically; ~6% reach a human |
| Classification | **High risk**: affects access to credit (EU AI Act Annex III, point 5) |

## Frameworks applied

| Framework | Used for |
|---|---|
| **EU AI Act** | High-risk classification, Fundamental Rights Impact Assessment (FRIA), human oversight, logging, explanations to affected persons, appeals, CE marking steps |
| **NIST AI RMF** | GOVERN (oversight roles), MAP (system context), MEASURE (evaluation evidence), MANAGE (risk prioritization and treatment) |
| **ISO/IEC 42001** | AIMS scope (4.3), roles (5.3), risk assessment (6.1.2), risk treatment (6.1.3), management review (9.3), Annex A.5, A.8, A.11 |

## Top risks

| Risk | Current level |
|---|---|
| Lack of meaningful human oversight | Very high |
| Discriminatory lending outcomes | Very high |
| Proxy bias through credit and business variables | High |
| Weak explainability and incomplete reason codes | High |
| Inaccurate automated denials | High |
| Accountability gaps in third-party AI deployment | High |

**Biggest concern:** human oversight. Only about 6% of applications reach a person, and combined with proxy-bias risk, applicants could be unfairly denied credit without a clear explanation or a realistic way to appeal.

## Conditions before production

1. Fairness and disparate impact testing
2. Denial reason code validation
3. Human review triggers and a working appeal process
4. Vendor documentation review (CrediSure AI)
5. Security and privacy review
6. Monitoring thresholds and incident escalation
7. Governance committee and executive approval

## Screenshots

### 1. Use case
![Use case](screenshots/01_use_case.png)
This screenshot shows the Meridian Automated Loan Underwriting System registered as a high-risk AI use case in VerifyWise, with applicable frameworks, approval workflow, and pre-production governance status.

### 2. Dataset
![Dataset](screenshots/02_dataset.png)
This screenshot shows the Small Business Loan Underwriting Dataset registered in VerifyWise, including data purpose, source, format, PII status, known bias concerns, mitigation approach, and connection to the CrediSure Credit Decision Engine and Meridian Automated Loan Underwriting System.

### 3. Risk register
![Risks](screenshots/03_risks.png)
This screenshot shows the six required risks for the Meridian Automated Loan Underwriting System, including risks imported from IBM AI Risk Database, MIT AI Risk Repository, and manually created custom risks.

### 4. Training registry
![Training](screenshots/04_training.png)
This screenshot shows the AI training registry record for the Meridian Automated Loan Underwriting System, documenting planned governance training for stakeholders responsible for compliance, model risk, credit risk, human oversight, vendor risk, and executive approval.

### 5. Vendor
![Vendor](screenshots/05_vendor.png)
This screenshot shows the CrediSure AI vendor record in VerifyWise, documenting the third-party provider responsible for the credit decisioning model used by the Meridian Automated Loan Underwriting System.

### 6. Policies
![Policies](screenshots/06_policies.png)
This screenshot shows the three core organizational AI policies selected for the Meridian Automated Loan Underwriting System: AI Governance Policy, AI Risk Management Policy, and AI Vendor Risk Policy. These policies establish the minimum governance, risk management, and third-party oversight structure for the high-risk AI portfolio.

### 7. ISO/IEC 42001 Annex controls
![ISO 42001 annexes](screenshots/07_iso_annexes.png)
This screenshot shows the three must-have ISO 42001 Annex controls completed for the Meridian Automated Loan Underwriting System: AI governance framework, AI system lifecycle management, and third-party AI risk management.

### 8. NIST AI RMF
![NIST AI RMF](screenshots/08_nist.png)
This screenshot shows the four must-have NIST AI RMF subfunctions completed for the Meridian Automated Loan Underwriting System, covering human-AI oversight roles, system context, evaluation evidence, and prioritized AI risk treatment.

### 9. EU AI Act FRIA
![FRIA](screenshots/09_fria.png)
This screenshot shows the EU AI Act FRIA summary for the Meridian Automated Loan Underwriting System, including stakeholder consultation status, flagged rights, risk score, and conditional approval recommendation.

## Evidence pack

| Document | Purpose |
|---|---|
| [AI System Profile and Governance Intake Record](evidence/1.%20AI%20Governance%20Intake%20Record.docx) | System scope, roles, data, intended use |
| [Third-Party Model and Vendor Governance Review](evidence/2.%20Vendor%20Model%20Governance%20Review.docx) | CrediSure AI due diligence and gaps |
| [AI Risk Register and Mitigation Summary](evidence/3.%20AI%20Risk%20Register%20Mitigation%20Summary.docx) | Six priority risks, treatments, residual risk |
| [Human Oversight, Exception Review, and Applicant Appeal Procedure](evidence/4.%20Human%20Oversight%20Appeal%20Procedure.docx) | Review triggers, reviewer authority, appeals, pause criteria |
| [AI Governance Production Readiness Decision Memo](evidence/5.%20AI%20Governance%20Production%20Readiness%20Decision%20Memo.docx) | Conditional approval decision and conditions |
| [Final VerifyWise report (PDF)](Vivek_Korikanthimath_AI_Governance_Portfolio_Report.pdf) | Generated use case report |

## Skills demonstrated

AI governance review · high-risk AI classification · AI risk identification · risk register development · vendor AI risk review · dataset and model inventory documentation · human oversight design · AI framework mapping (EU AI Act, NIST AI RMF, ISO/IEC 42001) · FRIA · production readiness assessment · executive communication

## Notes on platform limitations

The project was completed in VerifyWise as instructed. Where the platform differed from the instructions, the closest available option was used:

- **Model capabilities:** "Scoring" and "Risk assessment" are not available; Recommendation, Summarization, Anomaly Detection and Forecasting (closest to Prediction) were selected. A unique external key was required for the model.
- **Risk categories:** no "Ethical risk" or "Model risk" option (Technological used); "Data risk" mapped to "Data privacy risk"; "Governance risk" mapped to "Strategic risk". "Awaiting Review" is not an approval status, so "Requires review" was used. The Recommendations field did not save on any risk.
- **NIST AI RMF:** "Completed" is not a status option, so MEASURE and MANAGE use "Implemented". VerifyWise list numbering differs from the subcategory titles (e.g., the GOVERN 3.3.2 item appears as GOVERN 3.2).
- **ISO/IEC 42001:** A.8 and A.11 are section headers, so the implementation text was placed on A.8.1 and A.11.1.
- **EU AI Act:** owner, reviewer, approver, risk review and due date exist only at control level, not per subcontrol. Attaching existing evidence files to requirement subcontrols reported success but did not persist, so evidence was uploaded directly to each subcontrol instead. FRIA evidence attachments display without file names (a display issue).
- **FRIA:** "Private entity" is not a High-Risk Basis option, so "Annex III use case" was selected. First Use Date is left blank (production date unknown), which keeps completion at 95%.
- **Vendor:** the contact field rejects commas. The vendor website was given as two slightly different URLs in the instructions; cyberprosai.com was used consistently.
- **Report:** the generated use case report does not include the incident record (INC-15), although it exists in VerifyWise.

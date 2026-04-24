# Decision / Assumption / Open Questions Log

Structured review log for **Features of the Medical Records System (MRS)**.

| ID | Type | Title | Status | Notes |
| --- | --- | --- | --- | --- |
| Q-01 | Open questions | Role definitions and permission boundaries are not specified | Open | RBAC is required, but the source does not define the user-role matrix or which actions each role may perform across registration, clinical documentation, pharmacy, laboratory, imaging, billing, and reporting. |
| Q-02 | Open questions | SNOMED CT scope is unclear | Open | The source states that SNOMED CT support is optional, but it does not define whether that support is in scope for the baseline release or what depth of terminology support is expected. |
| Q-03 | Open questions | Integration protocols and data formats are not defined | Open | The source lists required integrations but does not specify interface standards, payload formats, authentication methods, or direction of data exchange for HIS, laboratory, PACS, billing, insurance, SMS, or LINE integrations. |
| RSK-01 | Risks | External dependencies may affect delivery and testability | Monitor | Broad integration requirements without interface specifications or partner-system constraints create risk for implementation sequencing, end-to-end testing, and acceptance readiness. |

## Recommended follow-up actions

- **Q-01 — Role definitions and permission boundaries are not specified**
  - RBAC is required, but the source does not define the user-role matrix or which actions each role may perform across registration, clinical documentation, pharmacy, laboratory, imaging, billing, and reporting.
  - Suggested follow-up: Resolve 'Role definitions and permission boundaries are not specified' before implementation and test planning are finalized.
- **Q-02 — SNOMED CT scope is unclear**
  - The source states that SNOMED CT support is optional, but it does not define whether that support is in scope for the baseline release or what depth of terminology support is expected.
  - Suggested follow-up: Resolve 'SNOMED CT scope is unclear' before implementation and test planning are finalized.
- **Q-03 — Integration protocols and data formats are not defined**
  - The source lists required integrations but does not specify interface standards, payload formats, authentication methods, or direction of data exchange for HIS, laboratory, PACS, billing, insurance, SMS, or LINE integrations.
  - Suggested follow-up: Resolve 'Integration protocols and data formats are not defined' before implementation and test planning are finalized.
- **RSK-01 — External dependencies may affect delivery and testability**
  - Broad integration requirements without interface specifications or partner-system constraints create risk for implementation sequencing, end-to-end testing, and acceptance readiness.
  - Suggested follow-up: Define mitigation and ownership for 'External dependencies may affect delivery and testability'.
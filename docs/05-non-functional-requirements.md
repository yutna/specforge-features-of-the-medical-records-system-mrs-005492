# Non-Functional Requirements

Non-functional constraints and quality expectations for **Features of the Medical Records System (MRS)**.

## Quality profile

| Area | Value |
| --- | --- |
| Explicit NFRs | 4 |
| Quality risks | 1 |
| Open questions | 3 |

## Explicit non-functional requirements

### NFR-01 — Performance targets

- **Source:** Lines 101-102

The system shall provide response times of less than 2 seconds and support 50-500 concurrent users.

### NFR-02 — Security controls

- **Source:** Lines 106-109

The system shall provide:
- Encryption at rest and in transit
- Role-based access control (RBAC)
- Full audit trail logging
- Unauthorized access prevention

### NFR-03 — Reliability and backup

- **Source:** Lines 113-114

The system shall provide uptime of at least 99.5% and daily automated backups.

### NFR-04 — Usability and device support

- **Source:** Lines 118-120

The system shall provide a simple user interface, support light and dark modes, and support mobile and tablet devices.


## Related open questions

- **Q-01 — Role definitions and permission boundaries are not specified**
  - RBAC is required, but the source does not define the user-role matrix or which actions each role may perform across registration, clinical documentation, pharmacy, laboratory, imaging, billing, and reporting.
- **Q-02 — SNOMED CT scope is unclear**
  - The source states that SNOMED CT support is optional, but it does not define whether that support is in scope for the baseline release or what depth of terminology support is expected.
- **Q-03 — Integration protocols and data formats are not defined**
  - The source lists required integrations but does not specify interface standards, payload formats, authentication methods, or direction of data exchange for HIS, laboratory, PACS, billing, insurance, SMS, or LINE integrations.

## Quality and delivery risks

- **RSK-01 — External dependencies may affect delivery and testability**
  - Broad integration requirements without interface specifications or partner-system constraints create risk for implementation sequencing, end-to-end testing, and acceptance readiness.

## Operational readiness considerations

- Define monitoring, alerting, and recovery expectations for every production-critical workflow.
- Confirm ownership for performance, availability, security, and compliance controls before implementation starts.
- Translate open questions into measurable acceptance checks before release planning.
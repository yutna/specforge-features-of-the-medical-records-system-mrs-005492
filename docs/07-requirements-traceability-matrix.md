# Requirements Traceability Matrix

Traceability for the current baseline and generated pack for **Features of the Medical Records System (MRS)**.

| Baseline ID | Kind | Title | Source lines | Referenced in | Delivery focus |
| --- | --- | --- | --- | --- | --- |
| BG-01 | Business goals | Support core medical-record operations in one system | Lines 9-9 | Vision / scope / problem statement | Product alignment |
| ACT-01 | Actors and users | Patient | Lines 13-19 | Vision / scope / problem statement, User stories with acceptance criteria | User modelling |
| ACT-02 | Actors and users | Doctor | Lines 39-47 | Vision / scope / problem statement, User stories with acceptance criteria | User modelling |
| ACT-03 | Actors and users | Nurse | Lines 39-47 | Vision / scope / problem statement, User stories with acceptance criteria | User modelling |
| ACT-04 | Actors and users | Radiologist | Lines 70-73 | Vision / scope / problem statement, User stories with acceptance criteria | User modelling |
| FR-01 | Features and capabilities | Patient registration and profile management | Lines 13-19 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| BR-01 | Business rules | Detect potential duplicate patients | Lines 13-19 | Functional requirements, User stories with acceptance criteria | Validation and policy |
| AC-01 | Acceptance conditions | Find existing patients by common identifiers | Lines 13-19 | User stories with acceptance criteria, QA test scenarios / use cases | Verification |
| FR-02 | Features and capabilities | Outpatient encounter documentation | Lines 23-35 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| FR-03 | Features and capabilities | Outpatient orders and certificates | Lines 23-35 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| AC-02 | Acceptance conditions | Complete an OPD visit in a single record | Lines 23-35 | User stories with acceptance criteria, QA test scenarios / use cases | Verification |
| FR-04 | Features and capabilities | Inpatient admission and stay management | Lines 39-47 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| WF-01 | Workflows and processes | Inpatient discharge documentation | Lines 39-47 | Functional requirements, QA test scenarios / use cases | Process orchestration |
| FR-05 | Features and capabilities | Medication and pharmacy operations | Lines 51-57 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| BR-02 | Business rules | Apply medication safety checks | Lines 51-57 | Functional requirements, User stories with acceptance criteria | Validation and policy |
| FR-06 | Features and capabilities | Laboratory order and result management | Lines 61-66 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| INT-01 | Integrations | Integrate laboratory results into the medical record | Lines 61-66 | Functional requirements | External dependency |
| FR-07 | Features and capabilities | Imaging and radiology management | Lines 70-73 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| INT-02 | Integrations | Support PACS and image attachments | Lines 70-73 | Functional requirements | External dependency |
| FR-08 | Features and capabilities | Clinical document management | Lines 77-80 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| FR-09 | Features and capabilities | Appointment scheduling and schedule management | Lines 84-87 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| INT-03 | Integrations | Send appointment reminders through messaging channels | Lines 84-87 | Functional requirements | External dependency |
| FR-10 | Features and capabilities | Billing and insurance processing | Lines 91-95 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| AC-03 | Acceptance conditions | Produce financial outputs for billable care | Lines 91-95 | User stories with acceptance criteria, QA test scenarios / use cases | Verification |
| NFR-01 | Non-functional requirements | Performance targets | Lines 101-102 | Non-functional requirements | Quality control |
| NFR-02 | Non-functional requirements | Security controls | Lines 106-109 | Non-functional requirements | Quality control |
| NFR-03 | Non-functional requirements | Reliability and backup | Lines 113-114 | Non-functional requirements | Quality control |
| NFR-04 | Non-functional requirements | Usability and device support | Lines 118-120 | Non-functional requirements | Quality control |
| CON-01 | Constraints | Clinical coding, privacy, and regulatory compliance | Lines 124-130 | Functional requirements, Non-functional requirements | Technical boundary |
| INT-04 | Integrations | External healthcare and enterprise integrations | Lines 134-138 | Functional requirements | External dependency |
| FR-11 | Features and capabilities | Operational and regulatory reporting | Lines 142-146 | Vision / scope / problem statement, Functional requirements, User stories with acceptance criteria | Functional implementation |
| Q-01 | Open questions | Role definitions and permission boundaries are not specified | Derived during baseline refinement | Non-functional requirements, Decision / assumption / open questions log, QA test scenarios / use cases | Clarification needed |
| Q-02 | Open questions | SNOMED CT scope is unclear | Derived during baseline refinement | Non-functional requirements, Decision / assumption / open questions log, QA test scenarios / use cases | Clarification needed |
| Q-03 | Open questions | Integration protocols and data formats are not defined | Derived during baseline refinement | Non-functional requirements, Decision / assumption / open questions log, QA test scenarios / use cases | Clarification needed |
| RSK-01 | Risks | External dependencies may affect delivery and testability | Derived during baseline refinement | Vision / scope / problem statement, Non-functional requirements, Decision / assumption / open questions log | Mitigation planning |
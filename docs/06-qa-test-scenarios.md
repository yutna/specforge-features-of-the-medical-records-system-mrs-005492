# QA Test Scenarios / Use Cases

This pack captures scenario-ready QA coverage for **Features of the Medical Records System (MRS)**.

## QA coverage snapshot

| Area | Value |
| --- | --- |
| Workflows under test | 1 |
| Executable scenarios | 3 |
| Feature references | 11 |
| Exploratory question areas | 3 |

## Workflow under test

- WF-01 — Inpatient discharge documentation

## TS-01 — Find existing patients by common identifiers

- **Derived from:** AC-01
- **Feature focus:** FR-01 — Patient registration and profile management

```gherkin
Feature: Features of the Medical Records System (MRS)
  Scenario: Find existing patients by common identifiers
    Given the onboarding workflow is available
    When users can search for a patient by hn, national id, name, or phone number.
    Then the expected outcome is produced
```

### Test intent

- Validate the happy path, rejection path, and observable system response.
- Capture traceability to source requirements in test evidence and defect reports.

## TS-02 — Complete an OPD visit in a single record

- **Derived from:** AC-02
- **Feature focus:** FR-02 — Outpatient encounter documentation

```gherkin
Feature: Features of the Medical Records System (MRS)
  Scenario: Complete an OPD visit in a single record
    Given the onboarding workflow is available
    When an opd visit can store clinical findings, diagnoses, orders, treatment plan, and generated medical certificate information as part of the visit record.
    Then the expected outcome is produced
```

### Test intent

- Validate the happy path, rejection path, and observable system response.
- Capture traceability to source requirements in test evidence and defect reports.

## TS-03 — Produce financial outputs for billable care

- **Derived from:** AC-03
- **Feature focus:** FR-03 — Outpatient orders and certificates

```gherkin
Feature: Features of the Medical Records System (MRS)
  Scenario: Produce financial outputs for billable care
    Given the onboarding workflow is available
    When for billable encounters, the system can calculate charges, verify insurance eligibility, and generate invoices and receipts.
    Then the expected outcome is produced
```

### Test intent

- Validate the happy path, rejection path, and observable system response.
- Capture traceability to source requirements in test evidence and defect reports.

## Exploratory follow-up areas

- Q-01 — Role definitions and permission boundaries are not specified
- Q-02 — SNOMED CT scope is unclear
- Q-03 — Integration protocols and data formats are not defined
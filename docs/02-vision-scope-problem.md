# Vision / Scope / Problem Statement

## Problem statement

Baseline requirements for a Medical Records System covering patient administration, outpatient and inpatient documentation, medication and pharmacy operations, laboratory and imaging workflows, document management, appointments, billing and insurance, reporting, compliance, integrations, and core operational quality requirements.

## Scope statement

End-to-end medical-record and care-delivery support for healthcare operations, including registration, clinical documentation, orders, results, scheduling, billing, reporting, security, reliability, compliance, and external-system connectivity.

## Planning profile

| Area | Value |
| --- | --- |
| Primary actors | 4 |
| In-scope capabilities | 11 |
| Documented assumptions | 0 |
| Known risks | 1 |
| Open questions | 3 |

## Business goals

- **BG-01 — Support core medical-record operations in one system**
  - Provide a unified system for patient registration, clinical documentation, orders, results, documents, appointments, billing, reporting, and healthcare integrations.

## Primary actors

- **ACT-01 — Patient**
  - The patient is the primary subject of registration, demographic/profile management, allergy and emergency-contact records, appointments, outpatient visits, inpatient admissions, billing, and reporting.
- **ACT-02 — Doctor**
  - Doctors document outpatient and inpatient clinical records, place medication and lab/X-ray orders, manage treatment plans, prepare discharge summaries, and manage schedules.
- **ACT-03 — Nurse**
  - Nurses document nursing notes, chart intake and output, monitor vital signs, and participate in inpatient medication administration workflows.
- **ACT-04 — Radiologist**
  - Radiologists enter radiology reports for imaging orders.

## In-scope capabilities

- **FR-01 — Patient registration and profile management**
  - The system shall support: - Patient registration - Demographic data entry - Patient profile updates - Allergy record management - Emergency contact information management
- **FR-02 — Outpatient encounter documentation**
  - The system shall support OPD visit creation and documentation of: - Vital signs - Chief complaint - History of present illness (HPI) - Past medical history (PMH) - Family history (FH) - Medication history - Physical examination - ICD-10 diagnoses - Treatment plan
- **FR-03 — Outpatient orders and certificates**
  - Within an OPD visit, the system shall support medication order entry, lab/X-ray order entry, and medical certificate generation.
- **FR-04 — Inpatient admission and stay management**
  - The system shall support: - Patient admission management - Nursing note documentation - Doctor progress note documentation - Intake and output charting - Continuous vital sign monitoring - Medication Administration Record (MAR) management - Lab/X-ray order entry during admission - Referral documentation
- **FR-05 — Medication and pharmacy operations**
  - The system shall support: - Medication order entry - Dispensing workflow management - Lot number and expiry date tracking - Drug inventory management - Drug utilization reporting
- **FR-06 — Laboratory order and result management**
  - The system shall support: - Laboratory order entry - Barcode printing - Laboratory result entry - Graphical display of laboratory results - Turnaround time (TAT) reporting
- **FR-07 — Imaging and radiology management**
  - The system shall support imaging orders for X-ray, CT, and MRI, along with radiologist report entry.
- **FR-08 — Clinical document management**
  - The system shall support document uploads in PDF and JPG formats and store: - Consent forms - Medical certificates - Referral documents
- **FR-09 — Appointment scheduling and schedule management**
  - The system shall support patient appointment scheduling, doctor schedule management, and no-show reporting.
- **FR-10 — Billing and insurance processing**
  - The system shall support: - Charge calculation - Medication, procedure, and room charge management - Insurance eligibility verification - Invoice and receipt generation - Revenue reporting
- **FR-11 — Operational and regulatory reporting**
  - The system shall provide: - Daily patient census reports - ICD-10 disease reports - Drug utilization reports - OPD/IPD statistical reports - Reports for the provincial health office / NHSO

## Assumptions affecting scope

- None captured in the current baseline.

## Key delivery risks

- **RSK-01 — External dependencies may affect delivery and testability**
  - Broad integration requirements without interface specifications or partner-system constraints create risk for implementation sequencing, end-to-end testing, and acceptance readiness.

## Clarifications still needed

- **Q-01 — Role definitions and permission boundaries are not specified**
  - RBAC is required, but the source does not define the user-role matrix or which actions each role may perform across registration, clinical documentation, pharmacy, laboratory, imaging, billing, and reporting.
- **Q-02 — SNOMED CT scope is unclear**
  - The source states that SNOMED CT support is optional, but it does not define whether that support is in scope for the baseline release or what depth of terminology support is expected.
- **Q-03 — Integration protocols and data formats are not defined**
  - The source lists required integrations but does not specify interface standards, payload formats, authentication methods, or direction of data exchange for HIS, laboratory, PACS, billing, insurance, SMS, or LINE integrations.
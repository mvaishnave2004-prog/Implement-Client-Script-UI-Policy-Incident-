# Phase 2 – Requirement Analysis

## Functional Requirements

| ID | Requirement | Proposed ServiceNow Feature |
|---|---|---|
| FR-01 | Detect High Impact Incident | UI Policy |
| FR-02 | Make Assignment group mandatory for High Impact | UI Policy Action |
| FR-03 | Make Urgency read-only for High Impact | UI Policy Action |
| FR-04 | Automatically set Urgency to High | onChange Client Script |
| FR-05 | Prevent save when Assigned To is empty for High Impact | onSubmit Client Script |
| FR-06 | Prevent direct State changes from Incident list | onCellEdit Client Script |
| FR-07 | Allow State changes through the Incident form | Normal form update |

## Configuration Requirements

### UI Policy
- Name: High Impact Control
- Table: Incident
- Active: True
- Condition: Impact is 1 – High
- Reverse if false: True

### Client Script Requirements
- Auto set urgency for high impact
- Prevent save if Assigned To missing
- Prevent state change via list edit

## Non-Functional Considerations
The supplied project specification describes the solution as lightweight, efficient, and suitable for a short-duration micro project.

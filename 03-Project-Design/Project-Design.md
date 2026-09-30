# Phase 3 – Project Design

## High-Level Workflow

Incident Form
→ Check Impact
→ If Impact = High:
  → Assignment group becomes mandatory
  → Urgency is set to High
  → Urgency becomes read-only
→ On Submit:
  → If High Impact + Assigned To empty → block save
  → Otherwise → allow save

Incident List
→ User attempts State list edit
→ onCellEdit runs
→ Alert displayed
→ Change blocked

Incident Form
→ User changes State through the form
→ Update is allowed

## Logical Design

### UI Policy Layer
Controls field behavior based on Impact.

### Client Script Layer
- onChange: automatic behavior
- onSubmit: validation
- onCellEdit: list-edit restriction

### Data Entry Layer
The Incident form and Incident list are the user interaction points.

## Design Objective
Keep the solution simple and focused on client-side Incident data integrity.

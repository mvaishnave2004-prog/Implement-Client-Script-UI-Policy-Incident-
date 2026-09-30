# Phase 1 – Brainstorming & Ideation

## Project Title
Implement Client Script & UI Policy (Incident)

## Problem Identified
Incident records require consistent and accurate data entry for triage, routing, resolution, reporting, SLA-related processes, and overall service quality. Manual checks can lead to incomplete, inconsistent, or incorrect information.

## Proposed Idea
Use ServiceNow client-side controls to enforce business rules directly on the Incident form and list.

The solution combines:
- UI Policy
- UI Policy Actions
- onChange Client Script
- onSubmit Client Script
- onCellEdit Client Script

## Main Idea
When an Incident has **High Impact**, the interface should enforce additional controls. The solution should also prevent invalid submission and restrict direct State changes from list editing.

## Expected Benefits
- Better data completeness
- Consistent Incident entry
- Automatic value population
- Immediate user feedback
- Prevention of invalid submission
- Controlled list editing

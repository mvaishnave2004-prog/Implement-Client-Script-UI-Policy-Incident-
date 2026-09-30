# Phase 8 – Project Demonstration Script

## Opening
“Hello. My project title is Implement Client Script & UI Policy (Incident), developed in ServiceNow.”

## Purpose
“The purpose of this project is to improve Incident data integrity by applying conditional UI behavior, automatic value setting, form validation, and list-edit control.”

## Demonstration 1 – High Impact
“First, I open an Incident and set Impact to High. The UI Policy is triggered. Assignment group becomes mandatory, and Urgency is automatically set to High and becomes read-only.”

## Demonstration 2 – Save Validation
“Next, I leave Assigned To empty and try to submit the Incident. The onSubmit Client Script prevents the save and displays a validation message.”

## Demonstration 3 – Successful Save
“Now I provide an Assigned To value and submit again. The Incident is saved successfully.”

## Demonstration 4 – Reverse Condition
“I change Impact from High to Medium. The UI Policy condition is no longer true, so the mandatory and read-only behavior is reversed.”

## Demonstration 5 – List Editing
“I open the Incident list and try to change State directly. The onCellEdit Client Script blocks the change and displays an alert.”

## Demonstration 6 – Form Update
“Finally, I open the Incident form and change State through the form. This update is allowed and saved successfully.”

## Closing
“This demonstration shows how ServiceNow UI Policies and Client Scripts can work together to improve data consistency and enforce Incident management rules.”

## Video Checklist
- Screen sharing
- Student voice-over
- Project name
- Project purpose
- Use/benefits
- Working process
- Final output
- Google Drive public link

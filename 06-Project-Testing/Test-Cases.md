# Phase 6 – Project Testing

## Test Case 01 – High Impact Behavior
**Input:** Impact = High

**Expected:**
- Assignment group becomes mandatory.
- Urgency becomes High.
- Urgency becomes read-only.

## Test Case 02 – Missing Assigned To
**Input:** Impact = High; Assigned To = empty; Submit.

**Expected:**
- Incident is not saved.
- Error message is displayed.

## Test Case 03 – Successful Save
**Input:** Impact = High; Assigned To = populated; Submit.

**Expected:**
- Incident saves successfully.

## Test Case 04 – Reverse Condition
**Input:** Change Impact from High to Medium.

**Expected:**
- Assignment group is no longer mandatory.
- Urgency becomes editable.

## Test Case 05 – State List Edit
**Input:** Incident → All → attempt direct State edit.

**Expected:**
- Alert appears.
- State remains unchanged.

## Test Case 06 – State Form Update
**Input:** Open Incident form → change State → Update.

**Expected:**
- State change saves successfully.

## Test Result Table

| Test ID | Result | Evidence |
|---|---|---|
| TC-01 | PASS / UPDATE | Add screenshot |
| TC-02 | PASS / UPDATE | Add screenshot |
| TC-03 | PASS / UPDATE | Add screenshot |
| TC-04 | PASS / UPDATE | Add screenshot |
| TC-05 | PASS / UPDATE | Add screenshot |
| TC-06 | PASS / UPDATE | Add screenshot |

Replace `PASS / UPDATE` with the actual result after testing.

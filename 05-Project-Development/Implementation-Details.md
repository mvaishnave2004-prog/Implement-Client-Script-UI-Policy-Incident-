# Phase 5 – Project Development

## 1. UI Policy – High Impact Control

### Configuration
- Name: High Impact Control
- Table: Incident
- Active: True
- Condition: Impact is 1 – High
- Reverse if false: True

## 2. UI Policy Action – Assignment Group

- Field: Assignment group
- Mandatory: True

## 3. UI Policy Action – Urgency

- Field: Urgency
- Read-only: True
- Visible: Leave unchanged

## 4. onChange Client Script

Name: Auto set urgency for high impact

```javascript
function onChange(control, oldValue, newValue, isLoading) {
    if (isLoading || newValue == '') {
        return;
    }

    if (newValue == '1') {
        g_form.setValue('urgency', '1');
        g_form.addInfoMessage('Urgency set to High for High impact incident.');
    }
}
```

## 5. onSubmit Client Script

Name: Prevent save if Assigned To missing

```javascript
function onSubmit() {
    if (g_form.getValue('impact') == '1' &&
        g_form.getValue('assigned_to') == '') {

        g_form.showErrorBox(
            'assigned_to',
            'Assigned To is mandatory for High impact incidents.'
        );

        return false;
    }

    return true;
}
```

## 6. onCellEdit Client Script

Name: Prevent state change via list edit

```javascript
function onCellEdit(sysIDs, table, oldValues, newValue, callback) {
    alert('State cannot be updated using list editing. Please open the Incident.');
    callback(false);
}
```

## Screenshot Evidence
Add actual ServiceNow screenshots to:
`05-Project-Development/Screenshots/`

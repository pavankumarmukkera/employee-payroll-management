# Employee Payroll Management - Power Apps

## Overview
Sample Canvas App design for managing employee
payroll requests and approval statuses.

## Suggested Screens
- Employee Dashboard
- Payroll Request Form
- Manager Approval Screen
- Payroll Status Screen

## Power Fx Examples

### Submit Payroll Request

```powerfx
Patch(
    PayrollRequests,
    Defaults(PayrollRequests),
    {
        Title: txtEmployeeName.Text,
        Amount: Value(txtAmount.Text),
        Status: "Pending"
    }
)
```

### Filter Pending Requests

```powerfx
Filter(
    PayrollRequests,
    Status = "Pending"
)
```

## Status
Learning example only. Not a deployed Canvas App.

The PayrollRequests data source and referenced controls
must be configured before these formulas can work.

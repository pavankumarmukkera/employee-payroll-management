# Dataverse - Payroll Management Data Model

## Proposed Table: PayrollRequests

| Column | Type |
|---|---|
| EmployeeName | Text |
| EmployeeEmail | Email/Text |
| Amount | Currency |
| RequestDate | Date |
| Status | Choice |
| Approver | Lookup |
| Comments | Multiline Text |

## Proposed Status Values
- Pending
- Approved
- Rejected

## Notes
This is a proposed data model.
No Dataverse table has been deployed.

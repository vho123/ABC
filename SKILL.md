---
name: lab-report-row-entry
description: Invoke when a lab-report PDF must be mapped to the lab_test_reports_database workbook schema, validated, and prepared as a new database row.
---

## Purpose
Convert one lab-report PDF into a validated row aligned to the destination workbook's existing columns. Always create new record in the excel not update.

## Uses
- Agent capabilities: code interpreter, OneDrive and SharePoint access
- Agent data: `NewReports` folder and `lab_test_reports_database.xlsx`

## Instructions
1. Locate the target PDF in `NewReports` and open `lab_test_reports_database.xlsx` to read its current header row.
2. Extract patient, report, facility, date, identifier, test-result, and unit values from the PDF. Preserve source wording for names and facilities.
3. Normalize dates to Excel-compatible ISO dates, keep numeric results as numbers, and place units in their matching unit columns.
4. Map only fields that correspond to existing workbook headers. Leave unavailable fields blank and record ambiguities separately rather than guessing.
5. Assigned report ID to the new record following the Report ID pattern, pick the last number in excel and increment by 1.
6. "Age at report" is calculated by the "Date Received" and the patient's "Date of birth".
7. A unique row in excel based on 2 columns, Patient ID and Ref. No.
8. Stop for review when required identifiers are missing, or extracted values conflict with the PDF.
9. Return the validated ordered row, validation messages, source filename, and processing status. Add the row to the workbook only when the host environment provides an authorized file-update action.

## Parameters
- Lab-report PDF folder path, https://hso1com-my.sharepoint.com/:f:/r/personal/hho_hso_com/Documents/Work/Training/GHK%20Hospital%20Copilot%20Studio%20Workflow/Lab1/NewReports?d=w297212d2e26a4c71915f545616eed9f3&csf=1&web=1&e=fLiNZg
- Destination workbook URL, https://hso1com-my.sharepoint.com/:x:/r/personal/hho_hso_com/Documents/Work/Training/GHK%20Hospital%20Copilot%20Studio%20Workflow/Lab1/lab_test_reports_database.xlsx?d=w6e71f3775e234ef89e4af20fe5568802&csf=1&web=1&e=cK2ojs

## Output
A validated JSON result containing the ordered workbook row, warnings, source filename, and ready-for-entry status.
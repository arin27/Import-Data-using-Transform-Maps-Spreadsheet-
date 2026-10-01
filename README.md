## IMPORT DATA USING TRASFORM MAPS (SPREADSHEET)

## Project Overview

Import Data Using Transform Maps (Spreadsheet) is a ServiceNow-based project developed to simplify the process of importing, managing, validating, and analysing employee information from spreadsheet data.
In many organizations, employee information is maintained in spreadsheets. Manually entering this information into a ServiceNow system can be time-consuming and may lead to incorrect data, duplicate records, or inconsistent information. This project provides a structured way to import employee data while maintaining accuracy and consistency.
The project uses ServiceNow Import Sets and Transform Maps to transfer spreadsheet data into a structured employee table. The data is first loaded into an Employee Import / staging table and then transformed into the Employee Test table using predefined field mappings.
Employee ID is configured as a coalesce field so that existing employee records can be identified during subsequent imports. This helps reduce unnecessary duplicate records and makes repeated data imports easier to manage.
The imported employee information is also used to generate reports and an Employee Analytics Dashboard, providing a centralized view of employee information based on department and location. Access to employee information is controlled using ServiceNow roles and ACLs.

---

## Objectives

- Import employee data from spreadsheets into ServiceNow
- Reduce repetitive manual data entry
- Maintain structured and consistent employee information
- Map spreadsheet fields to the appropriate ServiceNow fields
- Use Employee ID to identify existing employee records
- Prevent unnecessary duplicate records during re-import
- Validate imported employee information
- Generate employee reports based on department and location
- Provide an Employee Analytics Dashboard for data visualization
- Implement controlled access to employee information
- Improve the overall efficiency of employee data management
---

## Technologies Used

- ServiceNow
- Import Sets
- Transform Maps
- ServiceNow Tables
- ServiceNow Reports
- ServiceNow Dashboards
- Coalesce
- Roles & Access Control Lists (ACLs)
---

## Project Workflow

Spreadsheet
     ↓
Import Set
     ↓
Employee Import / Staging Table
     ↓
Transform Map
     ↓
Employee Test Table
     ↓
Reports & Employee Analytics Dashboard

The spreadsheet contains employee information such as Employee Name, Email, Department, Employee ID, and Location. These records are first imported into the staging table.
The Sample Spreadsheet Import Transform Map is then used to map the source fields to the corresponding fields in the Employee Test table. Employee ID is configured as the coalesce field to support matching with existing records.
After the transformation is completed, the employee records are validated and made available for reporting and dashboard analysis.

---

## Transform Map Field Mapping

Source Field : u_name, u_email, u_department, u_employee_id, u_location	

Target Field : u_employee_name, u_email, u_department, u_employee_id, u_location


---

## Key Features
- Spreadsheet-based employee data import
- Automated field mapping using Transform Maps
- Employee ID-based record matching
- Duplicate prevention through coalesce
- Centralized employee information
- Employee List report
- Employees by Location report
- Employees by Department report
- Employee Analytics Dashboard
- Role-based access control
- ACL-based read and write restrictions
- Structured data validation and testing
---

## Reporting and Dashboard

The project includes multiple reports to make employee information easier to understand and analyse.
The Employee List provides a detailed view of employee records, while the Employees by Location and Employees by Department reports provide summarized information based on specific employee attributes.
These reports are brought together in the Employee Analytics Dashboard, giving authorized users a centralized view of the employee dataset.

---

## Security

Since employee information needs to be protected, the project uses ServiceNow's built-in security mechanisms.
Roles and Access Control Lists (ACLs) are used to control read and write access to employee records. This ensures that only users with the appropriate permissions can view or modify the information.

---

## Testing and Results

The project was tested for spreadsheet import, field mapping, Transform Map execution, coalesce functionality, duplicate prevention, re-import handling, reports, and dashboard functionality.
8 User Acceptance Testing (UAT) test cases were completed successfully. During testing, issues related to duplicate records, blank Employee Name values, and an incorrect Location chart type were identified and resolved.
The final dataset contains 17 employee records.
The completed solution demonstrates an end-to-end ServiceNow workflow for importing spreadsheet data, transforming it into structured employee records, securing the information, and presenting it through reports and dashboards.

---

## Future Enhancements

The project can be further enhanced by introducing scheduled automatic imports, advanced spreadsheet validation, additional employee and training fields, more interactive dashboard filters, automated notifications, and detailed import audit reports.

---

## Team Members

Team ID: SWTID-2026-7612
- Gopika Sri G K
- Poojasri T S
- Harini Eswari Ramesh Babu
---

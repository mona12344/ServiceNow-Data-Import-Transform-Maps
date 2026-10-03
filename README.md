# ServiceNow-Data-Import-Transform-Maps
ServiceNow Import Sets, Transform Maps, and Analytics Dashboard Project for Naan Mudhalvan
# ServiceNow Data Import using Transform Maps & Analytics Dashboard

## Project Overview
This project focuses on importing structured employee data from an external spreadsheet into the ServiceNow platform using Import Sets and Transform Maps. It handles record transformations, implements Coalesce logic to prevent duplicates, and visualizes the dataset through custom Reports and an Employee Analytics Dashboard.

---

## Technical Features & Concepts
- **Target Table:** `u_employee_test` (Employee Test)
- **Import Set Table:** `u_employee_import` (Employee Import)
- **Transform Map:** `Sample Spreadsheet Import`
- **Data Integrity:** Coalesce enabled on `Employee ID` to perform updates on existing records and insert new ones.
- **Reporting:** Pie Chart, Bar Chart, and List Report embedded in `Employee Analytics Dashboard`.

---

## Project Phases & Workflow

### Phase 1–3: Data Preparation & Import Set
- Created sample `.xlsx` spreadsheet containing employee details.
- Loaded raw dataset into ServiceNow via **Load Data** to generate the staging Import Set Table.

### Phase 4–5: Field Mapping & Transformation
- Configured field mappings between source columns (`Employee ID`, `Name`, `Email`, `Department`, `Location`) and target table fields.
- Executed transformation to populate target records successfully.

### Phase 6–7: Coalesce Validation
- Set `Coalesce = True` on `Employee ID`.
- Re-imported modified datasets to verify that existing records updated while avoiding duplicate entries.

### Phase 8–9: Reports & Dashboard
- **Employees by Department:** Pie Chart (Grouped by Department)
- **Employees by Location:** Bar Chart (Grouped by Location)
- **Employee List:** Full record list view
- **Dashboard:** Consolidated all three reports into `Employee Analytics Dashboard`.

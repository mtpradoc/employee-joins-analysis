# Employee Demographics and Salary Analysis with Joins

## Overview
This project explores how to perform different types of joins in Tableau, utilizing employee demographics, job titles, and salary data from Excel files. By mimicking SQL-like joins, we demonstrate the impact of various joins (Inner, Left, Right, Full Outer) on a dataset, and how to effectively visualize the resulting data.

## Project Details

### 1. Data Overview
- **Demographics Table**: Contains 10 rows with columns `EmployeeID`, `Name of Employee`, `EmployeeAge`, and `EmployeeGender`.
- **Job Title Table**: Includes 11 rows, with one row missing its `EmployeeID`. Columns include `EmployeeID`, `EmployeeName`, and `JobTitle`.
- **Salary Table**: Contains 7 rows with columns `EmployeeID` and `EmployeeSalary`.

### 2. Performing Joins in Tableau
- Uploaded the Excel file into Tableau.
- Used joins on the `EmployeeID` field across the three tables:
  - **Inner Join**: Only records with matching `EmployeeID` in both tables are retained.
  - **Left Join**: All records from the Demographics table are retained, along with matching records from the Job Title table.
  - **Right Join**: All records from the Job Title table are retained, along with matching records from the Demographics table.
  - **Full Outer Join**: All records from both tables are retained, regardless of matching `EmployeeID`.

### 3. Employee Name Join
- After performing joins based on `EmployeeID`, we used `EmployeeName` as a second join condition between the Demographics and Job Title tables.

![joins](https://github.com/user-attachments/assets/4b8f5af9-6101-44f3-88e7-2bb7f4c9cf1c)

### 4. Final Join and Visualization
- Combined the **Demographics**, **Job Title**, and **Salary** tables using an `EmployeeID` join to consolidate all data into a single view.
- Visualized the total salary per employee by creating a bar chart:
  - **Columns**: `Name of Employee`
  - **Rows**: `Sum(Employee Salary)`
  - **Color Marks**: Used color to represent different salary sums.
<a href="https://public.tableau.com/views/Employee_Joins/SalaryperEmployee?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link">
<img src="https://github.com/user-attachments/assets/d74652e7-7ecf-4c42-bbbc-170a66d84c45">
</a>

## Tools Used
- **Tableau**: For performing joins and visualizing the data.
- **Excel**: Data source containing employee demographics, job titles, and salary information.

## How to Use
1. **Open Tableau Workbook**: Explore the joins and visualizations by opening the Tableau workbook file.
2. **Modify Joins**: Experiment with different join types (Inner, Left, Right, Full Outer) to see how they impact the dataset.
3. **Visualize Data**: Use the bar chart to explore the total salary per employee.

## Key Insights
- Each type of join affects the dataset differently based on matching and non-matching records.
- Joining on both `EmployeeID` and `EmployeeName` allows for a more comprehensive consolidation of employee data.
- The final visualization provides a clear view of the total salary per employee, with easy-to-interpret visual cues like color for salary sums.

## Future Enhancements
- Add more employee data for a larger dataset.
- Introduce additional fields like `EmployeeDepartment` or `Years of Service` for deeper analysis.
- Create more complex visualizations to further explore the data.

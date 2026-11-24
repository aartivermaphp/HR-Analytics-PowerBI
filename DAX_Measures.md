DAX Measures

Total Employees

Total Employees =
DISTINCTCOUNT('HR_Employee_Data'[EmployeeID])

Attrition Count

Attrition Count =
CALCULATE(
    [Total Employees],
    'HR_Employee_Data'[Attrition] = "Yes"
)

Attrition Rate

Attrition Rate =
DIVIDE(
    [Attrition Count],
    [Total Employees],
    0
)

Average Salary

Average Salary =
AVERAGE('HR_Employee_Data'[Salary])
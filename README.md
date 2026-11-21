# DSWP-Experiment-1.A-Employee-Data-Display-Using-Python

## Aim

To collect employee details, validate inputs, and calculate gross and net salary using Python.

## Algorithm

1. **Start** the program.
2. **Read Employee Details** from the user:
   * Input `name` (String) for the employee's full name.
   * Input `emp_id` (String) for the employee's identification number.
   * Input `basic` (Float) for the employee's basic salary.
3. **Validate Input**:
   * Ensure `basic` is a valid numeric value and check if `basic < 0`. If invalid or negative, display an appropriate error message and terminate the program.
4. **Compute Allowances**:
   * Calculate House Rent Allowance: $\text{HRA} = 0.15 \times \text{basic}$.
   * Calculate Dearness Allowance: $\text{DA} = 0.10 \times \text{basic}$.
5. **Compute Gross Salary**:
   * Calculate total earnings before deductions: $\text{Gross Salary} = \text{basic} + \text{HRA} + \text{DA}$.
6. **Compute Tax Deduction**:
   * Calculate income tax at $8\%$ of gross pay: $\text{Tax} = 0.08 \times \text{Gross Salary}$.
7. **Compute Net Salary**:
   * Calculate take-home pay: $\text{Net Salary} = \text{Gross Salary} - \text{Tax}$.
8. **Display Formatted Payroll Report**:
   * Print a structured summary displaying `name`, `emp_id`, `basic`, `HRA`, `DA`, `Gross Salary`, `Tax`, and `Net Salary` formatted to two decimal places.
9. **Stop** the program.

## Program
## Input 
```
# Employee Payroll Calculation

# Get employee details
name = input("Enter Employee Name: ")

emp_id = input("Enter Employee ID: ")

basic = float(input("Enter Basic Pay: "))

# Calculate allowances
hra = 0.15 * basic

da = 0.10 * basic

# Calculate gross salary
gross = basic + hra + da

# Calculate tax
tax = 0.08 * gross

# Calculate net salary
net = gross - tax

# Display employee salary report
print("\n--- Employee Salary Report ---")

print(f"Employee Name: {name}")

print(f"Employee ID: {emp_id}")

print(f"Basic Pay: {basic}")

print(f"HRA: {hra}")

print(f"DA: {da}")

print(f"Gross Salary: {gross}")

print(f"Tax Deducted: {tax}")

print(f"Net Salary: {net}")
```

## Output
```
Enter Employee Name: Santhosh M
Enter Employee ID: 212225410118
Enter Basic Pay: 200000

--- Employee Salary Report ---
Employee Name: Nagaraj S
Employee ID: 212225410118
Basic Pay: 200000.0
HRA: 15000.0
DA: 10000.0
Gross Salary: 225000.0
Tax Deducted: 10000.0
Net Salary: 215000.0
```

## Result

The program successfully accepts and validates employee details, calculates allowances and deductions, and displays a well-formatted salary report.

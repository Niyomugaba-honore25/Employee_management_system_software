# Employee Management System

A Java console-based Employee Management System designed to manage employee records, process payroll, and generate payroll reports.

## Features

* Add new employees
* Validate employee information
* Prevent duplicate employee IDs
* Remove employees by ID
* Process employee payments
* Calculate overtime payments
* Apply management bonuses
* Calculate applicable taxes
* Generate payroll reports
* Display total and average payroll
* Identify the highest-paid employee
* Display the current number of employees

## Functional Requirements

| ID   | Requirement                                                       |
| ---- | ----------------------------------------------------------------- |
| FR1  | Add an employee with ID, name, department, and base salary        |
| FR2  | Validate employee information and reject invalid input            |
| FR3  | Prevent duplicate employee IDs                                    |
| FR4  | Remove an employee using their employee ID                        |
| FR5  | Process employee payments based on salary and working hours       |
| FR6  | Calculate overtime payment and management bonus                   |
| FR7  | Apply the appropriate tax rate                                    |
| FR8  | Generate a payroll report containing employee payment information |
| FR9  | Display total and average payroll                                 |
| FR10 | Identify the highest-paid employee                                |
| FR11 | Display the current number of registered employees                |

## Business Rules

### Overtime

Overtime is calculated using an overtime multiplier of **1.5× the normal hourly rate**.

Normal hourly rate:

```text
Base Salary / 160
```

### Management Bonus

Employees in the **Management** department receive a management bonus of **15%**.

### Tax

The system applies the following tax rules:

* **20% tax** when gross payment is greater than or equal to 5,000
* **10% tax** when gross payment is below 5,000

### Allowed Departments

The following departments are accepted:

* Engineering
* Management
* HR
* Finance
* IT

## Input Validation

The system validates the following employee information:

### Employee ID

* Must be provided
* Must be unique
* Must contain valid characters

### Employee Name

* Must not be empty
* Must contain a valid employee name

### Department

The department must be one of the supported departments:

```text
Engineering
Management
HR
Finance
IT
```

### Base Salary

* Must be greater than 0
* Must be a valid numeric value

### Working Hours

The system validates regular and overtime working hours to prevent invalid payment calculations.

## Technologies Used

* **Java**
* **Object-Oriented Programming (OOP)**
* **Java Collections**
* **Input Validation**
* **Console-based User Interface**
* **Unit Testing**

## Project Structure

```text
EmployeeManagementSystem-main/
│
├── EmployeeManagementSystem.java
├── EmployeeManagementSystemTest.java
├── README.md
└── ...
```

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/Niyomugaba-honore25/Employee_management_system_software.git
```

### 2. Open the Project

```bash
cd Employee_management_system_software
```

### 3. Compile the Application

```bash
javac EmployeeManagementSystem.java
```

### 4. Run the Application

```bash
java EmployeeManagementSystem
```

## Testing

If the project includes the test class, compile both files:

```bash
javac EmployeeManagementSystem.java EmployeeManagementSystemTest.java
```

Then run:

```bash
java EmployeeManagementSystemTest
```

## Author

**NIYOMUGABA Honore**

Software Engineering Student

GitHub: `Niyomugaba-honore25`

## Repository

[Employee Management System](https://github.com/Niyomugaba-honore25/Employee_management_system_software)

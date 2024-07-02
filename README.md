# Software Requirements Specification for Payroll System Expansion

## Section 1: Introduction

### Purpose

The purpose of creating the Software Requirements Specification (SRS) is to provide a comprehensive and detailed description of the payroll system. This document aims to ensure that the system meets the intended requirements, and serves as a reference for the development, maintenance, and enhancement of the system. The SRS covers both functional and non-functional requirements and includes sections on project scope, product perspective, user needs, assumptions, dependencies, system features, and non-functional requirements. Key stakeholders, such as project managers, developers, testers, and end-users, will use this document to understand and implement the system accurately.

### Project Scope and Exclusions

#### Scope

The updated payroll system aims to enhance employee management and payroll processing capabilities. The system will provide a user-friendly interface and includes features such as employee management, payroll calculation, leave management, reporting, and a self-service portal for employees. The primary objectives are to improve efficiency, accuracy, and compliance with regulatory requirements. This system supports the corporate goal of enhancing operational efficiency and employee satisfaction.

#### Exclusions

The payroll system does not extend to employee performance evaluations, goal setting, or other aspects of performance management. Additionally, integration with external third-party software, non-payroll HR functions such as recruitment, and multi-currency payroll processing are excluded from this system.

---

## Section 2: Overall Description

### Product Perspective

The expanded payroll system offers a range of key features and functionalities to streamline payroll processing and employee management. It includes a secure employee login, automated payroll generation, comprehensive HR management, leave management, and a self-service portal for employees. These features enhance the overall efficiency and accuracy of operations. For example, the system's advanced reporting tools enable HR personnel to generate detailed payslips and payroll summaries effortlessly.

### User Needs

The payroll system addresses several key user needs and pain points:

- **Ease of Use:** Users require an intuitive interface for easy navigation and quick access to information.
- **Accurate Payroll Processing:** Payroll administrators need precise salary calculations and timely processing to meet regulatory requirements and employee expectations.
- **Comprehensive Reporting:** Payroll administrators need access to detailed reports and analytics for payroll data, including earnings summaries.
- **Self-Service Capabilities:** Employees should be able to view personal information, submit leave requests, and access electronic payslips easily.

These needs are prioritized based on their importance and impact on users, ensuring the system meets their expectations effectively.

### Assumptions and Dependencies

#### Assumptions

- **User Adoption:** Users will efficiently adopt and adapt to the new system with adequate training and support.
- **Data Accuracy:** Users will enter accurate and up-to-date data into the system.
- **Security Measures:** Implemented security measures will safeguard sensitive payroll data.

#### Dependencies

- **Database Management System (DBMS):** The system's stability relies on the chosen DBMS (e.g., MySQL) for efficient data management.
- **Hardware Requirements:** Adequate hardware resources are essential for the system's performance and scalability.
- **Regulatory Updates:** The system must adapt to timely updates in legal or regulatory requirements, impacting functionalities and compliance measures.

---

## Section 3: System Features and Requirements

### System Features

1. **Employee Login Functionality:** Secure login for employees to access profiles and personal information, with error handling for invalid login attempts.
   
2. **Payroll Generation Capability:** Automated calculation and generation of employee payslips. Payroll administrators review and save payslips, which are then automatically distributed to employees.
   
3. **HR Management Functions:** HR can add, edit, view, and delete employee information with input validation to ensure accurate records.
   
4. **Leave Management:** HR can approve, disapprove, view, and delete leave requests, maintaining accurate records of employee leave.
   
5. **Employee Self-Service Portal:** Employees can view personal information, record time in and out, submit and track leave requests, and view electronic payslips with detailed breakdowns.
   
6. **Reporting Capabilities:** Generates detailed payslip reports, including earnings, deductions, benefits, and take-home pay summaries. An analytics dashboard provides visual insights into payroll trends, attendance patterns, and leave utilization.
   
7. **System Administrator Functionalities:** System administrators manage user accounts, roles, and access levels, reset passwords, and update access controls. Role-based access control ensures secure and efficient system management.

### Non-functional Requirements

- **Performance:** The system should handle multiple concurrent users without performance degradation, ensuring timely payroll processing and report generation.
   
- **Scalability:** The system should accommodate growing employee numbers and increased data volume.
   
- **Security:** Strong authentication, authorization mechanisms, and data encryption must protect sensitive information, ensuring compliance with data privacy regulations.
   
- **Usability:** An intuitive interface should require minimal training for end-users.
   
- **Reliability:** The system should have minimal downtime, ensuring continuous availability.
   
- **Maintainability:** Modular design facilitates easy maintenance and updates, supported by comprehensive documentation.
   
- **Compliance:** The system must adhere to relevant payroll regulations and standards.

---

## Section 4: Appendix

### Glossary

- **Authentication:** The process of verifying the identity of a user attempting to access the system.
- **Controller:** In MVC architecture, the component that handles user input and interacts with the model to update the view.
- **CRUD:** Create, Read, Update, Delete - basic operations performed on database records.
- **Deduction:** Amounts subtracted from an employee's gross salary, such as taxes and insurance contributions.
- **DBMS:** Database Management System, used for storing and managing data (e.g., MySQL).
- **Employee:** An individual who works for the organization and receives compensation.
- **Entity:** An object with a distinct identity, typically represented as a table in the database.
- **Frontend:** The user-facing part of the application, typically involving the user interface.
- **Gross Salary:** The total salary earned by an employee before deductions.
- **HR:** Human Resources, the department responsible for managing employee-related functions.
- **HR Dashboard:** A real-time dashboard for HR administrators displaying key HR metrics and visualizations.
- **IT Administrator:** A user role responsible for managing IT-related aspects of the system.
- **Inheritance:** A class-based programming concept where one class derives properties and behaviors from another class.
- **JavaFX:** A software platform used for creating and delivering desktop applications with a modern user interface.
- **Leave Request:** An employee's application for time off from work.
- **Model:** In MVC architecture, the component that represents the application's data and business logic.
- **MVC:** Model-View-Controller, a design pattern for organizing code in applications.
- **Net Salary:** The amount of salary received by an employee after deductions.
- **Pag-IBIG:** A government-mandated savings program in the Philippines.
- **PhilHealth:** The Philippine Health Insurance Corporation, providing health insurance to employees.
- **Payslip:** A document detailing an employee's earnings and deductions for a specific period.
- **Reporting Tools:** Software tools used to generate and manage reports.
- **Role:** A defined set of permissions and access rights assigned to a user.
- **SSS:** Social Security System, providing social insurance to employees in the Philippines.
- **Security:** Measures taken to protect the system and its data from unauthorized access or attacks.
- **Timesheet:** A record of the hours an employee has worked.
- **TIN:** Tax Identification Number, used for tax purposes in the Philippines.
- **User:** An individual who interacts with the system, such as an employee or administrator.
- **User Interface (UI):** The part of the system that users interact with, including screens and menus.
- **View:** In MVC architecture, the component that displays the data to the user.

### Diagrams

- **Figure 1: Use Case Diagram of the Expanded Payroll System**
  [Click here to view full resolution](Use Case Diagram.png - initial (diagrams.net))

  The use case diagram illustrates the various interactions between different actors and the payroll system. Below is an explanation of the use case diagram components:

  **Actors:**
  - **Employee:** Interacts with personal account details, attendance records, payslip viewing, leave requests, and time tracking.
  - **Payroll Administrator:** Manages payroll reports, payslip generation, and payroll summaries.
  - **IT Administrator:** Handles system security and user role management.
  - **HR Administrator:** Manages employee records, attendance, leave requests, and approvals.

  **Use Cases:**
  - **Employee:**
    - **Time Tracking:** Records time in and time out.
    - **View Payslip:** Access payslips by month or year.
    - **View Leave Status:** Check approved leave request status.
    - **Login:** Secure access to the system.
    - **Manage Leave:** View remaining leave credits and submit leave requests.
  - **IT Administrator:**
    - **Role Management:** Administers role-based access control.
    - **User Management:** Manages user accounts.
  - **Payroll Administrator:**
    - **Generate Reports:** Creates monthly payroll reports and summaries.
    - **Generate Payslip:** Calculates and saves employee payslips.
  - **HR Administrator:**
    - **Employee Management:** Adds, modifies, and deletes employee records.
    - **Attendance and Leave:** Monitors attendance records and manages leave requests.

  **Interactions:**
  - All actors log in to access their respective functionalities.
  - Generate Payslip involves computing allowances, deductions, and saving payslips.
  - Role-Based Access Control ensures secure user access across the system.

- **Figure 2: Class Diagram of the Expanded Payroll System**
  [Click here to view full resolution](Class Diagram.png - initial (diagrams.net))

  The class diagram illustrates the structure and relationships of classes within the payroll system. Key components include:

  **Classes:**
  - **Employee:** Represents individual employee details such as ID, name, and contact information.
  - **Payroll:** Manages payroll data, including earnings, deductions, and net salary calculations.
  - **HRManager:** Handles employee management functionalities such as adding, editing, and deleting employee records.
  - **SecurityManager:** Implements authentication and authorization mechanisms to ensure secure system access.
  - **ReportGenerator:** Generates payroll reports and analytics dashboards based on user inputs.

  **Relationships:**
  - **Association:** Connects classes to represent relationships, such as Employee to Payroll for salary calculation.
  - **Inheritance:** Shows inheritance relationships, such as HRManager inheriting functionality from UserManager.
  - **Dependency:** Indicates dependencies between classes, for example, Payroll depends on Employee data for calculations.

---

## Section 5: References

- [PHP Manual](https://www.php.net/manual/en/)
- [MySQL Documentation](https://dev.mysql.com/doc/)
- [HTML5 Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS3 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [JavaScript Guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
- [Bootstrap Documentation](https://getbootstrap.com/docs/5.0/getting-started/introduction/)

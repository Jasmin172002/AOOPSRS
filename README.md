# Software Requirements Specification for Payroll System Expansion

## TABLE OF CONTENTS

- [Introduction](#introduction)
  - [Purpose](#purpose)
  - [Project Scope and Exclusions](#project-scope-and-exclusions)

- [Overall Description](#overall-description)
  - [Product Perspective](#product-perspective)
  - [User Needs](#user-needs)
  - [Assumptions and Dependencies](#assumptions-and-dependencies)

- [System Features and Requirements](#system-features-and-requirements)
  - [System Features](#system-features)
  - [Non-functional Requirements](#non-functional-requirements)

- [Appendix](#appendix)
  - [Glossary](#glossary)
  - [Diagrams](#diagrams)
  - [Demo Video](#demo-video)

## Introduction

### Purpose

The purpose of creating the Software Requirements Specification (SRS) is to provide a comprehensive and detailed description of the payroll system. This document aims to ensure that the system meets the intended requirements, and serves as a reference for the development, maintenance, and enhancement of the system. The SRS covers both functional and non-functional requirements and includes sections on project scope, product perspective, user needs, assumptions, dependencies, system features, and non-functional requirements. Key stakeholders, such as project managers, developers, testers, and end-users, will use this document to understand and implement the system accurately.

### Project Scope and Exclusions

#### Scope

The updated payroll system aims to enhance employee management and payroll processing capabilities. The system will provide a user-friendly interface and includes features such as employee management, payroll calculation, leave management, reporting, and a self-service portal for employees. The primary objectives are to improve efficiency, accuracy, and compliance with regulatory requirements. This system supports the corporate goal of enhancing operational efficiency and employee satisfaction.

#### Exclusions

The payroll system does not extend to employee performance evaluations, goal setting, or other aspects of performance management. Additionally, integration with external third-party software, non-payroll HR functions such as recruitment, and multi-currency payroll processing are excluded from this system.

---

## Overall Description

### Product Perspective

The expanded payroll system offers a range of key features and functionalities to streamline payroll processing and employee management. It includes a secure employee login, automated payroll generation, comprehensive HR management, leave management, and a self-service portal for employees. These features enhance the overall efficiency and accuracy of operations. For example, the system's advanced reporting tools enable HR personnel to generate detailed payslips and payroll summaries effortlessly.

### User Needs

The payroll system addresses several key user needs:

#### Payroll Administrators:
- **Accuracy and Compliance:** Ensure precise payroll calculations and compliance with labor laws.
- **Efficiency in Processing:** Streamline payroll processes to reduce manual errors and improve efficiency.
- **Payroll Dashboard:** Access a dashboard for monthly pay period management and monitoring.

#### Employees:
- **Self-Service Options:** Access electronic payslips, submit leave requests, and update personal information conveniently.
- **Clear Information Access:** Easily understand and access pay details, allowance breakdown, salary details, and leave balances.
- **User-Friendly Interface:** Navigate the system effortlessly for self-service tasks.

#### HR Administrators:
- **Employee Management:** Edit, view, and delete employee information as necessary to maintain accurate records and ensure compliance with company policies.
- **Leave Approval Management:** Streamline and automate the process of approving employee leave requests to ensure timely responses and compliance with company policies.
- **Dashboard for Leave Management:** Access a centralized dashboard to monitor leave balances, track employee absences, and forecast staffing needs effectively.
- **Timesheet Management:** Efficiently manage and track employee work hours and attendance through an integrated timesheet management module.

#### IT Administrators:
- **Access Control:** Manage access levels and permissions for employees to ensure data security and regulatory compliance.
- **Password Management:** Facilitate secure password management and updates for employee accounts, ensuring robust cybersecurity practices across the payroll system infrastructure.

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

## System Features and Requirements

### System Features

1. **Employee Login Functionality:** 
- Description: Provides a secure login mechanism for employees to access their profiles and personal information. Includes error handling for invalid login attempts and password recovery options.
- Use Case: Organizes requirements based on different scenarios like successful login and password recovery.
- Mode of Operation: Includes normal operation and password recovery modes.
- User Class: Targets employee users for accessing personal information and IT administrators for managing security aspects.
- Object Class: Manages user credentials securely.
- Functional Hierarchy: Includes modules for authentication and session management.
- Combinations: Integrates use cases for seamless functionality during login and information access.
   
   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/10f8fbb0-06ff-4356-a376-c5d4c8112997" alt="loginsuc" width="500">
   <small>Figure 1: Successful Login</small>

   {insert GIF}
   <small>Figure 2: Submitting Forgot Password</small>

2. **Payroll Generation Capability:** 
- Description: Automates calculation and generation of employee payslips based on predefined rules and inputs. Allows administrators to review, edit, and distribute payslips.
- Use Case: Organizes requirements for generating, editing, and distributing payslips.
- Mode of Operation: Includes processes for generating, editing, and distributing payslips securely.
- User Class: Targets payroll administrators for managing payslip generation and distribution.
- Object Class: Manages payroll data and rules for accurate calculation.
- Functional Hierarchy: Includes modules for payroll calculation, editing, and distribution.
- Combinations: Integrates use cases for seamless payroll management and distribution.

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/19296a34-9114-4368-96dc-4c4556258216" alt="generatepaylip" width="500"/>
   <small>Figure 3: Generating and Saving Payslips</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/630af10e-bd5f-48a2-af9e-49fe3f31e418" alt="editp" width="500"/>
   <small>Figure 4: Viewing and Editing Employee Payslipss</small>

3. **HR Management Functions:**
- Description: Enables HR personnel to manage employee records, including adding, editing, viewing detailed information, and handling deletions.
- Use Case: Organizes requirements for adding, editing, viewing, and deleting employee records.
- Mode of Operation: Includes secure operations for managing employee data.
- User Class: Targets HR administrators for managing employee information securely.
- Object Class: Manages employee data integrity and validation.
- Functional Hierarchy: Includes modules for employee data management and validation.
- Combinations: Integrates use cases for seamless HR operations and employee record management.

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/e38b0c34-f2a5-4e7f-95fd-27a795d8da42" alt="addem" width="500"/>
   <small>Figure 5: Adding a new employee</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/6a0f7ee2-dddf-42d7-a567-f77388c0fe2f" alt="editem" width="500"/>
   <small>Figure 6: Editing Employee Information</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/09fe8a54-6a14-49e8-8ba9-db092e01fb8a" alt="viewem" width="500"/>
   <small>Figure 7: Viewing and Deleting Employee Information</small>
   
4. **Leave Management:**
- Description: Facilitates the process of leave request management, including approval, disapproval, viewing, and deletion of leave requests.
- Use Case: Organizes requirements for managing leave requests through approval cycles.
- Mode of Operation: Includes secure processes for managing leave requests and approvals.
- User Class: Targets HR personnel for managing leave requests efficiently.
- Object Class: Manages leave request data and approval workflows.
- Functional Hierarchy: Includes modules for leave request submission, approval, and tracking.
- Combinations: Integrates use cases for seamless leave management and tracking.

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/54754eae-dc50-4dfc-99cb-f75099dfd142" alt="approve" width="500"/>
   <small>Figure 8: Approving Leave Request</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/753644bf-f96b-415c-b51a-aa1635f1fddc" alt="disapp" width="500"/>
   <small>Figure 9: Disapproving Leave Request</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/55c26bd2-46f5-4d01-9956-98a2b81ff867" alt="viewleave" style="width:500px;">
   <small>Figure 10: Viewing and Deleting Leave Request</small>
   
5. **Employee Self-Service Portal:**
- Description: Provides employees with a portal to manage personal information, record attendance, submit leave requests, and view payslips.
- Use Case: Organizes requirements for employee self-service functionalities.
- Mode of Operation: Includes processes for secure access and management of personal data.
- User Class: Targets employees for accessing and managing personal information securely.
- Object Class: Manages employee self-service data and transactions.
- Functional Hierarchy: Includes modules for personal information management, attendance recording, leave request submission, and payslip viewing.
- Combinations: Integrates use cases for seamless employee self-service functionality and data management.

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/ca391ba5-850d-4198-afa7-c684a7b913ad" alt="viewprof" style="width:500px;">
   <small>Figure 11: Viewing Personal Information</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/63248cad-d969-4384-846a-0fc9dbf46053" alt="timein" style="width:500px;">
   <small>Figure 12: Recording Time in</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/62e6e713-812d-432e-9010-8f0d1b1cc36c" alt="timeout" style="width:500px;">
   <small>Figure 13: Recording Time out</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/3c987bdc-f908-4411-a314-9a2f04171559" alt="sickleave" style="width:500px;">
   <small>Figure 14: Submitting Leave Request</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/d194b470-4fca-4192-b773-29ed95b9565a" alt="payslipv" style="width:500px;">
   <small>Figure 15: Viewing Payslip</small>

6. **Reporting Capabilities:**
- Description: Provides integrated analytics and reporting dashboards for payroll trends, attendance patterns, leave utilization, and other HR metrics.
- Use Case: Organizes requirements for generating and viewing various reports and analytics.
- Mode of Operation: Includes processes for generating and presenting analytical insights securely.
- User Class: Targets HR administrators and management for data-driven decision-making.
- Object Class: Manages data aggregation and visualization for reporting purposes.
- Functional Hierarchy: Includes modules for report generation, data visualization, and dashboard presentation.
- Combinations: Integrates use cases for seamless data analysis and reporting capabilities.
 
   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/19296a34-9114-4368-96dc-4c4556258216" alt="generatepaylip" width="500"/>
   <small>Figure 16: Generating Payslip Report</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/e6ece67b-6a3b-48f0-a3e0-c408c184fb27" alt="fdashboard" style="width:500px;">
   <small>Figure 17: Payroll Dashboard</small>

   <img src="https://github.com/Jasmin172002/AOOPSRS/assets/125138169/e8f0f4b6-806b-4d09-8f39-a27b9b4651de" alt="hrdash" width="500">
   <small>Figure 18: HR Dashboard</small>

7. **System Administrator Functionalities:**
- Description: Provides tools for system administrators to manage user accounts, roles, permissions, and access levels across the platform.
- Use Case: Organizes requirements for managing user accounts and access controls.
- Mode of Operation: Includes secure processes for user management and access control.
- User Class: Targets system administrators for managing platform-wide security and access policies.
- Object Class: Manages user accounts, roles, and permissions securely.
- Functional Hierarchy: Includes modules for user account management, role-based access control, and permission assignment.
- Combinations: Integrates use cases for seamless system administration and security management.

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/df351a08-5e1b-4bab-8683-e2250c6bea88" alt="newuser" style="width:500px;">
   <small>Figure 19: Adding a new user</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/54343d8d-eb68-4ab6-9081-a54eb73854e3" alt="ediuserr" style="width:500px;">
   <small>Figure 20: Editing user information and Resetting Password</small>

   <img src="https://github.com/Jasmin172002/documentation/assets/125138169/f0fd1962-e11e-4b8c-9369-1ea841425289" alt="delete" style="width:500px;">
   <small>Figure 21: Viewing and Deleting User</small>

### Non-functional Requirements

- **Performance:** The system should handle multiple concurrent users without performance degradation, ensuring timely payroll processing and report generation.
   
- **Scalability:** The system should accommodate growing employee numbers and increased data volume.
   
- **Security:** Strong authentication, authorization mechanisms, and data encryption must protect sensitive information, ensuring compliance with data privacy regulations.
   
- **Usability:** An intuitive interface should require minimal training for end-users.
   
- **Reliability:** The system should have minimal downtime, ensuring continuous availability.
   
- **Maintainability:** Modular design facilitates easy maintenance and updates, supported by comprehensive documentation.
   
- **Compliance:** The system must adhere to relevant payroll regulations and standards.

---

## Appendix

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

### Use Case Diagram

[![UseCaseDiagram](https://github.com/Jasmin172002/documentation/assets/125138169/4db3b507-c970-4494-ade5-8b21aa7bc433)](https://github.com/Jasmin172002/documentation/assets/125138169/4db3b507-c970-4494-ade5-8b21aa7bc433)
<small>Figure 22: Use Case Diagram of the Expanded Payroll System</small>

The use case diagram illustrates the various interactions between different actors and the payroll system. Below is an explanation of the use case diagram components:

Actors:
- Employee: Interacts with personal account details, attendance records, payslip viewing, leave requests, and time tracking.
- Payroll Administrator: Manages payroll reports, payslip generation, and payroll summaries.
- IT Administrator: Handles system security and user role management.
- HR Administrator: Manages employee records, attendance, leave requests, and approvals.

Use Cases:
- Employee:
  - Time Tracking: Records time in and time out.
  - View Payslip: Access payslips by month or year.
  - View Leave Status: Check approved leave request status.
  - Login: Secure access to the system.
  - Manage Leave: View remaining leave credits and submit leave requests.

- IT Administrator:
  - Role Management: Administers role-based access control.
  - User Management: Manages user accounts.

- Payroll Administrator:
  - Generate Reports: Creates monthly payroll reports and summaries.
  - Generate Payslip: Calculates and saves employee payslips.

- HR Administrator:
  - Employee Management: Adds, modifies, and deletes employee records.
  - Attendance and Leave: Monitors attendance records and manages leave requests.

Interactions:
- All actors log in to access their respective functionalities.
- Generate Payslip involves computing allowances, deductions, and saving payslips.
- Role-Based Access Control ensures secure user access across the system.
- HR Administrator manages employee records, attendance, and leave requests.

### Class Diagram

[![AOOP_S2101 (3)](https://github.com/Jasmin172002/documentation/assets/125138169/6f12c90b-2fd4-47ce-8e9d-b4e0de974db1)](https://github.com/Jasmin172002/documentation/assets/125138169/6f12c90b-2fd4-47ce-8e9d-b4e0de974db1)
<small>Figure 23: Class Diagram of the Expanded Payroll System</small>

This class diagram illustrates the relationships and dependencies between key classes in the payroll system, defining how data flows and interacts within the system's architecture.

Classes and Associations:
- Employee
  - 1..* Department
  - 1..* Allowance
  - 1..1 Timesheet (Composition)
  - 1..* Payslip (Aggregation)
  - 1..1 User (Association)
  - 1..* Role (Aggregation)
  - 1..* LeaveRequest (Association)

- Allowance
  - 1..* Employee

- EmployeePayrollSummaryReport
  - 1..* Deduction (Composition)
  - 1..* Timesheet (Composition)
  - 1..1 Payslip (Aggregation)

- Tax
  - 1..1 TaxCategory (Association)

- Timesheet
  - 1..1 Employee

- Payslip
  - 1..* PayslipViewer (Association)
  - 1..* PayslipImpl (Inheritance)

- User
  - 1..1 Employee

- Role
  - 1..1 Permission (Aggregation)

- Position
  - 1..* Employee

- LeaveRequest
  - 1..1 LeaveRequestCategory (Association)

### Entity-relationship Diagram (ERD)

![Entity Relationship Diagram for MotorPH Payroll System drawio](https://github.com/Jasmin172002/AOOPSRS/assets/125138169/50ba213b-0766-4e13-9ec2-8b0a219c3d8d)
  <small>Figure 24: Entity-Relationship Diagram (ERD) of the Expanded Payroll System</small>

  The figure above represents the entity relationships for the payroll system. Below is the list of entities:

- Employee
- Allowance
- Deduction
- Payslip
- Tax
- Tax Category
- Leave Request
- Leave Request Category
- Position
- Timesheet
- User
- Role
- Permission
- Department

The relationships within the ERD outline the connections between different entities, defining how they interact and correlate with each other:

- **Employee - Position:**
  This one-to-many relationship ensures that each employee is associated with one or more positions within the organization, while each position can be occupied by multiple employees.

- **Employee - Timesheet:**
  In this one-to-many relationship, each employee can have multiple timesheet entries, but each timesheet entry is linked to only one employee, facilitating accurate tracking of work hours.

- **Employee - Payslip:**
  This one-to-many relationship allows each employee to have multiple payslips, with each payslip uniquely associated with one employee, streamlining payroll management.

- **Employee - Allowance:**
  The one-to-many relationship between employee and allowance permits each employee to have multiple allowances, ensuring flexible compensation options tailored to individual employee needs.

- **Employee - Deduction:**
  With a one-to-many relationship, each employee can have multiple deductions, while each deduction entry is linked to only one employee, simplifying payroll deductions.

- **Employee - Leave Request:**
  This one-to-many relationship enables each employee to submit multiple leave requests, ensuring efficient management of employee absences and vacation time.

- **Employee - Department:**
  In this one-to-one relationship, each employee is associated with only one department, ensuring clear organizational structure and hierarchy.

- **Allowance - Payslip:**
  The one-to-one relationship between payslip and allowance ensures that each payslip corresponds to a single total allowance amount, maintaining accuracy in payroll calculations.

- **Payslip - Deduction:**
  The one-to-one relationship between payslip and deduction ensures that each payslip corresponds to a single total deduction amount, maintaining accuracy in payroll calculations.

- **Leave Request - Leave Request Category:**
  This one-to-one relationship links each leave request to a specific category, facilitating proper categorization and management of employee leave requests.

- **Employee - User:**
  The one-to-one relationship between employee and user associates each employee with a unique user account, ensuring secure access to system resources.

- **User - Role:**
  In this one-to-one relationship, each user is linked to exactly one role, defining their permissions and access rights within the system.

- **Role - Permission:**
  With a one-to-many relationship, each role can have multiple permissions associated with it, allowing for flexible and granular control over system access and functionality.


### Demo Video


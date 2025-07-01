# ✈SkyLink Airway Reservation System

A comprehensive airline reservation and operations management system for SkyLink Airways. This Oracle APEX-based application handles flight bookings, passenger records, baggage tracking, employee assignments, and airport operations with a focus on efficiency, accuracy, and role-based access control.

---

## Project Objectives

* Enable fast and easy flight reservations.
* Manage passenger, ticketing, baggage, and flight schedules.
* Support employee records and airport assignments.
* Provide operational reports and analytics.
* Enforce data validation and secure user access.

---

## 🛠Technologies Used

* **Oracle APEX** for application development
* **PL/SQL** for business logic (functions, procedures, triggers)
* **Oracle Database** for relational data management

---

## Key Modules & Features

### Airports

* View airport list and details.
* Assign employees to airports.

### Employees

* Manage employee information and roles.
* Assign employees to flights or airports.
* Role-based access via user management.

### Flights

* View and manage flight details.
* Assign flight schedule, departure, and arrival info.
* Validations for logical flight time entry.

### Tickets

* Book and issue tickets linked to passengers.
* Seat assignment validation (1-200 seats).

### Baggage

* Track baggage ID and weight.
* Validate max baggage weight.

### Passengers

* Maintain passenger records.
* Associate passengers with tickets and baggage.

---

## PL/SQL Components

### Functions:

* Calculate total baggage weight per passenger.
* Get total ticket count per flight.

### Stored Procedures:

* Assign employee to an airport.
* Update employee salary.

### Triggers:

* Prevent past flight departure times.
* Restrict seat numbers outside 1-200.

---

## Reports & Charts

| Report Type | Description                                      |
| ----------- | ------------------------------------------------ |
| IR          | Employee Details, Passenger Baggage              |
| Classic     | Flight Schedule, Employees & Airport Details     |
| Charts      | Seat Type Distribution, Flight by Airport        |
| Calendar    | Flight schedule overview with color coding       |
| Summary     | Monthly Flight Revenue, Employee Salary Analysis |

---

## Master-Detail Forms

* Airport ➔ Employees
* Passenger ➔ Baggage

---

## Calculated Items & Dynamic Actions

* Auto-calculate flight duration.
* Full name concatenation for employees and passengers.
* Show/hide fields based on context.
* Enable/disable buttons based on form completion.
* Alert on deletions.

---

## Security & User Roles

### Roles & Permissions

* **Administrator**: Full access + user management
* **Contributor**: Can edit content in assigned modules
* **Reader**: View-only access

### Users

* Total: 9 users assigned across 3 roles
* Sample users: AAESHA, AHMED, SARA, KHALID

Access is enforced using Oracle APEX security and visibility controls per role.

---

## Screenshots

* User roles and login view



<img width="452" alt="image" src="https://github.com/user-attachments/assets/bfc56826-1ba6-425b-84bd-990c925a0c16" />

* Admin panel access


<img width="452" alt="image" src="https://github.com/user-attachments/assets/cf6c57a0-ef17-4b3f-b62f-7e8b97f98a51" />

* Read-only forms based on roles




<img width="452" alt="image" src="https://github.com/user-attachments/assets/00946602-1862-4de3-9d5a-199b932b75dc" />


* Editable forms based on roles




<img width="452" alt="image" src="https://github.com/user-attachments/assets/5e881546-e18e-4b93-9c95-aeedbfdf6db5" />

---

## Entity Relationship Model (ERD)

Entities:

* **Passenger**: Personal & passport info
* **Ticket**: Seat, passenger ID, flight ID
* **Flight**: Departure/arrival info, airport IDs
* **Employee**: Name, position, salary, airport
* **Airport**: Location data
* **Baggage**: ID, weight, passenger link

---

## 💼 Authors

* CIA4203 - Enterprise Database Applications - Group Project (2025)

---

## 🔧 How to Use

1. Log in using your assigned role.
2. Navigate to modules via the sidebar.
3. Perform operations based on your role (Admin/Contributor/Reader).
4. Use reports and charts for operational insights.

---

## 📖 License

This project is developed for academic purposes only under CIA4203.

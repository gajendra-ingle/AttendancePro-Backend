# AttendancePro Rest API Documentation 

## About the Project

**AttendancePro** is a Spring Boot REST API project designed to streamline the process of managing student attendance in educational institutions. It allows faculty members to record attendance for specific subjects and provides interfaces for viewing and managing these records.

### Objective

- Automate attendance tracking through a REST API to streamline integration with existing systems.
- Ensure data accuracy with automated validation and storage of attendance records.
- Facilitate seamless integration with educational platforms to enhance faculty and administrative workflows.

### Scope of the Project

The project involves developing a REST API to manage student attendance, including functionalities for handling Students, Subjects, Faculty, and Attendance Records.


## Project Structure

AttendancePro follows a **layered architecture pattern**:

1. **Controller Layer**: Handles HTTP requests, validates input, and sends responses.
2. **Service Layer**: Contains business logic and coordinates between controllers and DAOs.
3. **DAO Layer**: Manages database interactions using CRUD operations.

### Responsibilities of Each Layer

- **Controller Layer**
  - Handle incoming HTTP requests.
  - Validate request parameters and payload.
  - Invoke appropriate methods in the service layer.
  - Format and return HTTP responses.

- **Service Layer**
  - Implement business logic and rules.
  - Coordinate interactions between controllers and DAOs.
  - Perform data manipulation and transformation.
  - Manage transactions and ensure data integrity.

- **DAO Layer**
  - Provide CRUD operations for accessing and modifying data.
  - Translate database queries and commands into SQL.
  - Abstract database-specific details from the service layer.


## Technology Stack

- **Backend Framework**: Spring Boot 2.5.6
- **Database**: MySQL 8
- **Database Framework**: Hibernate 5.6
- **Java**: JDK 17
- **Build Tool**: Maven
- **Development Environment**: Eclipse
- **API Testing Tool**: Postman


## Modules in the Project

1. **Student Module**
2. **Subject Module**
3. **Faculty Module**
4. **Attendance Module**
5. **User Module**

### API Endpoints Overview

#### **Student Module**
- `GET /student/get-all-students`: Fetches all students.
- `POST /student/add-student`: Creates a new student.
- `GET /student/get-student-by-id/{id}`: Fetches details of a student by ID.
- `PUT /student/update-student`: Updates an existing student's details.
- `DELETE /student/delete-student/{id}`: Deletes a student by ID.

#### **Subject Module**
- `GET /subject/get-all-subjects`: Fetches all subjects.
- `POST /subject/add-subject`: Creates a new subject.
- `GET /subject/get-subject-by-id/{id}`: Fetches details of a subject by ID.
- `PUT /subject/update-subject`: Updates an existing subject.
- `DELETE /subject/delete-subject/{id}`: Deletes a subject by ID.

#### **Faculty Module**
- `GET /faculty/get-all-faculties`: Fetches all faculty members.
- `POST /faculty/add-faculty`: Creates a new faculty member.
- `GET /faculty/get-faculty-by-id/{id}`: Fetches details of a faculty member by ID.
- `PUT /faculty/update-faculty`: Updates an existing faculty member.
- `DELETE /faculty/delete-faculty/{id}`: Deletes a faculty member by ID.

#### **Attendance Module**
- `GET /attendance/get-all-attendance-records`: Retrieves all attendance records.
- `POST /attendance/add-attendance`: Creates a new attendance record.

#### **User Module**
- `POST /user/login-user`: Authenticates a user.
- `POST /user/register-user`: Registers a new user.
- `GET /user/get-user-by-username/{username}`: Fetches details of a user by username.
- `GET /user/get-all-user`: Fetches all users.
- `DELETE /user/delete-user/{username}`: Deletes a user by username.


## Database

An Entity-Relationship (ER) diagram defines relationships between entities such as Students, Subjects, Faculty, and Attendance Records. 

![ER Diagram](/ER-Diagram.png)



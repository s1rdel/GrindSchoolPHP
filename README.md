# GrindSchoolSYS

**GrindSchoolSYS** is a PHP and MySQL-based web application designed to manage tutoring sessions ("grinds") for a school or educational center. It includes functionality to manage tutors, subjects, and session bookings. Student-related features are planned but not yet implemented.

This project is still in progress. Student management features are not yet developed.

##  Database Structure

The database is named `GrindSchoolSYS` and includes the following tables:

- `Grinds` – Represents tutoring sessions
- `StudentGrind` – Maps students to grinds
- `Students` – Stores student information
- `StudentSubject` – Maps students to subjects
- `Subjects` – List of available subjects
- `Tutors` – Tutor information

SQL initialization script: **`GrindSchoolSYS.sql`**

## Features

###  Subject Management
- **Add Subject**: Fill in a form to add a new subject to the database.
- **Delete Subject**: Enter a subject name from the list. If the subject is not linked to any tutor, it will be successfully deleted.

###  Tutor Management
- **Add Tutor**: Add new tutors through a form.
- **Update Tutor**: Select a tutor by ID, edit their information, and submit to save changes.
- **Remove Tutor**: Remove a tutor from the system by marking their status as “D”.

###  Grind Booking System
- **Book Grind**:
  - Select a student and subject.
  - Available grinds for that subject will appear.
  - Clicking the "Book" button will assign the grind to the student and reduce capacity by 1.

- **Update Grind**:
  - Modify date, time, capacity, and status of a grind.

- **Cancel Grind**:
  - Select a student to view their booked grinds.
  - Click “Cancel Grind” to cancel it and increase the grind’s capacity by 1.

##  In Progress

- **Student Management** (Add, Update, Remove) is under development and will mirror the tutor management features.

##  Requirements
- PHP (>= 7.x)
- MySQL Server
- Web server (e.g., Apache)

##  Setup Instructions
1. Import the `GrindSchoolSYS.sql` file into your MySQL database.
2. Configure your database connection in the PHP files (if needed).
3. Deploy the project to a local or remote web server with PHP support.
4. Access the application via your browser.


Feel free to contribute or fork the project for your own use.

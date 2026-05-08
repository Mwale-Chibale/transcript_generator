#  METU Student Transcript Management System

This system allows for management and generation of student transcripts based on department, curriculum, and course data using object-oriented Python and CSV files. It includes a user-friendly CLI and dynamic transcript generation in HTML format.

---

##  Features

### CSV-Based Data Loading
- **Department, Course, Student Import**: Loads from `departments.csv`, `courses.csv`, `students.csv`.
- **Curriculum Mapping by Department ID**: Dynamically loads curriculum from CSV using a department-to-curriculum mapping.

### Student Transcript Operations
- **Student ID Validation**: Ensures valid 7-digit student ID.
- **Individual Transcript Download**: Fetch and generate transcript for a specific student.
- **Bulk Transcript Download**: Generate transcripts for all students in a department.
- **HTML Transcript Output**: Transcripts are exported in clean HTML format.

### Department & Student Management
- **View All Departments**: Displays a list of all departments with their IDs.
- **List All Students**: Prints detailed info about all students.

### GPA and Curriculum Handling
- **Curriculum Loader**: Loads curriculum with prerequisites for a student’s department.
- **Dynamic Course Assignment**: Courses and grades are randomly loaded from mock data.
- **Transcript Generator**: Computes semester GPAs, CGPAs, and passed credits.

###  Utility Functions
- `isValidStudent_id(student_id: str) -> bool`: Validates 7-digit numeric student IDs.
- `is_valid_semester_format(semester: str) -> bool`: Checks if semester follows `YYYYx` format.
- `translate_semester_type(semester: str) -> str`: Translates semester codes to readable terms (e.g., `20231` → `Fall 2023–2024`).

### Menu-Driven CLI
- **User Interaction**: Menu loop with options to view students, departments, or generate transcripts.
- **Validation & Error Handling**: Handles invalid IDs and input with meaningful error messages.

---

## Data Files Required
- `departments.csv`
- `courses.csv`
- `students.csv`
- Curriculum files:
  - `SNG_CURRICULUM_1.csv` (Software Engineering)
  - `cng_curriculum.csv` (Computer Engineering)
  - `cyg_curriculum.csv` (CyberSecurity Engineering)

---

## Mock Data Source
- Predefined mock data like `data_cng_1`, `data_cyg_1`, etc., used to simulate enrolled courses and grades for testing.

---

## Potential Enhancements
- Export transcript as PDF
- User login/authentication
- Transcript download history/logs
- GUI interface using PySide6, Tkinter, or Flask Web App
- SQLite or Firebase backend integration

---

## Technologies Used
- Python 3+
- Object-Oriented Programming
- CSV File Handling
- Regular Expressions
- Random Data Assignment
- HTML Generation

---

## Example Menu Output 
## Screenshot Example in HTML
![Screenshot_4-6-2025_12733_](https://github.com/user-attachments/assets/6cb20f90-9fc0-4ea4-ada9-8c29f4745d16)

## Screenshot Example in PDF

[Davis_Noah_transcript.pdf](https://github.com/user-attachments/files/20611047/Davis_Noah_transcript.pdf)


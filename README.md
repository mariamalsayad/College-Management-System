# College Management System

A C++ command-line application for managing student records. Built to practice object-oriented programming, standard library containers, and file handling through a menu-driven interface.

## Features

- Add students with an ID, name, major, and GPA.
- Prevent duplicate student IDs when adding records.
- View all students, search by ID, and delete records.
- Export student records to `students.txt` in comma-separated format.
- Start with 10 sample records for exploring the application.

## Technical Highlights

- **Object-oriented design:** represents records with a `Student` class.
- **Data structures:** stores records in `std::vector` and uses `std::map` to count students by major.
- **File handling:** writes records with `std::ofstream`.
- **Algorithms:** uses linear searches for ID lookup and duplicate detection.
- **Code organization:** separates the main application from student-related source and header files.

## Build and Run

Requires a C++ compiler with C++11 support or later. From the folder containing `main.cpp`, `student.cpp`, and `student.h`, run:

```bash
g++ -std=c++11 main.cpp student.cpp -o cms
./cms
```

Choose a numbered menu option to perform an action. Select **5** to export records or **0** to exit.

## Current Scope and Next Steps

Records are kept in memory during each session. Saving overwrites `students.txt`; saved records are not loaded at startup.

Planned improvements:

- Complete student updates, sorting, and Dean's List filtering, which currently appear as menu placeholders.
- Refine the dashboard's average GPA calculation and empty-record handling.
- Strengthen input validation and deletion feedback.
- Load saved records when the application starts.

## Author

Mariam Alsayad

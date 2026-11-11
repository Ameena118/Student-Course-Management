# Student Course Management System

A lightweight, browser-based course planner for recording semester courses, tracking credit units, and backing up course data.

## Features

- Add courses with a course code, title, and credit units
- View all saved courses in a clear table
- Search courses by code or title
- Calculate total credit units with a recursive method
- Save the course list to a JSON file and load it later
- Keep a browser-local copy between visits
- Validate course details and report invalid or duplicate entries

## Getting started

No installation or server is required. Download or clone this project, then open `student_course_manager.html` in a modern web browser.

## Using the app

1. Enter a course code, course title, and positive credit-unit value, then choose **Add course**.
2. Search by code or title using the search box.
3. Review the course count and total units above the course list.
4. Choose **Save to file** to download `my_courses.json`.
5. Choose **Load file** to restore a previously saved JSON course list.

Course codes are trimmed and converted to uppercase. Duplicate codes are rejected. Units must be greater than 0 and no more than 60. The browser copy uses local storage; exported JSON files can be kept as backups or used in another browser.

## Project files

| File | Description |
| --- | --- |
| `student_course_manager.html` | Complete application source; HTML, CSS, and JavaScript are in one file. |
| `Project_Report.md` | Short project report covering design, features, error handling, and recursion. |
| `Student_Course_Management_System_Submission.pdf` | Combined PDF with the report and full source listing. |

## Design notes

The `Course` class stores and normalizes course details. The `CourseManager` class adds and searches courses, validates loaded data, and calculates the unit total recursively. JSON import and export use the browser's built-in file and Blob APIs. Browser local storage preserves the current list on the same device.

## License

No license has been specified for this project.
# Student-Course-Management
Student Course Management

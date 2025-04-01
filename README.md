# Python YAML Use Case

## Overview
This project demonstrates how to read and process student information from a YAML file using Python. It provides functionalities to display all student records and filter them based on GPA.

## Features
- Read student data from a YAML file
- Display all student records
- Filter students by minimum GPA

## Prerequisites
Ensure you have Python installed on your system. You will also need the `pyyaml` library. Install it using:
```bash
pip install pyyaml
```

## Project Structure
```
project-directory/
│-- students.yaml
│-- app.py
│-- README.md
```

## YAML File Structure
Create a `students.yaml` file with the following structure:
```yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
  - name: Bob
    age: 22
    major: Mathematics
    gpa: 3.5
  - name: Charlie
    age: 20
    major: Physics
    gpa: 3.9
```

## How to Run
1. Ensure `students.yaml` and `app.py` are in the same directory.
2. Open a terminal in the project directory and run:
   ```bash
   python app.py
   ```
3. The script will display all student records and prompt you to enter a minimum GPA for filtering.

## Expected Output
```
All Students:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Bob, Age: 22, Major: Mathematics, GPA: 3.5
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9

Enter minimum GPA to filter students: 3.6

Students with GPA >= 3.6:
Name: Alice, Age: 21, Major: Computer Science, GPA: 3.8
Name: Charlie, Age: 20, Major: Physics, GPA: 3.9
```

## Code Explanation
### `app.py` Functions
- `load_data(file_path)`: Reads YAML file and loads data.
- `display_students(students)`: Prints all student records.
- `filter_students_by_gpa(students, min_gpa)`: Displays students with GPA above a given threshold.
- `main()`: Orchestrates program execution.

## Conclusion
This project showcases how to handle YAML files in Python efficiently. You can extend it by adding features like sorting, updating records, or saving changes back to the YAML file.
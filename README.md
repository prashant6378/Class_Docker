# Class_Docker
# Student Management System

A simple Python application that loads student data from a YAML file, displays it, and allows filtering based on GPA.

## Features

- Load student data from a YAML configuration file
- Display information for all students
- Filter and display students based on minimum GPA threshold
- Command-line interface for easy interaction

## Prerequisites

- Python 3.x
- PyYAML package

## Installation

1. Clone this repository or download the files
2. Install the required dependencies:

bash
pip install pyyaml


## Usage

1. Ensure you have both app.py and students.yaml in the same directory
2. Run the application:

bash
python app.py


3. Follow the prompts to filter students by GPA

## File Structure

- app.py - Main Python application
- students.yaml - YAML file containing student data

## YAML Data Format

The students.yaml file must follow this structure:

yaml
students:
  - name: John Doe
    age: 20
    major: Computer Science
    gpa: 3.8
  - name: Jane Smith
    age: 21
    major: Engineering
    gpa: 3.9


## Functions

- load_data(file_path): Loads data from the YAML file
- display_students(students): Displays information about all students
- filter_students_by_gpa(students, min_gpa): Filters and displays students with a GPA above the specified minimum
- main(): Entry point that orchestrates the program flow

## Example Output


All Students:
Name: John Doe, Age: 20, Major: Computer Science, GPA: 3.8
Name: Jane Smith, Age: 21, Major: Engineering, GPA: 3.9
Name: Mike Johnson, Age: 19, Major: Mathematics, GPA: 3.5
Name: Sarah Williams, Age: 22, Major: Physics, GPA: 4.0

Enter minimum GPA to filter students: 3.9

Students with GPA >= 3.9:
Name: Jane Smith, Age: 21, Major: Engineering, GPA: 3.9
Name: Sarah Williams, Age: 22, Major: Physics, GPA: 4.0


## Common Issues

- If you encounter YAML parsing errors, check your indentation and format in the students.yaml file
- Ensure you're using spaces (not tabs) for indentation in the YAML file
- Verify the file path if you get "file not found" errors

## License

This project is open source and available under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

# YAML Data Processing Experiment

This project demonstrates how to work with YAML files in Python, specifically focusing on processing student data. The application allows you to load student information from a YAML file, display all students, and filter them based on their GPA.

## Project Structure

```
.
├── README.md
├── requirements.txt
├── students.yaml
└── app.py
```

## Components

### 1. students.yaml
Contains the student data in YAML format. Each student entry includes:
- name
- age
- major
- gpa

Example:
```yaml
students:
  - name: Alice
    age: 21
    major: Computer Science
    gpa: 3.8
```

### 2. app.py
The main Python script that processes the YAML data. It includes several functions:

- `load_data(file_path)`: Loads and parses the YAML file
- `display_students(students)`: Displays information about all students
- `filter_students_by_gpa(students, min_gpa)`: Filters students based on minimum GPA
- `main()`: Orchestrates the program flow

### 3. requirements.txt
Lists the project dependencies:
- pyyaml==6.0.1

## Setup and Installation

1. Clone or download this repository
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the application:
   ```bash
   python app.py
   ```

2. The program will:
   - Display all students and their information
   - Prompt you to enter a minimum GPA value
   - Show students who meet or exceed the specified GPA threshold

## Example Output

<div align="center">
  <img src="/images/Screenshot 2025-04-01 154111.png">
</div>

## Features

- YAML file parsing using PyYAML
- Student data management
- GPA-based filtering
- Clean and organized code structure
- Error handling for file operations

## Technical Details

- The application uses `yaml.safe_load()` for secure YAML parsing
- Student data is stored in a list of dictionaries
- GPA filtering is implemented using list comprehension
- The program handles floating-point GPA values

## Dependencies

- Python 3.x
- PyYAML 6.0.1

## Notes

- Make sure both `app.py` and `students.yaml` are in the same directory
- The program expects valid YAML syntax in the input file
- GPA values should be numeric (floating-point numbers) 
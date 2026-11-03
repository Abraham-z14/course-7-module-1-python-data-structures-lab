# Student Data Management System

A Python project for practicing core data structures and efficient data-processing techniques using student records.

## Features

The project supports:

- Storing student records using lists and tuples
- Formatting student information for readable output
- Displaying multiple student records
- Filtering students by major
- Case-insensitive major searches
- Finding unique majors using sets
- Processing students by major using a generator expression

## Project Structure

```text
lib/
├── student_data.py
├── filters.py
├── data_processing.py
├── set_operations.py
└── data_generator.py

testing/
├── test_filters.py
├── test_data_processing.py
├── test_set_operations.py
└── test_data_generator.py
```

## Data Format

Students are represented as tuples containing:

```python
(student_id, student_name, major)
```

Example:

```python
(101, "Alice Johnson", "Computer Science")
```

## Implemented Functions

### `filter_students_by_major(student_list, major)`

Returns a new list containing only students whose major matches the requested major.

The comparison is case-insensitive and uses a list comprehension.

### `format_student_data(student)`

Converts a student tuple into a readable string.

Example output:

```text
ID: 101 | Name: Alice Johnson | Major: Computer Science
```

### `display_students(student_list)`

Loops through the student list and prints each student using `format_student_data()`.

### `unique_majors(student_list)`

Returns a set containing the unique majors found in the student records.

### `student_generator(student_list, major)`

Returns a generator containing students whose major matches the requested major.

Using a generator allows matching records to be processed one at a time instead of building another complete list in memory.

## Setup

Install the project dependencies:

```bash
pipenv install
```

Enter the virtual environment:

```bash
pipenv shell
```

This project uses Python 3.10.

## Testing

Run the complete test suite with:

```bash
pytest
```

The completed project currently passes all provided tests:

```text
7 passed
```

## Concepts Practiced

This lab demonstrates:

- Lists
- Tuples
- Sets
- List comprehensions
- Set comprehensions
- Generator expressions
- Loops
- Functions
- Modular Python code
- Automated testing with pytest

## Author

Abraham Zarate
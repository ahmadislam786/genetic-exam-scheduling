# Genetic Algorithm for University Exam Scheduling

## Introduction
This project aims to generate a schedule for university exams using a Genetic Algorithm (GA). The GA reads data from input files, optimizes the schedule to meet given constraints, and produces an output schedule satisfying both hard and soft constraints.

## Implementation Details
- **Language:** Python
- **Libraries Used:** Pandas, NumPy
- **Constraints:**
  - **Hard Constraints:**
    - An exam for each course.
    - Each student enrolled in at least 3 courses, with no more than 1 exam at a time.
    - Exams not held on weekends (Saturday, Sunday).
    - Exams between 9 am and 5 pm.
    - Each exam invigilated by a unique teacher, avoiding invigilation of two exams simultaneously or in a row.
  - **Soft Constraints:**
    - Break on Friday from 1-2 for all students and teachers.
    - Students not giving more than 1 exam consecutively.
    - Preferential scheduling for certain courses (e.g., MG before CS).
    - Faculty meeting scheduling.
- **Input:** Data for exams includes teachers’ names, students’ names, exam duration, courses, and allowed classrooms.
- **Output:** Schedule with classroom and starting time for each exam along with course code and invigilating teacher.

## Usage
1. **Setup:** Ensure Python is installed with required libraries.
2. **Data Preparation:** Prepare input files (courses.csv, teachers.csv, studentCourse.csv, studentNames.csv).
3. **Execution:** Run the provided Python script.
4. **Output:** Review generated schedules and fitness values.

## Results
The project produces schedules that fulfill all hard constraints and optimize soft constraints to a certain extent. Fitness values are displayed at each iteration, providing insights into the optimization process.

## Notebooks and Reports
- `main.ipynb`: Jupyter notebook containing the implementation code.
- `report.pdf`: Report detailing the implementation and results.

## Sample Output
Generated schedules and their fitness values are displayed in a proper tabular format within the notebook.

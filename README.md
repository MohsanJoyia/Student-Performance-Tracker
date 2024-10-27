Here’s a **Markdown** (`.md`) file for your **Student Performance Tracker** assignment:

---

### Student Performance Tracker

#### Objective
Develop a Student Performance Tracker in Python to allow teachers to:
- Input student scores
- Track performance across subjects
- Calculate statistics (e.g., averages)
- Provide feedback on pass/fail status

This project reinforces concepts in Object-Oriented Programming (OOP), loops, conditionals, and data structures (lists and dictionaries).

---

### Project Steps & Guidelines

#### Step 1: Design the Project

**Goal**: Define the project’s structure by identifying key actions.
- **Key Actions**: Add students, store grades, calculate averages, provide pass/fail feedback.
- **Data**: Student names, subjects, and grades.

---

#### Step 2: Class Design

Create classes for **Student** and **PerformanceTracker**.

- **Student Class**
  - **Attributes**:
    - `name`: Student’s name (string).
    - `scores`: List of integers representing scores in subjects (e.g., math, science, English).
  - **Methods**:
    - `calculate_average()`: Calculates average of the student's scores.
    - `is_passing()`: Checks if the student is passing all subjects (pass threshold: 40).

- **PerformanceTracker Class**
  - **Attributes**:
    - `students`: Dictionary where keys are student names and values are Student objects.
  - **Methods**:
    - `add_student()`: Adds a student and their scores to the tracker.
    - `calculate_class_average()`: Calculates the overall average for the class.
    - `display_student_performance()`: Displays each student's performance, average score, and pass/fail status.

---

#### Step 3: Input Handling

**Objective**: Enable user input for student names and scores with robust error handling.

- **Input Prompts**:
  - Request a student’s name.
  - Ask for grades in 3 subjects (e.g., math, science, English) as integers.
- **Error Handling**:
  - Use try-except blocks to handle non-numeric input errors.
  - If the user enters invalid input, prompt for correction.
- **Data Storage**:
  - Store data in a dictionary with the student's name as the key and a list of scores as the value.

---

#### Step 4: Data Processing

**Objective**: Calculate metrics such as:
1. Each student’s average score.
2. Each student’s pass/fail status based on a threshold (e.g., 40).
3. Overall class average.

- **Tasks**:
  - Use `calculate_average()` in the Student class to compute individual averages.
  - Check if any score is below 40 using `is_passing()` in the Student class.
  - Calculate the class average with `calculate_class_average()` in the PerformanceTracker class.

---

#### Step 5: Display Output

**Objective**: Present results in a readable format.

- **Output Content**:
  - Each student's name, average score, and pass/fail status.
  - Overall class average score.
- **Formatting**:
  - Use f-strings to ensure output is clear and easy to understand.

---

#### Step 6: Error Handling and Edge Cases

**Objective**: Make the system robust against common input errors.

- **Tasks**:
  - Prompt user to re-enter scores if non-numeric values are entered.
  - Handle cases where no students or scores are entered.

---

### Step-by-Step Implementation Guide

1. **Create the Student Class**
   - Define `Student` class with attributes `name` and `scores`.
   - Implement methods `calculate_average()` and `is_passing()`.

2. **Create the PerformanceTracker Class**
   - Define `PerformanceTracker` class with attribute `students` (dictionary).
   - Implement methods `add_student()`, `calculate_class_average()`, and `display_student_performance()`.

3. **Handle User Input**
   - Write a loop for teacher input on student names and scores.
   - Implement try-except for input validation.

4. **Calculate Averages and Display Performance**
   - For each student, calculate their average and pass/fail status.
   - Display each student's performance along with the class average.

---

#### Sample Output

```plaintext
Student Performance Summary:
Student: Alice, Average Score: 75.67, Status: Passing
Student: Bob, Average Score: 65.33, Status: Passing
Student: Charlie, Average Score: 39.50, Status: Needs Improvement

Class Average Score: 60.17
```

---

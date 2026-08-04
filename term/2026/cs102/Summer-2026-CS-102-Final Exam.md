# Summer 2026 CS 102: Final Exam

**Instructor:** Jim D. Pham  
**Term:** Summer 2026 
**Course: Introduction to C++ Programming
**Topic:** Dynamic 2D Arrays & Function Implementation in C++  

---

## Program Description
This assignment requires students to develop a C++ program that dynamically constructs and evaluates a two-dimensional matrix of random integers. The application prompts the user for custom grid dimensions, dynamically allocates memory for the matrix, populates it with random data, and computes comprehensive row, column, and total array analytics using specialized functions. The program displays the matrix using a stylized, user-friendly grid layout and summarizes key metrics in a structured dashboard.

---

## Instructions
Write a complete, well-documented C++ program that dynamically allocates a two-dimensional array of random integers based on user input, processes the data through specific functions, and prints summary metrics. 

### Course & Academic Integrity Requirements
1. **AI Acceptable Use & Code Ownership:** In accordance with the Course Policy, AI tools may be used solely as learning aids (e.g., concept exploration, logic review). Direct generation or blind copy-pasting of assignment code is strictly prohibited.
2. **Oral Defense & Code Review Prep:** You must be prepared to explain your submitted code line-by-line during a live code review. If you cannot explain the logic, algorithms, or pointers used, no credit will be awarded.
3. **Dynamic Memory Allocation & Deallocation:** Prompt the user to enter the number of rows and columns. Dynamically allocate memory for the 2D array, fill it with random integers, and ensure all allocated memory is properly freed before program exit.
4. **Meaningful & Creative Formatted Output:** Design a visually appealing, highly readable console output dashboard. Display the array elements inside a formatted matrix grid using aligned columns (`std::setw`) and visual borders. Provide meaningful labels, section banners, and structured statistical metrics so the user can easily interpret the analytical data.
5. **Output Metrics:** The program output must display:
   * Total number of rows and columns.
   * Metrics for each row: lowest, highest, and average values.
   * Metrics for each column: lowest, highest, and average values.
   * Grand total and overall average of all elements in the array.

---

## Required Functions
You must define and demonstrate the following functions in your program:

* `int getTotal(int** arr, int rows, int cols)`  
  Accepts a 2D array (pointer-to-pointer) and its dimensions, returning the total sum of all values in the array.
* `double getAverage(int** arr, int rows, int cols)`  
  Accepts a 2D array and its dimensions, returning the average of all values in the array.
* `int getRowTotal(int** arr, int cols, int rowIndex)`  
  Accepts a 2D array, column count, and a row subscript, returning the total sum of values in the specified row.
* `int getColumnTotal(int** arr, int rows, int colIndex)`  
  Accepts a 2D array, row count, and a column subscript, returning the total sum of values in the specified column.
* `int getHighestInRow(int** arr, int cols, int rowIndex)`  
  Accepts a 2D array, column count, and a row subscript, returning the highest value in that row.
* `int getLowestInRow(int** arr, int cols, int rowIndex)`  
  Accepts a 2D array, column count, and a row subscript, returning the lowest value in that row.

---

## Submission Guidelines & Checklist

Follow the three-stage development process to complete and submit your final exam assignment:

### Step 1: Develop & Validate Your Original Solution
1. Write and complete the exam assignment independently based on the course prompts and technical requirements.
2. Compile and execute your code locally using your IDE/compiler.
3. Verify that your program runs successfully and produces the correct output.
4. Take a clear screenshot of your running program's output window.

### Step 2: AI-Assisted Peer Review & Optimization
1. Once your original code compiles and runs successfully, present your source code to an AI assistant.
2. Treat the AI as a technical peer reviewer. Prompt it to review your code for efficiency, readability, memory management, and structural optimization.
3. Evaluate the suggestions provided by the AI. Implement the optimizations that improve your program while maintaining the required core functionality.
4. Compile and run your new, optimized code to verify it works flawlessly.
5. Take a clear screenshot of your optimized program's output window.

### Step 3: Comprehensive Technical Reflection
1. Write an in-depth analytical reflection paragraph (**5 to 10 sentences**) explaining your program design and execution.
2. Provide a detailed breakdown of your pointer-to-pointer memory allocation strategy, pointer arithmetic or subscripting logic, and how memory deallocation prevents leaks.
3. Discuss how conditional routing, boundary condition handling, and modular function architecture were structured to maintain data integrity.
4. Critically evaluate the feedback received from your AI peer reviewer during Step 2, explaining which specific optimizations (such as input stream safety, constant abstraction, or creative layout formatting) were integrated and why they enhanced enterprise-grade maintainability.

### Final Submission Checklist
Ensure you have gathered all required deliverables and upload **all components** to your assignment portal:

- [ ] **`Exam-<your name>-Original.cpp`** *(Your independent, fully functional source code before AI optimization)*
- [ ] **`Exam-<your name>-AI-Improved.cpp`** *(Your refined source code after implementing AI peer-review suggestions)*
- [ ] **Screenshot of your Original program output** *(Clear visual verification that your original code compiled and executed successfully)*
- [ ] **Screenshot of your AI-Improved program output** *(Clear visual verification that your optimized code compiles and executes successfully)*
- [ ] **Extended Technical Reflection Paragraph** *(An exhaustive 5–10 sentence analytical reflection covering dynamic memory architecture, pointer safety, algorithmic flow, and AI peer-review evaluation)*

---

## Grading Rubric (50 Points Total)

This assignment is evaluated using a 50-point rubric adapted from the course standard:

### 1. Program Logic & Functional Correctness (10 Points)
* **Core Requirements Implementation (4 Points):** Program successfully executes all required dynamic array operations, matrix metric calculations, and displays.
* **Conditional Logic & Flow (4 Points):** Correct pointer navigation, iteration loops, array subscripting, and memory management structures.
* **Boundary & Edge-Case Stability (2 Points):** Handles edge dimensions, valid limits, and boundary conditions without program crashes or dynamic memory leaks.

### 2. Defensive Programming & Data Validation (5 Points)
* **Input Validation Structures (2.5 Points):** Checks dimension bounds, verifies `std::cin` input stream state, and prevents illegal sizes before memory allocation.
* **Error Handling & Communication (2.5 Points):** Provides clear user prompts, error messaging, and clean exit routes on illegal inputs.

### 3. Architecture, Formatting & Meaningful Presentation (15 Points)
* **Elimination of Hardcoded Magic Values (5 Points):** Abstraction of parameters, grid boundaries, dynamic ranges, and display width formatting into named constants.
* **Console Representation & Meaningful Layout (5 Points):** Creative, structured terminal dashboard using formatted grid cells, informative row/column labels, and visual metric summaries.
* **Code Styling & Documentation (5 Points):** Consistent indentation, semantic variable naming, function prototypes, and concise logic comments.

### 4. Final Submission & Analysis (20 Points)
* **Original Deliverable (`Exam-<your name>-Original.cpp`) (3.5 Points):** Independent, working program implementing all baseline requirements.
* **AI-Improved Deliverable (`Exam-<your name>-AI-Improved.cpp`) (3.5 Points):** Refined code file demonstrating code optimization, defensive input checks, and improved structure.
* **Visual Execution Evidence (3 Points):** Terminal screenshots showing successful builds, creative dynamic grid rendering, and summary metrics output.
* **Extended Technical Reflection (5–10 Sentences) (10 Points):** A rigorous, heavily weighted analytical summary comprehensively detailing pointer mechanics, memory safety implementation, structural design choices, and a critical evaluation of AI peer-review integration.

---

## Expected Sample Output

Your program output should look clean, intuitive, and meaningful, similar to the following run:

```text
  
  Enter Number of Rows    : 5
  Enter Number of Columns : 10
  ...
  Provide your program’s output based on the requirements listed here.
  ...
```

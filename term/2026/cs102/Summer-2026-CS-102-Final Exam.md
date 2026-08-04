# Computer Science 102: Final Exam Assignment Specifications

**Instructor:** Jim D. Pham[cite: 2, 3, 4]  
**Term:** Summer 2026[cite: 1]  
**Topic:** Dynamic 2D Arrays & Function Implementation in C++[cite: 1]  

---

## Program Description
This assignment requires students to develop a C++ program that dynamically constructs and evaluates a two-dimensional matrix of random integers[cite: 1]. The application prompts the user for custom grid dimensions, dynamically allocates memory for the matrix, populates it with random data, and computes comprehensive row, column, and total array analytics using specialized functions[cite: 1]. The program displays the matrix using a stylized, user-friendly grid layout and summarizes key metrics in a structured dashboard.

---

## Instructions
Write a complete, well-documented C++ program that dynamically allocates a two-dimensional array of random integers based on user input, processes the data through specific functions, and prints summary metrics[cite: 1]. 

### Course & Academic Integrity Requirements
1. **AI Acceptable Use & Code Ownership:** In accordance with the Course Policy, AI tools may be used solely as learning aids (e.g., concept exploration, logic review)[cite: 2]. Direct generation or blind copy-pasting of assignment code is strictly prohibited[cite: 2].
2. **Oral Defense & Code Review Prep:** You must be prepared to explain your submitted code line-by-line during a live code review[cite: 2]. If you cannot explain the logic, algorithms, or pointers used, no credit will be awarded[cite: 2].
3. **Dynamic Memory Allocation & Deallocation:** Prompt the user to enter the number of rows and columns[cite: 1]. Dynamically allocate memory for the 2D array, fill it with random integers, and ensure all allocated memory is properly freed before program exit[cite: 1].
4. **Meaningful & Creative Formatted Output:** Design a visually appealing, highly readable console output dashboard. Display the array elements inside a formatted matrix grid using aligned columns (`std::setw`) and visual borders. Provide meaningful labels, section banners, and structured statistical metrics so the user can easily interpret the analytical data.
5. **Output Metrics:** The program output must display:
   * Total number of rows and columns[cite: 1].
   * Metrics for each row: lowest, highest, and average values[cite: 1].
   * Metrics for each column: lowest, highest, and average values[cite: 1].
   * Grand total and overall average of all elements in the array[cite: 1].

---

## Required Functions
You must define and demonstrate the following functions in your program[cite: 1]:

* `int getTotal(int** arr, int rows, int cols)`  
  Accepts a 2D array (pointer-to-pointer) and its dimensions, returning the total sum of all values in the array[cite: 1].
* `double getAverage(int** arr, int rows, int cols)`  
  Accepts a 2D array and its dimensions, returning the average of all values in the array[cite: 1].
* `int getRowTotal(int** arr, int cols, int rowIndex)`  
  Accepts a 2D array, column count, and a row subscript, returning the total sum of values in the specified row[cite: 1].
* `int getColumnTotal(int** arr, int rows, int colIndex)`  
  Accepts a 2D array, row count, and a column subscript, returning the total sum of values in the specified column[cite: 1].
* `int getHighestInRow(int** arr, int cols, int rowIndex)`  
  Accepts a 2D array, column count, and a row subscript, returning the highest value in that row[cite: 1].
* `int getLowestInRow(int** arr, int cols, int rowIndex)`  
  Accepts a 2D array, column count, and a row subscript, returning the lowest value in that row[cite: 1].

---

## Submission Guidelines & Checklist

Follow the three-stage development process to complete and submit your final exam assignment[cite: 4]:

### Step 1: Develop & Validate Your Original Solution
1. Write and complete the exam assignment independently based on the course prompts and technical requirements[cite: 4].
2. Compile and execute your code locally using your IDE/compiler[cite: 4].
3. Verify that your program runs successfully and produces the correct output[cite: 4].
4. Take a clear screenshot of your running program's output window[cite: 4].

### Step 2: AI-Assisted Peer Review & Optimization
1. Once your original code compiles and runs successfully, present your source code to an AI assistant[cite: 4].
2. Treat the AI as a technical peer reviewer. Prompt it to review your code for efficiency, readability, memory management, and structural optimization[cite: 4].
3. Evaluate the suggestions provided by the AI. Implement the optimizations that improve your program while maintaining the required core functionality[cite: 4].
4. Compile and run your new, optimized code to verify it works flawlessly[cite: 4].
5. Take a clear screenshot of your optimized program's output window[cite: 4].

### Step 3: Comprehensive Technical Reflection
1. Write an in-depth analytical reflection paragraph (**5 to 10 sentences**) explaining your program design and execution[cite: 3, 4].
2. Provide a detailed breakdown of your pointer-to-pointer memory allocation strategy, pointer arithmetic or subscripting logic, and how memory deallocation prevents leaks.
3. Discuss how conditional routing, boundary condition handling, and modular function architecture were structured to maintain data integrity.
4. Critically evaluate the feedback received from your AI peer reviewer during Step 2, explaining which specific optimizations (such as input stream safety, constant abstraction, or creative layout formatting) were integrated and why they enhanced enterprise-grade maintainability.

### Final Submission Checklist
Ensure you have gathered all required deliverables and upload **all components** to your assignment portal[cite: 4]:

- [ ] **`Exam-<your name>-Original.cpp`** *(Your independent, fully functional source code before AI optimization)*[cite: 4]
- [ ] **`Exam-<your name>-AI-Improved.cpp`** *(Your refined source code after implementing AI peer-review suggestions)*[cite: 4]
- [ ] **Screenshot of your Original program output** *(Clear visual verification that your original code compiled and executed successfully)*[cite: 4]
- [ ] **Screenshot of your AI-Improved program output** *(Clear visual verification that your optimized code compiles and executes successfully)*[cite: 4]
- [ ] **Extended Technical Reflection Paragraph** *(An exhaustive 5–10 sentence analytical reflection covering dynamic memory architecture, pointer safety, algorithmic flow, and AI peer-review evaluation)*[cite: 3, 4]

---

## Grading Rubric (50 Points Total)

This assignment is evaluated using a 50-point rubric adapted from the course standard[cite: 3]:

### 1. Program Logic & Functional Correctness (10 Points)[cite: 3]
* **Core Requirements Implementation (4 Points):** Program successfully executes all required dynamic array operations, matrix metric calculations, and displays[cite: 1, 3].
* **Conditional Logic & Flow (4 Points):** Correct pointer navigation, iteration loops, array subscripting, and memory management structures[cite: 1, 3].
* **Boundary & Edge-Case Stability (2 Points):** Handles edge dimensions, valid limits, and boundary conditions without program crashes or dynamic memory leaks[cite: 1, 3].

### 2. Defensive Programming & Data Validation (5 Points)[cite: 3]
* **Input Validation Structures (2.5 Points):** Checks dimension bounds, verifies `std::cin` input stream state, and prevents illegal sizes before memory allocation[cite: 3].
* **Error Handling & Communication (2.5 Points):** Provides clear user prompts, error messaging, and clean exit routes on illegal inputs[cite: 3].

### 3. Architecture, Formatting & Meaningful Presentation (15 Points)[cite: 3]
* **Elimination of Hardcoded Magic Values (5 Points):** Abstraction of parameters, grid boundaries, dynamic ranges, and display width formatting into named constants[cite: 3].
* **Console Representation & Meaningful Layout (5 Points):** Creative, structured terminal dashboard using formatted grid cells, informative row/column labels, and visual metric summaries[cite: 3].
* **Code Styling & Documentation (5 Points):** Consistent indentation, semantic variable naming, function prototypes, and concise logic comments[cite: 3].

### 4. Final Submission & Analysis (20 Points)[cite: 3]
* **Original Deliverable (`Exam-<your name>-Original.cpp`) (3.5 Points):** Independent, working program implementing all baseline requirements[cite: 3, 4].
* **AI-Improved Deliverable (`Exam-<your name>-AI-Improved.cpp`) (3.5 Points):** Refined code file demonstrating code optimization, defensive input checks, and improved structure[cite: 3, 4].
* **Visual Execution Evidence (3 Points):** Terminal screenshots showing successful builds, creative dynamic grid rendering, and summary metrics output[cite: 3, 4].
* **Extended Technical Reflection (5–10 Sentences) (10 Points):** A rigorous, heavily weighted analytical summary comprehensively detailing pointer mechanics, memory safety implementation, structural design choices, and a critical evaluation of AI peer-review integration[cite: 3, 4].

---

## Expected Sample Output

Your program output should look clean, intuitive, and meaningful, similar to the following run:

```text
  ===============================================================
    CS 102: DYNAMIC MATRIX ANALYZER
  ===============================================================
  [?] Enter Number of Rows    : 3
  [?] Enter Number of Columns : 4

  ===============================================================
    GENERATED MATRIX GRID
  ===============================================================
         Col  0  Col  1  Col  2  Col  3  
        +-------+-------+-------+-------+
  Row  0 |     42 |     87 |     15 |     99 |
        +-------+-------+-------+-------+
  Row  1 |     63 |     24 |     78 |     31 |
        +-------+-------+-------+-------+
  Row  2 |     10 |     95 |     52 |     84 |
        +-------+-------+-------+-------+

  ===============================================================
    ROW METRICS DASHBOARD
  ===============================================================
  | Row [ 0] | Min:  15 | Max:  99 | Sum:   243 | Avg:  60.75 |
  | Row [ 1] | Min:  24 | Max:  78 | Sum:   196 | Avg:  49.00 |
  | Row [ 2] | Min:  10 | Max:  95 | Sum:   241 | Avg:  60.25 |
  +-------------------------------------------------------------+

  ===============================================================
    COLUMN METRICS DASHBOARD
  ===============================================================
  | Col [ 0] | Min:  10 | Max:  63 | Sum:   115 | Avg:  38.33 |
  | Col [ 1] | Min:  24 | Max:  95 | Sum:   206 | Avg:  68.67 |
  | Col [ 2] | Min:  15 | Max:  78 | Sum:   145 | Avg:  48.33 |
  | Col [ 3] | Min:  31 | Max:  99 | Sum:   214 | Avg:  71.33 |
  +-------------------------------------------------------------+

  ===============================================================
    EXAM SUMMARY TOTALS
  ===============================================================
  * Matrix Dimensions : 3 x 4 (12 total elements)
  * Grand Total Sum   : 680
  * Overall Average   : 56.67
  ================================-------------------------------
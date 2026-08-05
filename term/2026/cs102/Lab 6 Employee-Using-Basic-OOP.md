# Lab 6: Employee Class & Object-Oriented Programming

**Instructor:** **[Jim D. Pham](https://github.com/devservice-ora/AI/blob/main/My%20Professional%20Portfolio.md)**

**Course:** Summer 2026 - CS-102 C++ Programming

---

## 1. Assignment Overview
Design and implement an `Employee` class in C++ to demonstrate your understanding of core Object-Oriented Programming (OOP) concepts, including class design, constructor overloading, mutators/accessors (getters/setters), and arrays of objects.

Additionally, this assignment requires following a three-stage development workflow—developing your original solution first, engaging an AI tool as a technical peer reviewer, and writing a brief reflection on the process.

---

## 2. Lab Assignment Requirements

### Class Requirements

#### Member Variables (Private)
* `name`: A `string` that holds the employee's name.
* `id`: An `int` variable that holds the employee's ID number.
* `department`: A `string` that holds the name of the department where the employee works.
* `position`: A `string` that holds the employee's job title.

#### Constructors (Public)
* **Full Constructor:** Accepts values as arguments for `name`, `id`, `department`, and `position` (in that order) and assigns them to the appropriate member variables.
* **Partial Constructor:** Accepts arguments for `name` and `id`. The `department` and `position` fields should be assigned empty strings (`""`).
* **Default Constructor:** Assigns empty strings (`""`) to the `name`, `department`, and `position` member variables, and `0` to the `id` member variable.

#### Accessor & Mutator Functions (Public)
* Write appropriate **mutator (setter)** functions that store values in these member variables.
* Write appropriate **accessor (getter)** functions that return the values in these member variables.

---

### Main Driver Requirements
Once you have written the `Employee` class, write a driver program (`main`) that creates an array of `Employee` objects to hold the following data:

| Name | ID | Department | Position |
| :--- | :--- | :--- | :--- |
| **John Doe** | 12345 | Engineering | Software Engineer |
| **Jack Smith** | 12346 | IT | System Administrator |
| **Robert Junior** | 12347 | Manufacturing | Vice President |

The program should store the data in the array of objects and then display the data for each employee on the screen in a clear, formatted layout.

---

## 3. C++ Starter Code Template
Use the following template as your starting point for Step 1:

```cpp
#include <iostream>
#include <string>
#include <iomanip>

using namespace std;

// Class Definition
class Employee {
private:
    // TODO: Declare member variables (name, id, department, position)

public:
    // TODO: Overloaded Constructor 1 (Full Parameter Constructor)
    
    // TODO: Overloaded Constructor 2 (Partial Parameter Constructor: name, id)
    
    // TODO: Default Constructor
    
    // TODO: Mutator functions (Setters)
    
    // TODO: Accessor functions (Getters)
};

int main() {
    // TODO: Declare an array or vector of Employee objects and populate them with the required data
    
    // TODO: Print header for formatted output
    
    // TODO: Loop through the array and display each employee's details using getters
    
    return 0;
} 
```

---

## 4. Sample Program Output
Your program's output should be formatted neatly into columns using output formatting stream manipulators (e.g., `std::setw`, `std::left`).

```text
Name              ID        Department      Position              
------------------------------------------------------------------
John Doe          12345     Engineering     Software Engineer     
Jack Smith        12346     IT              System Administrator  
Robert Junior     12347     Manufacturing   Vice President        
```

---

## 5. Step-by-Step Submission Instructions

### Step 1: Develop & Validate Your Original Solution
* Complete the code template independently based on the prompt above.
* Compile and execute your code locally using your IDE/compiler.
* Verify that your program runs successfully and produces the correct formatted output.
* *Note: Your original code must be fully functional before moving to the AI review stage.*
* Take a clear screenshot of your running program's output window.

### Step 2: AI-Assisted Peer Review & Optimization
* Present your completed source code to an AI assistant.
* Treat the AI as a technical peer reviewer. Prompt it to review your code for efficiency, readability, memory management, and structural optimization.
* Evaluate the suggestions provided by the AI. Implement optimizations that improve your program while maintaining the required core functionality.
* Compile and run your new, optimized code to verify it works flawlessly.
* Take a clear screenshot of your optimized program's output window.

### Step 3: Program Explanation & Reflection
* Write a brief paragraph (3–5 sentences) explaining your program.
* Describe the program's overall purpose, the logic behind your technical approach, and how you integrated or evaluated the feedback from your AI peer reviewer.

---

## 6. Final Submission Checklist

> **🛑 Final Check Before Submission**
> Before uploading your files to the assignment portal, verify the following:
> * **Does it compile?** Ensure both `.cpp` files compile without syntax errors.
> * **Are the screenshots clear?** Make sure terminal output screenshots are legible and clearly display successful execution.
> * **Are the files named correctly?** Double-check that your name replaces `<your name>` in the file names.

Submit all components below to the assignment portal:
* `Lab-<your name>-Original.cpp` *(Your independent, fully functional source code before AI optimization)*
* `Lab-<your name>-AI-Improved.cpp` *(Your refined source code after implementing AI peer-review suggestions)*
* **Screenshot of your Original program output** *(Clear visual verification of successful run)*
* **Screenshot of your AI-Improved program output** *(Clear visual verification of successful run)*
* **Program Explanation Paragraph** *(Your 3–5 sentence summary and reflection as described in Step 3)*

*Note: Missing any of the deliverables above will result in an incomplete submission or a deduction in grading points.*

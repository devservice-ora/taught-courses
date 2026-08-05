# Lab 5: Coffee Shop Point-of-Sale (POS) System Using Functions

**Instructor:** **[Jim D. Pham](https://github.com/devservice-ora/AI/blob/main/My%20Professional%20Portfolio.md)**

**Course:** Summer 2026 - CS-102 C++ Programming

---

## 1. Assignment Overview
This lab assignment requires students to design and implement a menu-driven C++ point-of-sale (POS) system for a coffee shop. Students will practice core programming concepts including user-defined functions, pass-by-reference parameter passing, named constants, input validation, and formatted text output.

This assignment lasts 2 weeks and is due on **8/2/2026**. Although it may seem complicated, this is actually a straightforward demonstration of user-defined functions.

---

## 2. Lab Assignment Requirements

### Problem Statement
You are opening a local coffee shop and sell coffee in three sizes: small (9 oz), medium (12 oz), and large (15 oz). The prices are:
* **Small:** $1.75
* **Medium:** $1.90
* **Large:** $2.00

Write a menu-driven C++ program that makes the coffee shop operational. The sales tax rate is **9.25%**.

---

### Functional Requirements
Your interactive menu must allow the user to perform the following operations at any time during execution:
1. **Buy coffee:** Choose any size and specify the number of cups to purchase.
2. **Show total cups sold:** Display the total count of small, medium, and large cups sold so far.
3. **Show total coffee volume:** Display the total amount of coffee sold in fluid ounces (oz).
4. **Show total revenue:** Display the subtotal, calculated sales tax, and total money made (including tax).

---

### Technical Requirements
* **No Global Variables:** All state variables must be kept local to `main()` and passed to functions as arguments. Use pass-by-reference (`&`) where functions need to update state variables in `main()`.
* **Named Constants:** Special values like sizes, prices per cup, and the sales tax rate must be declared as `const` variables.
* **Libraries:** Use `#include <iostream>` for I/O and `#include <iomanip>` for output formatting.
* **Formatting:** All monetary values (Subtotal, Sales Tax, and Grand Total) must display with exactly 2 decimal places and right-align numbers in the second column for readability.

---

### Required Functions
Your program must implement (at minimum) the following user-defined functions:
* `void showInstructions()` — Explains how to use the program.
* `void sellCoffee(...)` — Handles buying coffee and updates the count of cups sold using reference parameters.
* `void showCupsSold(...)` — Displays the count of each cup size sold.
* `void showTotalVolume(...)` — Calculates and prints total fluid ounces sold.
* `double calculateTax(double amount)` — Calculates and returns 9.25% sales tax for a given amount.
* `void showTotalMoney(...)` — Computes subtotal, calls `calculateTax()`, and prints the formatted monetary breakdown.

---

## 3. Student Code Starter Template
Use the following skeleton code as the starting point for your assignment. Fill in the missing function prototypes, parameter lists, and function implementations:

```cpp
#include <iostream>
#include <iomanip>

using namespace std;

// TODO: Declare Function Prototypes
void showInstructions();
// Declare prototypes for sellCoffee, showCupsSold, showTotalVolume, 
// calculateTax, and showTotalMoney here...


int main() {
    // Local state variables to track total cups sold
    int smallCupsSold = 0;
    int mediumCupsSold = 0;
    int largeCupsSold = 0;

    int choice = 0;

    // Display introductory instructions
    showInstructions();

    do {
        cout << "
-----------------------------------
";
        cout << "            MAIN MENU              
";
        cout << "-----------------------------------
";
        cout << "1: Buy Coffee
";
        cout << "2: Show Total Cups Sold
";
        cout << "3: Show Total Coffee Volume Sold
";
        cout << "4: Show Total Revenue
";
        cout << "5: Exit Program
";
        cout << "Enter choice: ";
        cin >> choice;

        cout << endl;

        switch (choice) {
            case 1:
                // TODO: Call sellCoffee function (pass parameters by reference)
                break;
            case 2:
                // TODO: Call showCupsSold function
                break;
            case 3:
                // TODO: Call showTotalVolume function
                break;
            case 4:
                // TODO: Call showTotalMoney function
                break;
            case 5:
                cout << "Thank you for using the Coffee Shop POS System. Goodbye!
";
                break;
            default:
                cout << "Invalid choice! Please select an option between 1 and 5.
";
        }
    } while (choice != 5);

    return 0;
}

// =================================================================
// FUNCTION IMPLEMENTATIONS
// =================================================================

// Explains how to use the program
void showInstructions() {
    cout << "====================================================
";
    cout << "        WELCOME TO THE COFFEE SHOP POS SYSTEM       
";
    cout << "====================================================
";
    cout << "Use the menu below to navigate the shop's operations.
";
    cout << "You can sell coffee, track inventory, and view full 
";
    cout << "financial summaries at any time.
";
}

// TODO: Implement sellCoffee
// Hint: Must update the cup counters in main using reference parameters (&)
void sellCoffee(/* Add parameters */) {
    // 1. Prompt user for size choice (1-3) and quantity
    // 2. Validate user input
    // 3. Update the corresponding counter variable
}

// TODO: Implement showCupsSold
// Displays total count of each cup size sold
void showCupsSold(/* Add parameters */) {
    // Use setw() and right/left formatting to align output columns
}

// TODO: Implement showTotalVolume
// Calculates total volume in ounces sold across all cup sizes
void showTotalVolume(/* Add parameters */) {
    // Named constants for sizes
    const int SMALL_OZ = 9;
    const int MED_OZ = 12;
    const int LARGE_OZ = 15;

    // Calculate and print total oz
}

// TODO: Implement calculateTax
// Returns 9.25% of the passed amount
double calculateTax(double amount) {
    const double TAX_RATE = 0.0925;
    // Calculate and return sales tax
    return 0.0; // Placeholder
}

// TODO: Implement showTotalMoney
// Computes subtotal, calculates sales tax using calculateTax(), and displays totals
void showTotalMoney(/* Add parameters */) {
    // Named constants for costs
    const double COST_SMALL = 1.75;
    const double COST_MED = 1.90;
    const double COST_LARGE = 2.00;

    // 1. Calculate subtotal
    // 2. Call calculateTax() to get tax amount
    // 3. Compute grand total
    // 4. Format output with 2 decimal places fixed (setprecision(2))
    // 5. Ensure second column is right-aligned
}
```

---

## 4. Expected Sample Run

```text
====================================================
        WELCOME TO THE COFFEE SHOP POS SYSTEM       
====================================================
Use the menu below to navigate the shop's operations.
You can sell coffee, track inventory, and view full 
financial summaries at any time.

-----------------------------------
            MAIN MENU              
-----------------------------------
1: Buy Coffee
2: Show Total Cups Sold
3: Show Total Coffee Volume Sold
4: Show Total Revenue
5: Exit Program
Enter choice: 1

Select Coffee Size:
1: Small  (9 oz)
2: Medium (12 oz)
3: Large  (15 oz)
Enter size (1-3): 1
Enter quantity: 3
Successfully added 3 cup(s) to total sales.

-----------------------------------
            MAIN MENU              
-----------------------------------
1: Buy Coffee
2: Show Total Cups Sold
3: Show Total Coffee Volume Sold
4: Show Total Revenue
5: Exit Program
Enter choice: 4

Subtotal:           $    5.25
Sales Tax (9.25%):  $    0.49
Total Amount Due:   $    5.74
```

---

## 5. Step-by-Step Instructions

### Step 1: Develop & Validate Your Original Solution
* Write and complete the lab assignment independently based on the course prompts and technical requirements.
* Compile and execute your code locally using your IDE/compiler.
* Verify that your program runs successfully and produces the correct output.
* *Note: Your original code must be fully functional before moving to the AI review stage.*
* Take a clear screenshot of your running program's output window.

### Step 2: AI-Assisted Peer Review & Optimization
* Once your original code compiles and runs successfully, present your source code to an AI assistant.
* Treat the AI as a technical peer reviewer. Prompt it to review your code for efficiency, readability, memory management, and structural optimization.
* Evaluate the suggestions provided by the AI. Implement the optimizations that improve your program while maintaining the required core functionality.
* Compile and run your new, optimized code to verify it works flawlessly.
* Take a clear screenshot of your optimized program's output window.

### Step 3: Program Explanation & Reflection
* Write a brief paragraph (3–5 sentences) explaining your program.
* Describe the program's overall purpose, the logic behind your technical approach, and how you integrated or evaluated the feedback from your AI peer reviewer.

---

## 6. Final Submission Checklist

> **🛑 STOP: Final Review Before Submission**
> Before uploading your files to the assignment portal, perform one final sanity check:
> * **Does it compile?** Ensure both `.cpp` files compile without syntax errors. Code that does not compile will not receive full credit.
> * **Are the screenshots clear?** Make sure your terminal output screenshots are legible and clearly display the successful execution of your programs.
> * **Are the files named correctly?** Double-check that your name replaces `<your name>` in the filenames exactly as specified below.

Submit all of the following components to your class assignment portal:
* `Lab-<your name>-Original.cpp` *(Your independent, fully functional source code before AI optimization)*
* `Lab-<your name>-AI-Improved.cpp` *(Your refined source code after implementing the AI peer-review suggestions)*
* **Screenshot of your Original program output** *(Clear visual verification that your original code compiled and executed successfully)*
* **Screenshot of your AI-Improved program output** *(Clear visual verification that your optimized code compiles and executes successfully)*
* **Program Explanation Paragraph** *(Your summary and reflection as indicated in Step 3, submitted either as a separate document or inline text as directed by the portal)*

*Note: Missing any of the deliverables above will result in an incomplete submission or a deduction in grading points.*

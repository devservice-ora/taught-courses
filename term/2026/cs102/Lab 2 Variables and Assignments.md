# Lab 2: Basic input and output, variables and assignments

This assignment covers the basics of using variables, doing math, and formatting text in C++.

You will build a simple store checkout program that:
* **Creates Variables and Assigns Values:** You will set up five variables to act as labeled containers for your data. You then use the assignment operator (`=`) to store a specific dollar amount inside each variable.
* **Performs Math Calculations:** The program will add the items to find the subtotal, calculate 9.25% sales tax, and sum them for the final total.
* **Prints the Receipt:** Finally, it prints the entire receipt on the screen using a single `cout` statement, with all prices neatly rounded to two decimal places.

Please follow the step-by-step instructions outlined below. Once you have verified that your original code compiles and runs successfully, use an AI assistant as a peer reviewer to optimize your work.

### Sample Output

```text
T-Shirt:        $14.95
Wireless Mouse: $23.95
Coffee Mug:     $5.95
Notebook:       $11.95
Charging Cable: $4.95
-------------------------
Subtotal:       $61.75
Sales Tax:      $5.71
Total:          $67.46

```

# Step-by-Step Instructions
## Step 1: Open Your IDE or Text Editor
Open your preferred programming environment (e.g., Visual Studio, VS Code, or OnlineGDB).

Create a new file and save your initial workspace draft as: Chapter 2_Lab-[YourName]-Original.cpp.

Step 2: Paste and Fill Out the Header
Copy the required comment block and paste it at the very top of your .cpp file. Replace the placeholder brackets with your actual details:

C++
```
***************************************************************
* Name: John Doe                                              *
* Description: Calculates total sale price of 5 distinct      *
* retail items using a single cout statement.                 *
* Course: CS 102 - Introduction to Programming C++            *
* Due Date: 07/05/2026                                        *
***************************************************************

```

## Step 3: Write Your Initial (Original) Code
Set up the basic structure using using namespace std;. Write your initial code using basic sequential variables (item1, item2, etc.) to hold the prices, compute the math, and chain the values into a single cout statement.

C++

```
#include <iostream>
#include <iomanip>
using namespace std;

int main() {
    // Original variables
    double item1 = 14.95, item2 = 23.95, item3 = 5.95, item4 = 11.95, item5 = 4.95;
    const double TAX_RATE = 0.0925;
    
    double subtotal = item1 + item2 + item3 + item4 + item5;
    double salesTax = subtotal * TAX_RATE;
    double total = subtotal + salesTax;
    
    cout << fixed << setprecision(2)
         << "Item 1: $" << item1 << "\n"
         << "Item 2: $" << item2 << "\n"
         << "Subtotal: $" << subtotal << "\n"
         << "Tax: $" << salesTax << "\n"
         << "Total: $" << total << "\n"; // (Truncated for brevity)
         
    return 0;
}

```

Compile this version, verify it works, and take a screenshot of your console output.

## Step 4: Ask AI to Improve Your Program
Once you have a working baseline, copy your entire code block and submit it to an AI assistant with a refinement prompt.

Example prompt to send the AI:

"Here is a working C++ program for my intro class. Please review it and provide an optimized, professional version. Specifically, help me refactor item1 through item5 into descriptive, camelCase variables representing real store items, improve the output console alignment so it looks like a real receipt, and explain the code changes."

## Step 5: Implement the AI-Improved Code
Review the AI's feedback. Create a brand-new file named Chapter 2_Lab-[YourName]-AI-Improved.cpp and implement the cleaner, self-documenting code.

Your updated file should look similar to this:

C++
```
    // AI-Improved descriptive item price variables
    double priceTshirt = 14.95;
    double priceWirelessMouse = 23.95;
    double priceCoffeeMug = 5.95;
    double priceNotebook = 11.95;
    double priceChargingCable = 4.95;

    // Calculations using descriptive names
    double subtotal = priceTshirt + priceWirelessMouse + priceCoffeeMug + 
                      priceNotebook + priceChargingCable;
    double salesTax = subtotal * 0.0925;
    double total = subtotal + salesTax;

    // Aligned and polished single cout receipt output
    cout << fixed << setprecision(2)
         << "T-Shirt:        $" << priceTshirt << "\n"
         << "Wireless Mouse: $" << priceWirelessMouse << "\n"
         << "-------------------------\n"
         << "Subtotal:       $" << subtotal << "\n"; // (Truncated for brevity)

```

## Step 6: Compile and Take Your Screenshots
Compile and run both programs to guarantee there are no hidden syntax errors.

Confirm both console outputs match the exact mathematical target:

Subtotal: $61.75

Sales Tax: $5.71

Total: $67.46

Capture crisp screenshots of both execution windows and save them as .jpg or .png files.

## Step 7: Final Submission Checklist
Before submitting, ensure you have gathered all required deliverables. Upload all components to your class assignment portal:

*   [ ] **`Lab-<your name>-Original.cpp`** (Your independent, fully functional source code before AI optimization)
*   [ ] **`Lab-<your name>-AI-Improved.cpp`** (Your refined source code after implementing the AI peer-review suggestions)
*   [ ] **Screenshot of your Original program output** (Clear visual verification that your original code compiled and executed successfully)
*   [ ] **Screenshot of your AI-Improved program output** (Clear visual verification that your optimized code compiles and executes successfully)
*   [ ] **Program Explanation Paragraph** (Your summary and reflection as indicated in Step 3, submitted either as a separate document or inline text as directed by the portal)
        
**Note:** Missing any of the deliverables above will result in an incomplete submission or a deduction in grading points.

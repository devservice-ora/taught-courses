# Lab 2: Basic input and output, variables and assignments with AI-Assisted Peer Review

Instructor: Jim D. Pham

Course: Fall 2026 - CS-142 Pythron Programming

---

## Assignment Overview
This assignment covers the basics of using variables, doing math, and formatting text in Python.
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
Open your preferred programming environment (e.g., VS Code, PyCharm, OnlineGDB, or Replit).
Create a new file and save your initial workspace draft as: Chapter2_Lab-[YourName]-Original.py


Step 2: Paste and Fill Out the Header
Copy the required comment block and paste it at the very top of your .py file. Replace the placeholder brackets with your actual details:

Python
```
***************************************************************
* Name: John Doe                                              *
* Description: Calculates total sale price of 5 distinct      *
* retail items using a single cout statement.                 *
* Course: CS 142 - Introduction to Python                     *
* Due Date: 11/01/2026                                        *
***************************************************************

```

## Step 3: Write Your Initial (Original) Code
Write your initial code using basic sequential variables (item1, item2, etc.) to hold the prices, compute the math, and chain the values into a single print() statement using f-strings for formatting.

Python

```
# Original variables
item1 = 14.95
item2 = 23.95
item3 = 5.95
item4 = 11.95
item5 = 4.95

TAX_RATE = 0.0925

subtotal = item1 + item2 + item3 + item4 + item5
sales_tax = subtotal * TAX_RATE
total = subtotal + sales_tax

# Single print statement with newline characters (\n)
print(f"Item 1: ${item1:.2f}\n"
      f"Item 2: ${item2:.2f}\n"
      f"Subtotal: ${subtotal:.2f}\n"
      f"Tax: ${sales_tax:.2f}\n"
      f"Total: ${total:.2f}\n") # (Truncated for brevity)
```

Run this script, verify it works, and take a screenshot of your console output.

## Step 4: Ask AI to Improve Your Program
Once you have a working baseline, copy your entire code block and submit it to an AI assistant with a refinement prompt.

Example prompt to send the AI:

"Here is a working Python program for my intro class. Please review it and provide an optimized, professional version. Specifically, help me refactor item1 through item5 into descriptive, snake_case variables representing real store items, improve the output console alignment so it looks like a real receipt, and explain the code changes."

## Step 5: Implement the AI-Improved Code
Review the AI's feedback. Create a brand-new file named Chapter2_Lab-[YourName]-AI-Improved.py and implement the cleaner, self-documenting code.

Your updated file should look similar to this:

Python
```
# AI-Improved descriptive item price variables
price_tshirt = 14.95
price_wireless_mouse = 23.95
price_coffee_mug = 5.95
price_notebook = 11.95
price_charging_cable = 4.95

# Calculations using descriptive names
subtotal = (price_tshirt + price_wireless_mouse + price_coffee_mug + 
            price_notebook + price_charging_cable)
sales_tax = subtotal * 0.0925
total = subtotal + sales_tax

# Aligned and polished single print receipt output using a multi-line f-string
print(f"""T-Shirt:        ${price_tshirt:.2f}
Wireless Mouse: ${price_wireless_mouse:.2f}
-------------------------
Subtotal:       ${subtotal:.2f}
Sales Tax:      ${sales_tax:.2f}
Total:          ${total:.2f}""")
Step 6: Run and Take Your Screenshots
Run both programs to guarantee there are no hidden syntax errors.
Confirm both console outputs match the exact mathematical target:

Subtotal: $61.75

Sales Tax: $5.71

Total: $67.46
```

## Step 6: Compile and Take Your Screenshots
Run both programs to guarantee there are no hidden syntax errors.
Confirm both console outputs match the exact mathematical target:

Subtotal: $61.75

Sales Tax: $5.71

Total: $67.46

Capture crisp screenshots of both execution windows and save them as .jpg or .png files.

## Step 7: Final Submission Checklist
Before submitting, ensure you have gathered all required deliverables. Upload all components to your class assignment portal:

*   [ ] **`Lab-<your name>-Original.py`** (Your independent, fully functional source code before AI optimization)
*   [ ] **`Lab-<your name>-AI-Improved.y`** (Your refined source code after implementing the AI peer-review suggestions)
*   [ ] **Screenshot of your Original program output** (Clear visual verification that your original code compiled and executed successfully)
*   [ ] **Screenshot of your AI-Improved program output** (Clear visual verification that your optimized code compiles and executes successfully)
*   [ ] **Program Explanation Paragraph** (Your summary and reflection as indicated in Step 3, submitted either as a separate document or inline text as directed by the portal)
        
**Note:** Missing any of the deliverables above will result in an incomplete submission or a deduction in grading points.

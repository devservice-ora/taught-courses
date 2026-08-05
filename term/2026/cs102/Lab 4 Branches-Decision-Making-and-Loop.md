# Lab 4: Savings Account Balance Using Branches, Decision-Making, and Loop

**Instructor:** **[Jim D. Pham](https://github.com/devservice-ora/AI/blob/main/My%20Professional%20Portfolio.md)**

**Course:** Summer 2026 - CS-102 C++ Programming

---

## 1. Assignment Description
This program calculates the final balance of a savings account over a user-specified period of time measured in months. It applies an iterative simulation model to accurately track cumulative deposits, withdrawals, and compounding monthly interest, while continuously monitoring the account integrity to detect and prevent negative balances.

---

## 2. Core Objectives & Logic Flow
* **User Input Initialization:** The program prompts the user to enter the account's annual interest rate, the starting balance, and the total number of months the account has been open.
* **Input Validation:** It verifies that the starting balance is valid (greater than or equal to zero). If the balance is invalid, the program outputs an error and terminates immediately.
* **Monthly Iteration Loop:** Using a `for` loop, the program steps through each individual month sequentially to process transaction history, updating running totals for deposits, withdrawals, and balance updates.
* **Interest Compounding:** Calculates monthly interest based on the standard financial formula:
$$\text{Monthly Interest} = \left(\frac{\text{Annual Interest Rate}}{12}\right) \times \text{Current Balance}$$
This interest is accumulated and added to the balance.
* **Formatted Reporting:** Once the simulation finishes, the program generates a neatly aligned, professional text report displaying the final balances and totals formatted strictly to two decimal places.

---

## 3. Step-by-Step Implementation Guide

### Step 1: Initialize Accumulators & Prevent Garbage Data
Before the loop begins, ensure all your total tracking variables (`total_deposits`, `total_withdrawals`, `total_interest_earned`) are explicitly initialized to `0.0`. Also, set your `updated_balance` equal to the `starting_balance` provided by the user.

```cpp
double total_deposits = 0.0;
double updated_balance = starting_balance;
```

### Step 2: Streamline the Loop Structure
Instead of checking if `month == 1` inside the loop body, seed the `updated_balance` before entering the loop. This eliminates duplicated math blocks and allows a single, clean sequence of operations for every iteration.

> A uniform math path applies from `month = 1` to `number_of_months` without duplicate logic blocks.

### Step 3: Implement Monthly Transaction Logic
Within each iteration of the `for` loop, prompt the user for the specific month's deposit and withdrawal. Add the deposit and subtract the withdrawal from the running `updated_balance`, then accumulate these values into your tracking variables.

* **Example:** If current balance is $1000.00, deposit is $200.00, withdrawal is $50.00:
$$\text{updated\_balance} = 1000.00 + 200.00 - 50.00 = 1150.00$$

### Step 4: Enforce Immediate Account Validation
Immediately after applying transactions, check if `updated_balance` has dropped below $0. If it has, print the negative balance/account closure warning and exit the application immediately using `return -1`.

```cpp
if (updated_balance < 0) {
    cout << "Account closed due to negative balance.\n";
    return -1;
}
```

### Step 5: Apply Compounding Monthly Interest
If the balance remains positive, compute the interest earned for that month using the monthly breakdown formula. Add this result to `total_interest_earned` and update the running `updated_balance`.

* **Example:** If annual rate is 12% (0.12) and balance is $1150.00:
$$\text{Monthly Interest} = \left(\frac{0.12}{12}\right) \times 1150.00 = 11.50$$

### Step 6: Format and Align Output Reports
Once the loop terminates successfully, use stream manipulators (`<iomanip>`) including `setprecision(2)`, `fixed`, `left`, `right`, and `setw` to output a polished, tabular summary financial report.

```cpp
cout << fixed << setprecision(2);
cout << left << setw(45) << "Ending Balance:" << right << "$" << setw(10) << updated_balance;
```

---

## 4. C++ Starter Program Template
Use the following scaffold structure to build out your implementation. Ensure you replace the placeholder comments with your active math logic statements:

```cpp
#include <iostream>
#include <iomanip>

using namespace std;

int main()
{
    // Variable declarations
    double starting_balance, annual_interest_rate;
    double deposit_per_month, withdrawal_per_month, monthly_interest;

    // Initializing tracking accumulators to prevent garbage data
    double updated_balance = 0.0;
    double total_deposits = 0.0;
    double total_withdrawals = 0.0;
    double total_interest_earned = 0.0;
    int number_of_months = 0;

    // TODO: Prompt for interest rate and starting balance

    // TODO: Perform input validation on starting_balance

    // Simulation loop
    for (int month = 1; month <= number_of_months; month++)
    {
        // 1. Prompt for current month deposits/withdrawals

        // 2. Adjust updated_balance & update total accumulators

        // 3. Check for account insolvency (< 0), terminate if true

        // 4. Calculate monthly interest & add to balance
    }

    // TODO: Output final financial summary using <iomanip> manipulators

    return 0;
}
```

---

## 5. Sample Program Output
When executing correctly, your program terminal interaction and final summary alignment must match the format below:

```text
Enter the annual interest rate as a decimal (e.g., 0.05 for 5%): 0.05
Enter the starting balance of your account: $10000.00
Enter the number of months that your bank account has been open: 3
Enter the amount deposited during month 1: $500.00
Enter the amount withdrawn during month 1: $200.00
Enter the amount deposited during month 2: $0.00
Enter the amount withdrawn during month 2: $150.00
Enter the amount deposited during month 3: $1200.00
Enter the amount withdrawn during month 3: $300.00
----------------------------------------------------------------
The ending balance of your account is:       $  11116.53
The total amount you have deposited is:      $   1700.00
The total amount you have withdrawn is:      $    650.00
The total amount of interest earned is:      $    116.53
```

---

## 6. Laboratory Requirements & Evaluation Criteria

### Step 2: AI-Assisted Peer Review & Optimization
1. Once your original code compiles and runs successfully, present your source code to an AI assistant.
2. Treat the AI as a technical peer reviewer. Prompt it to review your code for efficiency, readability, memory management, and structural optimization.
3. Evaluate the suggestions provided by the AI. Implement the optimizations that improve your program while maintaining the required core functionality.
4. Compile and run your new, optimized code to verify it works flawlessly.
5. Take a clear screenshot of your optimized program's output window.

### Step 3: Program Explanation & Reflection
Write a brief paragraph (3–5 sentences) explaining your program. Describe the program's overall purpose, the logic behind your technical approach, and how you integrated or evaluated the feedback from your AI peer reviewer.

---

## 7. Final Submission Checklist

> **🛑 STOP:** Before submitting, ensure you have gathered all required deliverables.

Submit all of the following components to your class assignment portal:
* `Lab-<your name>-Original.cpp` *(Your independent, fully functional source code before AI optimization)*
* `Lab-<your name>-AI-Improved.cpp` *(Your refined source code after implementing the AI peer-review suggestions)*
* **Screenshot of your Original program output** *(Clear visual verification that your original code compiled and executed successfully)*
* **Screenshot of your AI-Improved program output** *(Clear visual verification that your optimized code compiles and executes successfully)*
* **Program Explanation Paragraph** *(Your summary and reflection as indicated in Step 3, submitted either as a separate document or inline text as directed by the portal)*

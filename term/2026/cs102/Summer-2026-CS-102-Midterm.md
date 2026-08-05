# Summer 2026 CS 102: Midterm

**Instructor:** Jim D. Pham  

**Term:** Summer 2026 

**Course:** Introduction to C++ Programming

**Topic:** A basic interest rate calculator in C++ with data input and output.

## Program Description
This midterm programming assignment challenges you to develop a C++ Interest Calculator that processes loan data, handles structured data storage, and outputs formatted results. You will write a program that prompts the user for a loan amount and an interest rate, calculates the corresponding interest, and stores these records dynamically. The final structured data must be formatted similarly to the console interaction example using `<iomanip>` and written to both the console and an external output file.

To complete this assignment, you will follow a software development workflow:
1. **Develop** a fully functional, independent original solution.
2. **Review & Optimize** your code by using an AI assistant as a technical peer reviewer.
3. **Reflect** on your implementation choices and the AI's suggestions in a brief written explanation.

---

## 2. Problem Description & Specifications
Use the concepts from your zyBooks Chapters 1–5 to write a C++ program that calculates the interest on a loan, stores the results dynamically, and displays the final output to both the console and an external file.

### Technical Specifications
* **Interest Formula:** Use the formula: `loan_amount * (interest_rate / 100)` to calculate interest.
* **Rounding:** Round the final calculated interest to exactly 2 decimal places.
* **Console Formatting:** Display the loan amount and interest with 2 decimal places, and the rate with 3 decimal places using `<iomanip>`.
* **Data Storage:** Store the history of each column (Amount, Rate, and Interest) dynamically in separate, parallel vectors.
* **User Input Assumption:** You may assume that the user will enter valid decimal values for both the loan amount and the interest rate.

---

## 3. Console Interaction Example

```text
Interest Calculator

Enter loan amount:
520000
Enter interest rate: 5.375
Interest amount:
27950.00

Continue? (y/n): y

Enter loan amount:
4944.5
Enter interest rate: 1.3
Interest amount:
64.28

Continue? (y/n): n

AMOUNT      RATE     INTEREST
520000.00   5.375    27950.00
4944.50     1.300    64.28

Bye!
```

---

## 4. Step-by-Step Instructions

### Step 1: Develop & Validate Your Original Solution
Independently write your C++ program (`Lab-<your name>-Original.cpp`) based on the specifications. Ensure you utilize separate parallel vectors to store the calculation history.

> **💡 Hint:** Don't forget to include the `<vector>` library at the top of your program (`#include <vector>`) to work with C++ dynamic arrays!

Compile and execute your code locally to ensure it is completely functional before moving onto the AI peer-review. Take a clear, legible screenshot of your running original program's console window.

### Step 2: AI-Assisted Peer Review & Optimization
Present your C++ source code to an AI assistant and treat it as a technical peer reviewer. Prompt it to evaluate your code's runtime efficiency, readability, vector usage, and structure.

Evaluate and selectively implement the suggestions. Compile and test your optimized code, saving it as `Lab-<your name>-AI-Improved.cpp`. Capture a screenshot of this program's output window.

### Step 3: Program Explanation & Reflection
Write a structured, brief paragraph of 3 to 5 sentences that covers the overall purpose of your Interest Calculator, explains the technical logic of your modular vector-based design, and reflects on the specific optimization suggestions you chose to accept or decline and why.

---

## 5. Final Sanity Check & Submission Checklist

> **🛑 STOP:** Before uploading your files, ensure:
> * Both files compile without syntax errors. Non-compiling code will receive zero functionality points.
> * Your screenshots are sharp and fully readable.
> * Your name replaces `<your name>` in your C++ filenames exactly.

Ensure you submit the following **5 distinct deliverables**:
1. `Lab-<your name>-Original.cpp` *(Your original fully working independent code)*
2. `Lab-<your name>-AI-Improved.cpp` *(Your optimized code post AI peer-review)*
3. Screenshot of your original code's execution output
4. Screenshot of your optimized code's execution output
5. Your 3–5 sentence reflection paragraph *(submitted inline or as directed)*

---

## 6. Midterm Grading Rubric (50 Points Total)

| Deliverable / Criteria | Excellent (Full Marks) | Developing (Partial Credit) | Unsatisfactory (No Credit) |
| :--- | :--- | :--- | :--- |
| **Original Program Logic & Functionality**<br>*(20 Points)* | **18–20 points**<br>• Code compiles with no errors.<br>• Stores history in parallel C++ vectors.<br>• Correctly uses `<iomanip>` decimal formatting.<br>• Highly modular. | **10–17 points**<br>• Minor execution bugs.<br>• Missing one or more layout/formatting rules.<br>• Missing parallel vectors to store history. | **0–9 points**<br>• Code does not compile.<br>• Major logical errors or incomplete solution. |
| **AI Optimization & Refinement**<br>*(10 Points)* | **9–10 points**<br>• Optimized code compiles flawlessly.<br>• Demonstrates logical improvements in code quality, readability, safety, or speed. | **5–8 points**<br>• Code compiles but shows minimal change.<br>• Weak application of peer feedback. | **0–4 points**<br>• Code does not compile.<br>• No evidence of AI collaboration. |
| **Execution Screenshots**<br>*(10 Points total / 5 pts each)* | **5 points each**<br>• Clear, legible terminal screenshot verifying proper input/output matching specifications. | **3–4 points each**<br>• Screenshots provided but blurry, cropped, or partially unreadable. | **0 points**<br>• Missing screenshot(s). |
| **Explanation & Reflection**<br>*(10 Points)* | **9–10 points**<br>• Detailed 3–5 sentence reflection.<br>• Clear breakdown of logic and AI feedback decisions. | **5–8 points**<br>• Reflection is too short (< 3 sentences).<br>• Analysis is superficial or vague. | **0–4 points**<br>• Missing explanation.<br>• Fails to reflect on AI peer-review. |

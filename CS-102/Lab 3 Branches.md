# Lab 3: Branches and Making Decisions - Bank Charges Calculator

**Instructor:** Jim D. Pham  
**Course Requirement:** Three-Stage Development Process (Independent Design, AI Peer Review, Reflection)

---

## Assignment Overview
In this assignment, you will create a C++ application to calculate monthly fees for commercial checking accounts based on a bank's pricing model.

This project will help you practice using conditional logic (like if-else statements), simple math, and checking user input for errors. You will need to calculate fees based on the number of checks written, determine whether any low-balance fees apply, and correctly handle user input errors (such as negative check counts or overdrafts).

---

## 1. Problem Description & Logic Requirements

A bank charges **$10 per month** plus the following tiered check fees for a commercial checking account:
*   **$2.50 each** for fewer than 20 checks
*   **$1.50 each** for 20–39 checks
*   **$1.00 each** for 40–59 checks
*   **$.50 each** for 60 or more checks

### Additional Fees & Input Validation Constraints:
1.  **Low Balance Fee:** The bank charges an extra **$15** if the account balance falls below **$400** (evaluated *before* any check fees are applied).
2.  **Input Validation A:** Do not accept a negative value for the number of checks written.
3.  **Input Validation B:** If a negative value is given for the beginning balance, display an urgent message indicating the account is overdrawn.

Your program must prompt the user for the beginning balance and the number of checks written, compute the final fees, and display the total monthly service charges.

---

## 2. Step-by-Step Instructions

To receive full credit for this programming lab assignment, you must strictly follow this three-stage development process before uploading your files:

### Step 1: Develop & Validate Your Original Solution
1.  **Write and complete** the lab assignment independently based on the course prompts and technical requirements.
2.  **Compile and execute** your code locally using your IDE/compiler.
3.  **Verify** that your program runs successfully and produces the correct output.
    *   *Note:* Your original code must be fully functional before moving to the AI review stage.
4.  **Take a clear screenshot** of your running program's output window.

### Step 2: AI-Assisted Peer Review & Optimization
1.  Once your original code compiles and runs successfully, present your source code to an AI assistant.
2.  **Treat the AI as a technical peer reviewer**. Prompt it to review your code for efficiency, readability, memory management, and structural optimization.
3.  **Evaluate the suggestions** provided by the AI. Implement the optimizations that improve your program while maintaining the required core functionality.
4.  **Compile and run** your new, optimized code to verify it works flawlessly.
5.  **Take a clear screenshot** of your optimized program's output window.

### Step 3: Program Explanation & Reflection
1.  Write a brief paragraph (**3-5 sentences**) explaining your program.
2.  Describe the program's overall purpose, the logic behind your technical approach, and how you integrated or evaluated the feedback from your AI peer reviewer.

---

## 3. Final Review Before Submission
Before uploading your files to the assignment portal, perform one final sanity check:
*   **Does it compile?** Ensure **both** `.cpp` files compile without syntax errors. Code that does not compile will not receive full credit.
*   **Are the screenshots clear?** Make sure your terminal output screenshots are legible and clearly display the successful execution of your programs.
*   **Are the files named correctly?** Double-check that your name replaces `<your name>` in the filenames exactly as specified below.

---

## 4. Final Submission Checklist
Before submitting, ensure you have gathered all required deliverables. Upload all components to your class assignment portal:

*   [ ] **`Lab-<your name>-Original.cpp`** (Your independent, fully functional source code before AI optimization)
*   [ ] **`Lab-<your name>-AI-Improved.cpp`** (Your refined source code after implementing the AI peer-review suggestions)
*   [ ] **Screenshot of your Original program output** (Clear visual verification that your original code compiled and executed successfully)
*   [ ] **Screenshot of your AI-Improved program output** (Clear visual verification that your optimized code compiles and executes successfully)
*   [ ] **Program Explanation Paragraph** (Your summary and reflection as indicated in Step 3, submitted either as a separate document or inline text as directed by the portal)

*Note: Missing any of the deliverables above will result in an incomplete submission or a deduction in grading points.*

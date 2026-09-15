# EXPERIMENT 5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

### Date: 05-09-2026
### Name: NITHISHKUMAR S
### Register no.212223240109

## PROJECT TITLE

**REVIORA – AI-Based Code Review System**

---

## AIM

To compare different prompting techniques and evaluate their effectiveness in solving a real-world software engineering problem using an AI-based automated code review scenario from the **REVIORA – AI Code Review System** project.

---

# AI TOOLS REQUIRED

* ChatGPT

---

# EXPERIMENT OVERVIEW

**REVIORA** is an AI-based code review system designed to analyze source code and provide meaningful feedback to developers. The system aims to identify common programming issues such as bugs, inefficient code, security vulnerabilities, poor coding practices and maintainability problems.

Traditional code review requires developers or reviewers to manually inspect source code. This can be time-consuming, especially when reviewing large amounts of code. REVIORA uses Artificial Intelligence to assist developers by automatically analyzing submitted code and generating review comments.

For this experiment, the selected engineering problem is:

> **How can an AI-based code review system analyze a given source code, identify programming issues, explain the problems clearly and provide practical suggestions for improving the code?**

The same code-review problem was given to ChatGPT using four different prompting techniques. The generated responses were then compared based on **relevance, accuracy, completeness, clarity, feasibility and usefulness**.

---

# SELECTED ENGINEERING SCENARIO

The following Python code contains a potential programming problem.

```python
def calculate_average(numbers):
    total = 0

    for i in range(len(numbers)):
        total = total + numbers[i]

    average = total / len(numbers)

    return average


numbers = []
print("Average:", calculate_average(numbers))
```

### Problem in the Code

The function attempts to calculate the average of a list of numbers. However, when an empty list is passed, `len(numbers)` becomes zero and the program attempts to perform division by zero.

This can result in:

```text
ZeroDivisionError: division by zero
```

### Expected AI Review

The AI code review system should:

* Identify the error.
* Explain why the error occurs.
* Suggest a correction.
* Provide improved code.
* Mention relevant edge cases.
* Give a clear and practical review.

---

# PROMPTING TECHNIQUE 1 – STRAIGHTFORWARD PROMPT

## Prompt

> Review the following Python code and identify any errors or problems. Explain the problem and suggest how to fix it.
>
> ```python
> def calculate_average(numbers):
>     total = 0
>
>     for i in range(len(numbers)):
>         total = total + numbers[i]
>
>     average = total / len(numbers)
>
>     return average
>
> numbers = []
> print("Average:", calculate_average(numbers))
> ```

## AI-GENERATED OUTPUT

The AI identified that the code can produce a **ZeroDivisionError** when the list is empty.

The problem occurs because:

```python
average = total / len(numbers)
```

attempts to divide by zero when `numbers` contains no elements.

### Suggested Solution

The function should check whether the list is empty before calculating the average.

```python
def calculate_average(numbers):
    if len(numbers) == 0:
        return 0

    total = sum(numbers)
    return total / len(numbers)
```

### Observation

The straightforward prompt successfully identified the main error and provided a basic correction. However, it did not request a detailed review of other aspects such as efficiency, edge cases or code quality.

---

# PROMPTING TECHNIQUE 2 – ROLE-BASED PROMPTING

## Prompt

> Act as a senior Python software engineer performing a professional code review for the REVIORA AI Code Review System. Analyze the following Python code. Identify bugs, edge cases, code-quality issues and possible improvements. Explain each issue clearly and provide corrected code.
>
> ```python
> def calculate_average(numbers):
>     total = 0
>
>     for i in range(len(numbers)):
>         total = total + numbers[i]
>
>     average = total / len(numbers)
>
>     return average
>
> numbers = []
> print("Average:", calculate_average(numbers))
> ```

## AI-GENERATED OUTPUT

### Issue 1 – Division by Zero

The function fails when an empty list is supplied.

```python
average = total / len(numbers)
```

If the list is empty:

```text
len(numbers) = 0
```

which causes a `ZeroDivisionError`.

### Issue 2 – Edge Case Not Handled

The function does not define what should happen when the input list is empty.

### Issue 3 – Unnecessary Loop

The following code:

```python
for i in range(len(numbers)):
    total = total + numbers[i]
```

can be simplified using Python's built-in `sum()` function.

### Improved Code

```python
def calculate_average(numbers):
    if not numbers:
        return 0

    return sum(numbers) / len(numbers)


numbers = []
print("Average:", calculate_average(numbers))
```

### Observation

Role-based prompting produced a more professional review. The AI not only identified the main bug but also considered code quality and efficiency.

---

# PROMPTING TECHNIQUE 3 – CONSTRAINT-BASED PROMPTING

## Prompt

> Review the following Python code as part of the REVIORA AI Code Review System.
>
> Follow these constraints:
>
> 1. Identify all runtime errors that can occur.
> 2. Identify important edge cases.
> 3. Identify inefficient or unnecessarily complex code.
> 4. Explain the cause of each problem.
> 5. Provide corrected code.
> 6. Do not change the intended purpose of the program.
> 7. Use standard Python practices.
> 8. Keep the solution simple and readable.
> 9. Mention the time complexity where relevant.
> 10. Present the review using the format: **Issue → Explanation → Severity → Recommendation → Corrected Code**.
>
> Code:
>
> ```python
> def calculate_average(numbers):
>     total = 0
>
>     for i in range(len(numbers)):
>         total = total + numbers[i]
>
>     average = total / len(numbers)
>
>     return average
>
> numbers = []
> print("Average:", calculate_average(numbers))
> ```

## AI-GENERATED OUTPUT

### Issue 1: Division by Zero

**Explanation:**
If `numbers` is empty, `len(numbers)` is zero. The division operation therefore raises a `ZeroDivisionError`.

**Severity:** High

**Recommendation:**
Check whether the input list is empty before calculating the average.

---

### Issue 2: Empty Input

**Explanation:**
The function does not define how an empty input should be handled.

**Severity:** Medium

**Recommendation:**
Return an appropriate value or raise a meaningful exception.

---

### Issue 3: Unnecessary Iteration

**Explanation:**
The loop manually calculates the sum of the list.

**Severity:** Low

**Recommendation:**
Use Python's built-in `sum()` function.

---

### Corrected Code

```python
def calculate_average(numbers):
    if not numbers:
        return 0

    return sum(numbers) / len(numbers)


numbers = []
print("Average:", calculate_average(numbers))
```

### Complexity

The improved implementation has:

* **Time Complexity:** O(n)
* **Space Complexity:** O(1)

### Observation

The constraint-based prompt generated a highly structured code review. It identified the runtime error, edge case and unnecessary complexity while following the requested review format.

---

# PROMPTING TECHNIQUE 4 – STEP-BY-STEP PROMPTING

## Prompt

> Perform a systematic code review for the REVIORA AI Code Review System.
>
> Analyze the following code using these steps:
>
> **Step 1:** Understand the intended functionality of the program.
>
> **Step 2:** Trace the code using the given input.
>
> **Step 3:** Identify runtime errors and logical errors.
>
> **Step 4:** Identify edge cases that are not handled.
>
> **Step 5:** Identify opportunities for improving code quality and efficiency.
>
> **Step 6:** Provide corrected code while preserving the original functionality.
>
> **Step 7:** Provide a concise final review containing the issue, severity, explanation and recommendation.
>
> Code:
>
> ```python
> def calculate_average(numbers):
>     total = 0
>
>     for i in range(len(numbers)):
>         total = total + numbers[i]
>
>     average = total / len(numbers)
>
>     return average
>
> numbers = []
> print("Average:", calculate_average(numbers))
> ```

## AI-GENERATED OUTPUT

### Step 1 – Understand the Function

The function is designed to calculate the average value of all numbers in a list.

### Step 2 – Trace the Given Input

The input is:

```python
numbers = []
```

Therefore:

```python
len(numbers) = 0
```

The loop does not execute because the list contains no elements.

The variable:

```python
total = 0
```

remains unchanged.

The program then executes:

```python
average = total / len(numbers)
```

which becomes:

```python
average = 0 / 0
```

### Step 3 – Identify Error

The operation results in:

```text
ZeroDivisionError
```

### Step 4 – Edge Case

The empty-list case is not handled.

### Step 5 – Code Quality

The manual loop can be replaced with Python's `sum()` function.

### Step 6 – Corrected Code

```python
def calculate_average(numbers):
    if not numbers:
        return 0

    return sum(numbers) / len(numbers)


numbers = []
print("Average:", calculate_average(numbers))
```

### Step 7 – Final Review

**Issue:** Division by zero for empty input.

**Severity:** High

**Recommendation:** Validate the input before performing the division and simplify the summation using `sum()`.

### Observation

Step-by-step prompting produced the most systematic explanation because the AI was instructed to understand, trace, diagnose and improve the code in a specific sequence.

---

# COMPARISON OF PROMPTING TECHNIQUES

| Prompting Technique     | Relevance | Accuracy  | Completeness | Clarity   | Feasibility | Usefulness |
| ----------------------- | --------- | --------- | ------------ | --------- | ----------- | ---------- |
| Straightforward Prompt  | Good      | Very Good | Medium       | Good      | Very Good   | Good       |
| Role-Based Prompt       | Very Good | Very Good | Good         | Very Good | Very Good   | Very Good  |
| Constraint-Based Prompt | Excellent | Excellent | Excellent    | Excellent | Excellent   | Excellent  |
| Step-by-Step Prompt     | Excellent | Excellent | Excellent    | Excellent | Excellent   | Excellent  |

---

### Overall Finding

The experiment demonstrates that **prompt specificity and structure have a significant impact on AI-generated code review quality**.

For simple programming questions, a straightforward prompt may be sufficient. However, for an AI-based code review system, structured prompts provide better consistency and more useful feedback.

---

# RESULT

The experiment was successfully executed using ChatGPT for the **REVIORA – AI-Based Code Review System** project.

Four prompting techniques—**Straightforward Prompting, Role-Based Prompting, Constraint-Based Prompting and Step-by-Step Prompting**—were applied to the same software engineering problem.

The generated outputs were compared based on relevance, accuracy, completeness, clarity, feasibility and usefulness.

The **Constraint-Based and Step-by-Step prompting techniques produced the most comprehensive and structured code reviews**, while the straightforward prompt was sufficient for identifying the primary error.

The experiment confirms that **well-designed prompts can improve the effectiveness of AI-based code analysis by producing clearer, more accurate and actionable software engineering feedback.**

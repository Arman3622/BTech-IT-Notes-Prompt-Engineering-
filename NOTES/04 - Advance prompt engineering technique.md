# Chapter 4 — Advanced Prompt Engineering Techniques

> **Subject:** Generative AI / Prompt Engineering  
> **Chapter:** Advanced Prompt Engineering Techniques  
> **Purpose:** Long-term revision + upcoming examinations + practical AI usage

---

# Table of Contents

1. [Introduction](#1-introduction)
2. [What is Advanced Prompt Engineering?](#2-what-is-advanced-prompt-engineering)
3. [Prompt Chaining](#3-prompt-chaining)
4. [Strategic Role Player](#4-strategic-role-player)
5. [ReAct Prompting](#5-react-prompting)
6. [Iterative Self-Refinement](#6-iterative-self-refinement)
7. [Multi-Step Prompting](#7-multi-step-prompting)
8. [Hierarchical Prompting](#8-hierarchical-prompting)
9. [Multi-Step vs Hierarchical Prompting](#9-multi-step-vs-hierarchical-prompting)
10. [Prompt Decomposition](#10-prompt-decomposition)
11. [Prompt Decomposition vs Multi-Step Prompting](#11-prompt-decomposition-vs-multi-step-prompting)
12. [Customer Feedback Classification](#12-customer-feedback-classification)
13. [Customer Feedback Classification Example](#13-customer-feedback-classification-example)
14. [Financial Analyst Prompt](#14-financial-analyst-prompt)
15. [Year-over-Year Growth Calculation](#15-year-over-year-growth-calculation)
16. [YoY Growth Example for 2026 Revenue](#16-yoy-growth-example-for-2026-revenue)
17. [Code Generation for a Specific Task](#17-code-generation-for-a-specific-task)
18. [Advanced Prompt Example](#18-advanced-prompt-example)
19. [Combining Advanced Techniques](#19-combining-advanced-techniques)
20. [Prompt Engineering Workflow](#20-prompt-engineering-workflow)
21. [Advantages](#21-advantages)
22. [Limitations](#22-limitations)
23. [Common Mistakes](#23-common-mistakes)
24. [Important Comparisons](#24-important-comparisons)
25. [Important Terms](#25-important-terms)
26. [Case Study](#26-case-study)
27. [Important Exam Questions](#27-important-exam-questions)
28. [Important Diagrams](#28-important-diagrams)
29. [Quick Revision](#29-quick-revision)
30. [One-Minute Revision](#30-one-minute-revision)
31. [Most Important Exam Points](#31-most-important-exam-points)
32. [Final Chapter Summary](#32-final-chapter-summary)
33. [Final Memory Map](#33-final-memory-map)

---

# 1. Introduction

Basic Prompt Engineering focuses on creating clear and effective individual prompts.

However, complex real-world tasks often require more than one instruction.

For example:

> "Analyze customer feedback, classify the complaints, identify the most common issue, calculate its percentage, and recommend a solution."

This task contains multiple smaller tasks.

Advanced Prompt Engineering provides techniques for handling such complex tasks.

Important advanced techniques include:

- Prompt Chaining
- Strategic Role Playing
- ReAct
- Iterative Self-Refinement
- Multi-Step Prompting
- Hierarchical Prompting
- Prompt Decomposition
- Structured classification
- Financial analysis prompting
- Specialized code-generation prompts

---

# 2. What is Advanced Prompt Engineering?

## Definition

> **Advanced Prompt Engineering is the use of structured and sophisticated prompting techniques to solve complex, multi-stage, or specialized tasks using Generative AI.**

It goes beyond simply asking a question.

It involves:

- Breaking complex problems into smaller tasks
- Assigning suitable roles
- Controlling intermediate outputs
- Reviewing and refining results
- Connecting multiple prompts
- Organizing tasks hierarchically
- Using reasoning and action-oriented workflows

---

## Simple Difference

### Basic Prompt

> "Analyze this data."

### Advanced Prompt

> "Act as a financial analyst. First identify the revenue figures, then calculate the year-over-year growth, verify the calculation, identify the major trend, and finally present the result in a table."

The second prompt gives the AI a structured process.

---

# 3. Prompt Chaining

## Definition

**Prompt Chaining** is a technique where the output of one prompt is used as the input or context for another prompt.

Instead of asking the AI to complete a large task in one step, the task is divided into multiple connected prompts.

---

## Basic Structure

**Prompt 1**

↓

**Output 1**

↓

**Prompt 2**

↓

**Output 2**

↓

**Prompt 3**

↓

**Final Output**

---

## Example

Suppose we want to create a report about Artificial Intelligence.

### Prompt 1

> "List the major applications of Artificial Intelligence."

### Output 1

The AI generates a list of applications.

### Prompt 2

> "Using the applications identified above, explain their benefits."

### Output 2

The AI explains the benefits.

### Prompt 3

> "Using the previous information, create a final report with an introduction, applications, benefits, limitations, and conclusion."

---

## Why Use Prompt Chaining?

It is useful when:

- The task is complex
- Different stages require different instructions
- Intermediate results are useful
- The final task requires multiple operations

---

## Advantages

- Breaks complex tasks into manageable parts
- Makes each stage easier to control
- Improves organization
- Makes debugging easier
- Allows different prompts for different subtasks

---

# 4. Strategic Role Player

## Definition

A **Strategic Role Player** is a prompting technique where the AI is assigned a specialized professional role to approach a task from a particular perspective.

The role is selected according to the objective of the task.

---

## Examples

### Financial Task

> "Act as a financial analyst."

### Programming Task

> "Act as a senior software developer."

### Education Task

> "Act as an experienced professor."

### Marketing Task

> "Act as a digital marketing strategist."

---

## Example

### Prompt

> "Act as a financial analyst. Analyze the company's revenue data, calculate the year-over-year growth, identify important trends, and provide a short business interpretation."

---

## Why Use Strategic Roles?

A strategic role can help:

- Establish the desired perspective
- Set an appropriate level of expertise
- Make the response more task-specific
- Improve organization
- Focus the AI on the relevant objective

---

# 5. ReAct Prompting

## Definition

**ReAct** stands for:

> **Reason + Act**

ReAct is a prompting approach that combines reasoning with actions or tool interactions to solve a task.

The system can:

1. Analyze the problem
2. Decide what action is required
3. Perform the action
4. Observe the result
5. Continue until the task is completed

---

## Basic ReAct Cycle

**Problem**

↓

**Reason**

↓

**Action**

↓

**Observation**

↓

**Reason**

↓

**Action**

↓

**Final Answer**

---

## Simple Example

Suppose an AI needs to answer:

> "What is the current temperature in Mumbai?"

A tool-enabled AI may:

1. Determine that current weather information is needed.
2. Use a weather tool.
3. Observe the returned temperature.
4. Provide the answer.

---

## Another Example

For a research task:

> "Find the latest information about a technology, compare reliable sources, and summarize the findings."

The AI may:

- Determine what information is required
- Search for information
- Examine the results
- Compare information
- Produce the final answer

---

## Important Point

ReAct is especially useful when a task requires interaction with:

- Search tools
- Calculators
- Databases
- APIs
- External tools
- Other information sources

---

## Advantages

- Useful for multi-stage tasks
- Connects reasoning with actions
- Useful for tool-based AI systems
- Helps handle tasks requiring external information

---

# 6. Iterative Self-Refinement

## Definition

**Iterative Self-Refinement** is a technique where the AI generates an output, evaluates it, identifies weaknesses, improves it, and repeats the process.

The process continues until the result meets the required criteria.

---

## Basic Process

**Initial Prompt**

↓

**Generate Output**

↓

**Evaluate Output**

↓

**Find Problems**

↓

**Refine Output**

↓

**Evaluate Again**

↓

**Final Output**

---

## Example

### Initial Prompt

> "Write an introduction about Artificial Intelligence."

The AI generates an introduction.

Then the user can ask:

> "Review the introduction for clarity, grammar, accuracy, and relevance. Rewrite it to improve the weaknesses."

---

## More Advanced Prompt

> "Write the introduction. Then evaluate it for clarity, factual accuracy, organization, and relevance. Identify weaknesses and produce an improved final version."

---

## Advantages

- Improves quality
- Can reduce obvious errors
- Helps improve clarity
- Useful for writing and coding
- Useful for complex outputs

---

## Limitation

Self-refinement does **not guarantee correctness**.

The AI may fail to recognize some of its own mistakes.

Important facts and calculations should still be independently verified.

---

# 7. Multi-Step Prompting

## Definition

**Multi-Step Prompting** divides a task into several ordered steps.

Each step has a specific purpose.

---

## Example

Task:

> Analyze a company's revenue.

### Multi-Step Prompt

> 1. Identify the revenue for each year.
> 2. Calculate the year-over-year growth.
> 3. Identify the year with the highest growth.
> 4. Identify the year with the lowest growth.
> 5. Explain the overall trend.
> 6. Present the final results in a table.

---

## Advantages

- Makes the process clear
- Helps handle complex tasks
- Improves organization
- Makes requirements explicit

---

# 8. Hierarchical Prompting

## Definition

**Hierarchical Prompting** organizes a large task into levels.

A main objective is divided into major subtasks, and those subtasks can be further divided into smaller tasks.

---

## Structure

**Main Goal**

↓

**Major Task 1**

→ Subtask 1.1  
→ Subtask 1.2

↓

**Major Task 2**

→ Subtask 2.1  
→ Subtask 2.2

↓

**Final Result**

---

## Example

### Main Goal

> Create a business analysis report.

### Level 1

1. Collect information
2. Analyze financial data
3. Analyze customers
4. Identify risks
5. Provide recommendations

### Level 2

Under financial analysis:

- Identify revenue
- Calculate growth
- Compare years
- Identify trends

---

## Why Hierarchical Prompting?

It is useful when:

- The task is very large
- There are multiple related subtasks
- Tasks have dependencies
- The final result needs a clear structure

---

# 9. Multi-Step vs Hierarchical Prompting

| Multi-Step Prompting | Hierarchical Prompting |
|---|---|
| Divides a task into ordered steps | Divides a task into levels |
| Usually follows a sequence | Can contain multiple branches |
| Step 1 → Step 2 → Step 3 | Main Task → Subtasks → Sub-subtasks |
| Good for sequential tasks | Good for complex large tasks |
| Focuses on process | Focuses on structure and organization |

---

## Memory Trick

> **Multi-Step = Sequence**

> **Hierarchical = Levels**

---

# 10. Prompt Decomposition

## Definition

**Prompt Decomposition** is the process of breaking a complex prompt or problem into smaller, simpler prompts or subtasks.

Instead of asking the AI to solve everything at once, each part is handled separately.

---

## Example

### Complex Task

> "Analyze customer feedback and recommend product improvements."

This can be decomposed into:

### Prompt 1

> "Extract the main customer complaints."

### Prompt 2

> "Classify each complaint into Pricing, Support, or Features."

### Prompt 3

> "Calculate the percentage of complaints in each category."

### Prompt 4

> "Identify the category with the highest number of complaints."

### Prompt 5

> "Recommend improvements based on the results."

---

## Benefits

- Reduces complexity
- Makes each task easier
- Improves control
- Makes errors easier to locate
- Produces organized results

---

# 11. Prompt Decomposition vs Multi-Step Prompting

| Prompt Decomposition | Multi-Step Prompting |
|---|---|
| Breaks a complex task into smaller subtasks/prompts | Specifies an ordered sequence of steps |
| Focuses on dividing the problem | Focuses on the execution sequence |
| Subtasks may be handled separately | Steps are generally connected in sequence |
| Useful for very complex tasks | Useful for structured processes |

---

## Simple Memory

> **Decomposition = Divide**

> **Multi-Step = Sequence**

---

# 12. Customer Feedback Classification

Customer feedback can be classified into predefined categories.

For this chapter, the categories are:

1. **Pricing**
2. **Support**
3. **Features**

---

## Category 1 — Pricing

Feedback related to:

- Cost
- Price
- Subscription
- Discounts
- Payment
- Expensive products
- Affordability

### Example

> "The monthly subscription is too expensive."

**Category → Pricing**

---

## Category 2 — Support

Feedback related to:

- Customer service
- Technical support
- Response time
- Help desk
- Complaint resolution

### Example

> "The support team took three days to respond."

**Category → Support**

---

## Category 3 — Features

Feedback related to:

- Missing functionality
- Product features
- New features
- Feature requests
- Product capabilities

### Example

> "The application should have a dark mode."

**Category → Features**

---

# 13. Customer Feedback Classification Example

## Task

Classify customer feedback into:

- Pricing
- Support
- Features

---

## Feedback

> "The software is useful, but the subscription price is too high."

### Classification

**Pricing**

---

## Feedback

> "The customer service team solved my issue very quickly."

### Classification

**Support**

---

## Feedback

> "The application needs an offline mode."

### Classification

**Features**

---

## Prompt

> "Classify each customer feedback statement into exactly one of the following categories: Pricing, Support, or Features. Do not create new categories. Provide the feedback statement and its category in a table."

---

## Output Format

| Customer Feedback | Category |
|---|---|
| The subscription is too expensive. | Pricing |
| Support took too long to respond. | Support |
| The app needs dark mode. | Features |

---

# 13.1 Customer Feedback Classification Workflow

**Customer Feedback**

↓

**Understand Feedback**

↓

**Identify Main Issue**

↓

**Compare With Categories**

↓

**Assign One Category**

↓

**Present Result**

---

# 13.2 Prompt Decomposition for Customer Feedback

Instead of using one large prompt:

> "Analyze all customer feedback."

Use several smaller prompts.

### Step 1

> "Extract all customer feedback statements."

### Step 2

> "Classify each statement into Pricing, Support, or Features."

### Step 3

> "Count the number of feedback items in each category."

### Step 4

> "Calculate the percentage for each category."

### Step 5

> "Identify the category receiving the most negative feedback."

### Step 6

> "Suggest improvements based on the results."

---

# 14. Financial Analyst Prompt

## Role

A financial analyst examines financial information and identifies useful trends.

Prompt Engineering can assign this role to AI.

---

## Example Prompt

> "Act as a financial analyst. Analyze the company's revenue data for 2024, 2025, and 2026. Calculate the year-over-year growth for 2025 and 2026, identify the growth trend, and present the results in a table. Clearly show the formula used."

---

## Components

| Component | Example |
|---|---|
| Role | Financial Analyst |
| Task | Analyze revenue |
| Data | 2024, 2025, 2026 revenue |
| Calculation | YoY Growth |
| Analysis | Identify trend |
| Output | Table |

---

# 15. Year-over-Year Growth Calculation

## What is YoY Growth?

**YoY** stands for:

> **Year-over-Year**

YoY growth compares a value from one year with the value from the previous year.

It is commonly used to measure growth or decline in:

- Revenue
- Sales
- Profit
- Users
- Expenses
- Production

---

# 15.1 YoY Growth Formula

$$
\text{YoY Growth (\%)} =
\frac{\text{Current Year Value} - \text{Previous Year Value}}
{\text{Previous Year Value}}
\times 100
$$

---

## Alternative Form

$$
\text{YoY Growth (\%)} =
\left(
\frac{\text{Current Year Value}}
{\text{Previous Year Value}}
-1
\right)
\times 100
$$

Both formulas give the same result.

---

# 15.2 Interpreting YoY Growth

### Positive YoY

If the result is positive:

> The value increased compared with the previous year.

### Negative YoY

If the result is negative:

> The value decreased compared with the previous year.

### Zero YoY

If the result is zero:

> The value remained unchanged.

---

# 16. YoY Growth Example for 2026 Revenue

Suppose:

- 2025 Revenue = ₹80 lakh
- 2026 Revenue = ₹100 lakh

We need to calculate the YoY growth for 2026.

---

## Step 1 — Identify Current Year

2026 Revenue:

**₹100 lakh**

---

## Step 2 — Identify Previous Year

2025 Revenue:

**₹80 lakh**

---

## Step 3 — Apply Formula

$$
\text{YoY Growth}
=
\frac{100-80}{80}
\times100
$$

$$
=
\frac{20}{80}
\times100
$$

$$
=25\%
$$

---

## Final Answer

> **The company's revenue grew by 25% in 2026 compared with 2025.**

---

# 16.1 Example With Revenue Table

Suppose the company has:

| Year | Revenue |
|---|---:|
| 2024 | ₹60 lakh |
| 2025 | ₹80 lakh |
| 2026 | ₹100 lakh |

---

## YoY Growth for 2025

$$
\frac{80-60}{60}\times100
=
33.33\%
$$

---

## YoY Growth for 2026

$$
\frac{100-80}{80}\times100
=
25\%
$$

---

## Interpretation

The company continued to grow, but the growth rate decreased from **33.33% in 2025** to **25% in 2026**.

This means:

> Revenue increased, but the rate of growth slowed.

---

# 16.2 Prompt for YoY Calculation

> "Act as a financial analyst. Given the following revenue data, calculate the year-over-year growth for 2026. Use the formula: ((2026 Revenue - 2025 Revenue) / 2025 Revenue) × 100. Show the calculation step by step and provide the final percentage. Then briefly interpret whether revenue increased or decreased."

---

# 17. Code Generation for a Specific Task

Generative AI can also be used to generate programming code.

However, a good coding prompt should clearly specify:

- Programming language
- Task
- Input
- Expected output
- Constraints
- Level of complexity
- Explanation requirements

---

## Poor Prompt

> "Write a program."

This is too vague.

---

## Better Prompt

> "Write a C program to check whether a number is even or odd."

---

## Advanced Prompt

> "Act as a C programming tutor. Write a beginner-friendly C program that accepts an integer from the user and checks whether it is even or odd. Explain the logic before the code, provide the complete code, explain each important line, and show one sample input and output. Do not use advanced concepts."

---

# 17.1 Code Generation Prompt Structure

A strong coding prompt can contain:

### 1. Role

> "Act as a C programming tutor."

### 2. Language

> "Use C."

### 3. Task

> "Check whether a number is prime."

### 4. Input

> "Accept an integer from the user."

### 5. Output

> "Print whether the number is prime or not."

### 6. Constraints

> "Keep the program beginner-friendly."

### 7. Explanation

> "Explain the logic and code."

---

# 17.2 Example — Prime Number Program

### Prompt

> "Act as a beginner-level C programming tutor. Write a C program that accepts an integer and checks whether it is prime. First explain the logic, then provide the code, then explain the important lines, and finally provide sample input and output. Use only basic C concepts such as loops, if-else, and variables."

---

## Why This Prompt is Better

It specifies:

- Role
- Programming language
- Task
- Input
- Concepts
- Difficulty level
- Output
- Explanation

---

# 18. Advanced Prompt Example

A complex prompt can combine several advanced techniques.

## Example

> "Act as a senior business analyst. Analyze the company's revenue and customer feedback. First extract the relevant data. Then classify customer feedback into Pricing, Support, and Features. Next calculate the YoY revenue growth for 2026 using the previous year's revenue. Review the calculations for possible errors. Finally, provide a concise business summary in a structured table."

---

## Techniques Used

| Technique | Use |
|---|---|
| Strategic Role | Business analyst |
| Prompt Decomposition | Separate analysis tasks |
| Multi-Step | Perform tasks in sequence |
| Self-Refinement | Review calculations |
| Output Control | Structured table |
| Classification | Categorize feedback |

---

# 19. Combining Advanced Techniques

Advanced Prompt Engineering becomes more powerful when multiple techniques are combined.

---

## Example

Suppose we want to analyze customer feedback and revenue.

### Step 1 — Role

> "Act as a financial and business analyst."

### Step 2 — Decompose

Break the task into:

- Revenue analysis
- Customer feedback classification
- Growth calculation
- Recommendation

### Step 3 — Multi-Step

1. Extract data.
2. Classify feedback.
3. Calculate YoY growth.
4. Identify trends.
5. Generate recommendations.

### Step 4 — Self-Refinement

> "Review the calculations and classifications for errors."

### Step 5 — Output Control

> "Present the results in tables followed by a short summary."

---

# 20. Prompt Engineering Workflow

A complex AI task can follow this workflow:

**Understand Objective**

↓

**Identify Required Information**

↓

**Assign Suitable Role**

↓

**Decompose Task**

↓

**Create Multi-Step Process**

↓

**Generate Output**

↓

**Review / Refine**

↓

**Control Final Format**

↓

**Final Result**

---

# 21. Advantages

## 21.1 Handles Complex Tasks

Large problems can be divided into manageable parts.

---

## 21.2 Better Organization

Tasks and outputs can be clearly structured.

---

## 21.3 Improved Control

The user can control:

- Role
- Process
- Output
- Format
- Requirements

---

## 21.4 Better Error Detection

Review and refinement stages can help identify possible problems.

---

## 21.5 Useful for Professional Tasks

Advanced prompting can be used for:

- Financial analysis
- Programming
- Research
- Customer feedback analysis
- Business planning
- Education
- Data analysis
- Software development

---

## 21.6 Reusable

A well-designed prompt can be reused for similar tasks.

---

# 22. Limitations

## 22.1 No Guarantee of Accuracy

Even advanced prompts can produce incorrect answers.

---

## 22.2 Complexity

Very complicated prompts can become difficult to manage.

---

## 22.3 Model Dependency

Different AI models may interpret the same prompt differently.

---

## 22.4 Incorrect Assumptions

AI may make assumptions when information is missing.

---

## 22.5 Self-Checking Is Not Perfect

An AI may fail to detect its own mistakes.

---

## 22.6 External Data May Be Required

Some tasks require current or external information that the model may not have.

---

# 23. Common Mistakes

## Mistake 1 — Giving a Very Broad Task

Poor:

> "Analyze the company."

Better:

> "Analyze the company's revenue from 2024 to 2026 and calculate the YoY growth."

---

## Mistake 2 — Not Providing Categories

Poor:

> "Classify customer feedback."

Better:

> "Classify feedback into exactly three categories: Pricing, Support, and Features."

---

## Mistake 3 — Not Specifying the Formula

Poor:

> "Calculate growth."

Better:

> "Calculate YoY growth using ((Current Year - Previous Year) / Previous Year) × 100."

---

## Mistake 4 — Not Specifying Programming Language

Poor:

> "Write a program to check prime numbers."

Better:

> "Write a beginner-friendly C program to check whether an integer is prime."

---

## Mistake 5 — Combining Too Many Tasks Without Structure

Poor:

> "Analyze feedback, revenue, customers, competitors, make recommendations, create a report, and write code."

Better:

Break the task into clear stages.

---

## Mistake 6 — Not Reviewing the Result

Always evaluate important AI-generated outputs.

---

# 24. Important Comparisons

## 24.1 Basic vs Advanced Prompt Engineering

| Basic Prompt Engineering | Advanced Prompt Engineering |
|---|---|
| Usually handles simpler tasks | Handles complex tasks |
| Often uses individual prompts | Can use multiple connected prompts |
| Basic role/task instructions | Uses advanced workflows |
| Less structured | Highly structured |
| Simple output control | Multi-stage output control |

---

# 24.2 Prompt Chaining vs Prompt Decomposition

| Prompt Chaining | Prompt Decomposition |
|---|---|
| Connects multiple prompts | Breaks a complex task into smaller tasks |
| Output of one prompt can become input for another | Focuses on dividing the original problem |
| Emphasis on connection | Emphasis on division |

---

# 24.3 ReAct vs Self-Refinement

| ReAct | Self-Refinement |
|---|---|
| Reason + Act | Generate + Review + Improve |
| Often involves actions/tools | Focuses on improving generated output |
| Useful for tool-based tasks | Useful for quality improvement |
| Can interact with external tools | Can review its own response |

---

# 24.4 Multi-Step vs Hierarchical

| Multi-Step | Hierarchical |
|---|---|
| Sequential | Multi-level |
| Step 1 → Step 2 → Step 3 | Main task → subtasks → sub-subtasks |
| Focuses on order | Focuses on organization |

---

# 24.5 Role-Based vs Strategic Role Player

| Role-Based | Strategic Role Player |
|---|---|
| Assigns a role | Assigns a role specifically suited to the strategic objective |
| "Act as a teacher" | "Act as an academic advisor and design an exam preparation strategy" |
| General role | More task-oriented and goal-focused |

---

# 25. Important Terms

| Term | Meaning |
|---|---|
| **Advanced Prompt Engineering** | Sophisticated techniques for solving complex AI tasks |
| **Prompt Chaining** | Connecting multiple prompts together |
| **Strategic Role Player** | Assigning AI a specialized role for a specific objective |
| **ReAct** | Reason + Act |
| **Iterative Self-Refinement** | Repeatedly reviewing and improving output |
| **Multi-Step Prompting** | Dividing a task into ordered steps |
| **Hierarchical Prompting** | Organizing tasks into multiple levels |
| **Prompt Decomposition** | Breaking a complex task into smaller subtasks |
| **Classification** | Assigning data to predefined categories |
| **Pricing** | Feedback related to cost or price |
| **Support** | Feedback related to customer service/help |
| **Features** | Feedback related to product functionality |
| **Financial Analyst** | Person who analyzes financial information |
| **YoY** | Year-over-Year |
| **YoY Growth** | Percentage change compared with previous year |
| **Code Generation** | Using AI to create programming code |
| **Refinement** | Improving an existing output |

---

# 26. Case Study

# Case Study — Customer Feedback + Revenue Analysis

## Problem

A company has collected customer feedback and annual revenue data.

Customer feedback needs to be classified into:

- Pricing
- Support
- Features

The company also wants to calculate the YoY revenue growth for 2026.

---

## Customer Feedback

1. "The subscription is too expensive."
2. "Customer support takes too long to respond."
3. "The application should provide dark mode."
4. "The price is affordable."
5. "I want an offline mode."

---

## Classification

| Feedback | Category |
|---|---|
| The subscription is too expensive. | Pricing |
| Customer support takes too long to respond. | Support |
| The application should provide dark mode. | Features |
| The price is affordable. | Pricing |
| I want an offline mode. | Features |

---

## Category Count

| Category | Count |
|---|---:|
| Pricing | 2 |
| Support | 1 |
| Features | 2 |

---

## Revenue Data

| Year | Revenue |
|---|---:|
| 2025 | ₹80 lakh |
| 2026 | ₹100 lakh |

---

## YoY Calculation

$$
\text{YoY Growth}
=
\frac{100-80}{80}
\times100
$$

$$
=25\%
$$

---

## Final Analysis

- Pricing feedback → 2
- Support feedback → 1
- Features feedback → 2
- 2026 YoY revenue growth → **25%**
- Pricing and Features have the highest number of feedback items in this example.

---

## Suitable Advanced Prompt

> "Act as a business analyst. Analyze the customer feedback and revenue data. First classify every feedback statement into exactly one of these categories: Pricing, Support, or Features. Then count the feedback in each category. Next calculate the 2026 YoY revenue growth using 2025 as the previous year. Review the classification and calculation for possible errors. Finally, present the findings in tables followed by a concise business summary."

---

# 27. Important Exam Questions

## Very Short Answer Questions

1. Define Advanced Prompt Engineering.
2. What is Prompt Chaining?
3. What is a Strategic Role Player?
4. What does ReAct stand for?
5. What is Iterative Self-Refinement?
6. What is Multi-Step Prompting?
7. What is Hierarchical Prompting?
8. What is Prompt Decomposition?
9. What is customer feedback classification?
10. What are the three customer feedback categories used in this chapter?
11. What does YoY stand for?
12. Write the YoY growth formula.
13. What is Code Generation?
14. Mention two advantages of advanced prompting.
15. Mention two limitations of advanced prompting.

---

# 27.1 Short Answer Questions

1. Explain Prompt Chaining with an example.
2. Explain Strategic Role Playing.
3. Explain ReAct prompting.
4. Explain Iterative Self-Refinement.
5. Explain Multi-Step Prompting.
6. Explain Hierarchical Prompting.
7. Explain Prompt Decomposition.
8. Differentiate Multi-Step and Hierarchical Prompting.
9. Explain customer feedback classification.
10. Explain the categories Pricing, Support, and Features.
11. Explain YoY growth with a formula.
12. Explain how AI can be used as a financial analyst.
13. Explain how Prompt Engineering can be used for code generation.
14. Explain the advantages of Advanced Prompt Engineering.
15. Explain the limitations of Advanced Prompt Engineering.

---

# 27.2 Long Answer / 5-Mark Questions

1. Explain different Advanced Prompt Engineering techniques with suitable examples.

2. Explain Prompt Chaining and Prompt Decomposition in detail.

3. Explain ReAct prompting and Iterative Self-Refinement.

4. Explain Multi-Step and Hierarchical Prompting with examples.

5. Explain the role of Strategic Role Playing in Prompt Engineering.

6. Explain how AI can classify customer feedback into Pricing, Support, and Features.

7. Explain how to create a prompt for a financial analyst to calculate YoY growth.

8. Calculate the YoY growth for 2026 revenue using suitable data and explain the result.

9. Explain how Prompt Engineering can be used for code generation.

10. Design an advanced prompt for analyzing customer feedback and financial data.

11. Discuss the advantages and limitations of Advanced Prompt Engineering.

12. Explain how multiple advanced Prompt Engineering techniques can be combined to solve a complex task.

---

# 27.3 Practical Questions

## Question 1

Create a prompt that classifies customer feedback into:

- Pricing
- Support
- Features

### Answer

> "Classify each customer feedback statement into exactly one of the following categories: Pricing, Support, or Features. Do not create additional categories. Present the result in a table with columns for Feedback and Category."

---

## Question 2

Create a prompt to calculate 2026 YoY revenue growth.

### Answer

> "Act as a financial analyst. Given the company's 2025 and 2026 revenue, calculate the 2026 year-over-year growth using the formula ((2026 Revenue - 2025 Revenue) / 2025 Revenue) × 100. Show the calculation step by step and interpret the result."

---

## Question 3

Create a prompt for code generation.

### Answer

> "Act as a C programming tutor. Write a beginner-friendly C program to check whether a number is prime. Explain the logic first, then provide the code, followed by sample input and output."

---

# 28. Important Diagrams

## Diagram 1 — Prompt Chaining

**Prompt 1**

↓

**Output 1**

↓

**Prompt 2**

↓

**Output 2**

↓

**Prompt 3**

↓

**Final Output**

---

# Diagram 2 — ReAct

**Problem**

↓

**Reason**

↓

**Act**

↓

**Observe**

↓

**Reason**

↓

**Act**

↓

**Final Answer**

---

# Diagram 3 — Self-Refinement

**Initial Output**

↓

**Evaluate**

↓

**Identify Problems**

↓

**Refine**

↓

**Evaluate Again**

↓

**Improved Output**

---

# Diagram 4 — Prompt Decomposition

**Complex Problem**

↓

**Subtask 1**

**Subtask 2**

**Subtask 3**

**Subtask 4**

↓

**Combine Results**

↓

**Final Answer**

---

# Diagram 5 — Hierarchical Prompting

**Main Objective**

↓

├── **Major Task 1**

│   ├── Subtask 1.1

│   └── Subtask 1.2

↓

├── **Major Task 2**

│   ├── Subtask 2.1

│   └── Subtask 2.2

↓

└── **Major Task 3**

    ├── Subtask 3.1

    └── Subtask 3.2

↓

**Final Result**

---

# Diagram 6 — Advanced Prompt Engineering Workflow

**Understand Goal**

↓

**Assign Role**

↓

**Decompose Task**

↓

**Create Steps**

↓

**Generate Output**

↓

**Review**

↓

**Refine**

↓

**Format**

↓

**Final Output**

---

# Diagram 7 — YoY Growth

**Previous Year Revenue**

↓

**Current Year Revenue**

↓

**Subtract Previous from Current**

↓

**Divide by Previous Year**

↓

**Multiply by 100**

↓

**YoY Growth %**

---

# 29. Quick Revision

## Prompt Chaining

> Output of one prompt is used for another prompt.

---

## Strategic Role Player

> Assign AI a specialized role according to the task.

---

## ReAct

> **Reason + Act**

---

## Iterative Self-Refinement

> Generate → Review → Improve → Repeat.

---

## Multi-Step Prompting

> Complete a task through ordered steps.

---

## Hierarchical Prompting

> Organize a large task into levels.

---

## Prompt Decomposition

> Break a complex task into smaller subtasks.

---

## Customer Feedback Categories

> **Pricing + Support + Features**

---

## YoY

> **Year-over-Year**

---

## YoY Formula

$$
\frac{\text{Current Year} - \text{Previous Year}}
{\text{Previous Year}}
\times100
$$

---

## Code Generation

> Use AI to generate programming code based on clearly defined requirements.

---

# 30. One-Minute Revision

## Remember:

### C

**Prompt Chaining**

→ Connect prompts

### R

**ReAct**

→ Reason + Act

### S

**Self-Refinement**

→ Review + Improve

### M

**Multi-Step**

→ Sequence

### H

**Hierarchical**

→ Levels

### D

**Decomposition**

→ Divide

### R

**Role Player**

→ Specialized role

### Y

**YoY**

→ Current vs previous year

---

# 31. Most Important Exam Points

> ⭐ Advanced Prompt Engineering is used for complex and specialized AI tasks.

> ⭐ Prompt Chaining connects multiple prompts where the output of one stage can support the next stage.

> ⭐ Strategic Role Playing assigns AI a specialized role suited to the objective.

> ⭐ ReAct stands for **Reason + Act**.

> ⭐ ReAct is particularly useful for tasks involving actions, tools, or external information.

> ⭐ Iterative Self-Refinement follows a generate → evaluate → improve cycle.

> ⭐ Multi-Step Prompting divides a task into ordered steps.

> ⭐ Hierarchical Prompting organizes a task into multiple levels.

> ⭐ Prompt Decomposition breaks a complex problem into smaller subtasks.

> ⭐ Customer feedback can be classified into predefined categories such as **Pricing, Support, and Features**.

> ⭐ Pricing feedback concerns cost, price, subscriptions, or affordability.

> ⭐ Support feedback concerns customer service and assistance.

> ⭐ Features feedback concerns product functionality or feature requests.

> ⭐ YoY means **Year-over-Year**.

> ⭐ YoY growth measures the percentage change between the current year and previous year.

> ⭐ YoY Growth Formula = ((Current Year − Previous Year) / Previous Year) × 100.

> ⭐ Code-generation prompts should specify programming language, task, inputs, outputs, and constraints.

> ⭐ Advanced techniques can be combined to solve complex real-world problems.

> ⭐ Advanced prompting does not guarantee that the AI's output is correct.

---

# 32. Final Chapter Summary

Advanced Prompt Engineering extends basic prompting techniques to handle complex, multi-stage, and specialized tasks.

The major techniques are:

### 1. Prompt Chaining

Connects multiple prompts together.

### 2. Strategic Role Player

Assigns AI a specialized professional role.

### 3. ReAct

Combines reasoning with actions.

### 4. Iterative Self-Refinement

Allows output to be reviewed and improved repeatedly.

### 5. Multi-Step Prompting

Breaks a task into ordered steps.

### 6. Hierarchical Prompting

Organizes complex tasks into multiple levels.

### 7. Prompt Decomposition

Breaks a large problem into smaller subtasks.

These techniques can be applied to practical problems such as:

- Customer feedback classification
- Financial analysis
- YoY growth calculation
- Code generation
- Business analysis
- Data analysis
- Research
- Software development

---

# 33. Final Memory Map

## ADVANCED PROMPT ENGINEERING

### Step 1 — Understand the Problem

↓

### Step 2 — Assign a Strategic Role

↓

### Step 3 — Decompose the Problem

↓

### Step 4 — Create Multiple Steps

↓

### Step 5 — Use Prompt Chaining if Required

↓

### Step 6 — Use ReAct for Reason + Action Tasks

↓

### Step 7 — Generate Output

↓

### Step 8 — Self-Review

↓

### Step 9 — Refine

↓

### Step 10 — Control Final Format

↓

### FINAL RESULT

---

# MASTER MEMORY TABLE

| Concept | Quick Memory |
|---|---|
| Advanced Prompt Engineering | Handle complex AI tasks |
| Prompt Chaining | Connect prompts |
| Strategic Role Player | Give AI a specialized role |
| ReAct | Reason + Act |
| Self-Refinement | Review + Improve |
| Multi-Step | Ordered sequence |
| Hierarchical | Multiple levels |
| Decomposition | Divide complex problem |
| Classification | Assign predefined categories |
| Pricing | Cost-related feedback |
| Support | Customer-service feedback |
| Features | Functionality-related feedback |
| Financial Analyst | Analyze financial information |
| YoY | Year-over-Year |
| YoY Growth | Percentage change from previous year |
| Code Generation | AI-generated programming code |
| Iteration | Repeated improvement |

---

# FINAL EXAM FORMULA

## If asked: "Explain Advanced Prompt Engineering Techniques"

Write:

**Introduction**

↓

**Definition**

↓

**Prompt Chaining**

↓

**Strategic Role Player**

↓

**ReAct**

↓

**Iterative Self-Refinement**

↓

**Multi-Step Prompting**

↓

**Hierarchical Prompting**

↓

**Prompt Decomposition**

↓

**Examples**

↓

**Applications**

↓

**Advantages**

↓

**Limitations**

↓

**Conclusion**

---

# ULTIMATE MEMORY TRICK

## "CHAIN → ROLE → REACT → REFINE → STEP → HIERARCHY → DECOMPOSE"

### CHAIN
**Prompt Chaining**

→ Connect multiple prompts

### ROLE
**Strategic Role Player**

→ Assign specialized expertise

### REACT
**Reason + Act**

→ Think/decide + perform action

### REFINE
**Iterative Self-Refinement**

→ Review and improve

### STEP
**Multi-Step Prompting**

→ Follow ordered steps

### HIERARCHY
**Hierarchical Prompting**

→ Organize into levels

### DECOMPOSE
**Prompt Decomposition**

→ Break complex tasks into smaller tasks

---

# PRACTICAL MEMORY

## Customer Feedback

**Pricing**

→ Cost / Price

**Support**

→ Customer Service

**Features**

→ Functionality

---

## Financial Analysis

**2025 Revenue**

↓

**2026 Revenue**

↓

**YoY Formula**

↓

**Growth %**

↓

**Business Interpretation**

---

## Code Generation

**Language**

↓

**Task**

↓

**Input**

↓

**Output**

↓

**Constraints**

↓

**Code**

↓

**Explanation**

---

# FINAL CHAPTER TAKEAWAY

> **Advanced Prompt Engineering is the systematic use of sophisticated prompting techniques to solve complex tasks by assigning appropriate roles, decomposing problems, organizing multiple steps, connecting prompts, using reasoning and actions, reviewing outputs, and refining results.**

> **The main goal is: Complex Problem → Structured Prompting → Controlled Process → Improved AI Output.**

---

# End of Chapter 4

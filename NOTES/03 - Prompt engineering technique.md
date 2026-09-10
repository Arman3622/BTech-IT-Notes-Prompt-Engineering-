# Chapter 3 — Prompt Engineering Techniques

> **Subject:** Generative AI / Prompt Engineering  
> **Chapter:** Prompt Engineering Techniques  
> **Purpose:** Long-term revision + upcoming examinations + practical AI usage

---

# Table of Contents

1. [Introduction](#1-introduction)
2. [What is Prompt Engineering?](#2-what-is-prompt-engineering)
3. [Components of Effective Prompting](#3-components-of-effective-prompting)
4. [Zero-Shot Prompting](#4-zero-shot-prompting)
5. [One-Shot Prompting](#5-one-shot-prompting)
6. [Few-Shot Prompting](#6-few-shot-prompting)
7. [Step-by-Step Prompting](#7-step-by-step-prompting)
8. [Self-Reflection Prompting](#8-self-reflection-prompting)
9. [Role-Based Prompting](#9-role-based-prompting)
10. [Persona Prompting](#10-persona-prompting)
11. [Role-Based vs Persona Prompting](#11-role-based-vs-persona-prompting)
12. [Output Control](#12-output-control)
13. [Output Format](#13-output-format)
14. [JSON Output](#14-json-output)
15. [Table Output](#15-table-output)
16. [Bullet Point Output](#16-bullet-point-output)
17. [Structured Output](#17-structured-output)
18. [Prompt Optimization](#18-prompt-optimization)
19. [Prompt Testing and Evaluation](#19-prompt-testing-and-evaluation)
20. [Prompt Iteration](#20-prompt-iteration)
21. [Combining Prompt Engineering Techniques](#21-combining-prompt-engineering-techniques)
22. [Prompt for a Travel Planner](#22-prompt-for-a-travel-planner)
23. [Prompt for Architecture](#23-prompt-for-architecture)
24. [Prompt for Study Notes](#24-prompt-for-study-notes)
25. [Prompt for Code Generation](#25-prompt-for-code-generation)
26. [Prompt for Mathematics](#26-prompt-for-mathematics)
27. [Prompt for Summarization](#27-prompt-for-summarization)
28. [Common Mistakes](#28-common-mistakes)
29. [Good Prompt vs Poor Prompt](#29-good-prompt-vs-poor-prompt)
30. [Advantages of Prompt Engineering](#30-advantages-of-prompt-engineering)
31. [Limitations of Prompt Engineering](#31-limitations-of-prompt-engineering)
32. [Case Study](#32-case-study)
33. [Important Comparisons](#33-important-comparisons)
34. [Important Terms](#34-important-terms)
35. [Important Exam Questions](#35-important-exam-questions)
36. [Important Diagrams](#36-important-diagrams)
37. [Quick Revision](#37-quick-revision)
38. [One-Minute Revision](#38-one-minute-revision)
39. [Most Important Exam Points](#39-most-important-exam-points)
40. [Final Chapter Summary](#40-final-chapter-summary)
41. [Final Memory Map](#41-final-memory-map)

---

# 1. Introduction

Prompt Engineering is the process of designing effective instructions for Generative AI systems.

A simple prompt may produce a useful answer, but carefully designed prompts can provide:

- More relevant results
- Better organization
- Better control over the response
- More consistent outputs
- Appropriate level of explanation
- Specific formats
- Better results for complex tasks

Prompt Engineering uses different techniques to communicate the desired result effectively.

Some important techniques are:

- Zero-shot prompting
- One-shot prompting
- Few-shot prompting
- Step-by-step prompting
- Self-reflection
- Role-based prompting
- Persona prompting
- Output control
- Prompt optimization

---

# 2. What is Prompt Engineering?

## Definition

> **Prompt Engineering is the process of designing, testing, refining, and optimizing prompts to obtain effective and useful outputs from an AI model.**

In simple words:

> **Prompt Engineering = Designing better instructions to get better results from AI.**

---

## Example

### Simple Prompt

"Explain Python."

### Engineered Prompt

"Act as a programming teacher. Explain Python to a beginner. Cover its definition, features, applications, advantages, and one simple example. Use simple English and present the answer using headings and bullet points."

The second prompt provides much more control.

---

# 3. Components of Effective Prompting

An effective prompt can contain several components.

## 3.1 Role

Defines the role or expertise the AI should use.

Example:

> "Act as a programming professor."

---

## 3.2 Task

Clearly states what the AI needs to do.

Example:

> "Explain recursion in C."

---

## 3.3 Context

Provides relevant background information.

Example:

> "The learner is a first-year B.Tech IT student."

---

## 3.4 Constraints

Defines limitations or rules.

Example:

> "Use simple English and keep the explanation under 500 words."

---

## 3.5 Examples

Provides examples of the desired pattern.

Example:

> "Use the following example as a format for the remaining questions."

---

## 3.6 Output Format

Specifies how the result should be presented.

Example:

> "Present the answer as a comparison table."

---

## 3.7 Audience

Defines who will read or use the output.

Example:

> "Explain it for a beginner."

---

## 3.8 Tone

Defines the communication style.

Examples:

- Formal
- Professional
- Friendly
- Academic
- Simple
- Technical

---

## Effective Prompt Structure

**Role**

↓

**Task**

↓

**Context**

↓

**Constraints**

↓

**Examples**

↓

**Output Format**

↓

**AI Response**

---

# 4. Zero-Shot Prompting

## Definition

**Zero-shot prompting** is a prompting technique where the AI is asked to perform a task without being given any examples.

### Memory Trick

> **Zero-shot = Zero examples**

---

## Example

Prompt:

> "Classify the following sentence as Positive or Negative: 'I really enjoyed the movie.'"

No example is provided.

The AI directly performs the task.

---

## Advantages

- Simple
- Fast
- Requires less prompt length
- Useful for common tasks

---

## Limitations

- May not always understand the exact desired pattern
- Can produce inconsistent formatting
- Less suitable for unusual or highly specific tasks

---

# 5. One-Shot Prompting

## Definition

**One-shot prompting** provides exactly one example to demonstrate how the AI should perform the task.

### Memory Trick

> **One-shot = One example**

---

## Example

Prompt:

> Classify the sentiment.
>
> Example:
> "I love this phone." → Positive
>
> Now classify:
> "This laptop is excellent."

The AI uses the provided example as guidance.

---

## Advantages

- Gives the AI a clear pattern
- Useful when the expected format is important
- Can improve consistency

---

# 6. Few-Shot Prompting

## Definition

**Few-shot prompting** provides multiple examples before asking the AI to perform the task.

### Memory Trick

> **Few-shot = Multiple examples**

---

## Example

Prompt:

> Classify the sentiment.
>
> "I love this phone." → Positive
>
> "This product is terrible." → Negative
>
> "The service was excellent." → Positive
>
> Now classify:
> "The experience was disappointing."

Multiple examples demonstrate the desired pattern.

---

## Advantages

- Provides stronger guidance
- Useful for classification
- Useful for specialized formats
- Can improve consistency

---

# 7. Step-by-Step Prompting

## Definition

Step-by-step prompting divides a complex task into smaller, ordered steps.

Instead of asking the AI to complete a complicated task at once, the prompt specifies the stages.

---

## Example

### General Prompt

> "Create a study plan."

### Step-by-Step Prompt

> 1. Identify the subjects.
> 2. Divide them according to difficulty.
> 3. Allocate study time.
> 4. Add revision sessions.
> 5. Add practice tests.
> 6. Present the final plan in a table.

---

## Advantages

- Makes complex tasks easier to understand
- Improves organization
- Makes requirements explicit
- Provides better control over the process

---

## Memory

> **Complex task → Break into steps → Complete systematically**

---

# 8. Self-Reflection Prompting

## Definition

**Self-reflection prompting** asks the AI to review or evaluate its own generated response against specified criteria before producing or finalizing the answer.

The goal is to encourage the model to identify possible errors, missing information, or weaknesses.

---

## Example

> "Solve the problem. Then check your answer for calculation errors and missing steps before presenting the final answer."

---

## Another Example

> "Write the explanation, then review it for clarity, factual consistency, and whether all requested points have been covered."

---

## Basic Process

**Generate Answer**

↓

**Review Answer**

↓

**Identify Possible Problems**

↓

**Improve Answer**

↓

**Final Response**

---

## Advantages

- Can improve completeness
- Can help identify mistakes
- Useful for complex tasks
- Encourages checking against requirements

---

## Important Note

Self-reflection does **not guarantee correctness**.

An AI can review an answer and still fail to detect an error.

Therefore, important information should still be verified independently.

---

# 9. Role-Based Prompting

## Definition

**Role-based prompting** assigns a particular role or area of expertise to the AI.

---

## Examples

> "Act as a mathematics teacher."

> "Act as a C programming tutor."

> "Act as a B.Tech professor."

> "Act as a technical writer."

---

## Example

### Prompt

> "Act as a C programming tutor. Explain pointers to a beginner using simple examples."

The assigned role helps establish the expected perspective and level.

---

## Benefits

- Establishes a clear perspective
- Helps set the appropriate communication style
- Can make explanations more relevant
- Useful for specialized tasks

---

# 10. Persona Prompting

## Definition

**Persona prompting** gives the AI a more specific character, communication style, background, or behavioral perspective.

A persona can include:

- Personality
- Communication style
- Expertise
- Audience awareness
- Teaching style
- Professional characteristics

---

## Example

> "Act as a patient and friendly programming tutor who explains difficult concepts using simple real-life analogies."

The prompt defines more than just the subject expertise.

---

## Another Example

> "Respond like an experienced professor who teaches first-year students and focuses on practical examples."

---

# 11. Role-Based vs Persona Prompting

| Role-Based Prompting | Persona Prompting |
|---|---|
| Defines a role or expertise | Defines a broader style/persona |
| Focuses mainly on function or expertise | Can include personality, behavior, communication style, and expertise |
| "Act as a mathematics teacher" | "Act as a patient mathematics teacher who uses real-life analogies" |
| Usually simpler | Usually more detailed |

---

## Easy Memory

**Role = Who/what expertise?**

**Persona = Who + how they behave/communicate**

---

# 12. Output Control

## Definition

**Output control** means specifying how the AI should structure, format, limit, or organize its response.

Output control can specify:

- Format
- Length
- Number of points
- Number of sections
- Language
- Tone
- Required fields
- Order of information

---

## Example

> "Give exactly five bullet points."

This controls the number and format of the output.

---

## Another Example

> "Answer using a table with three columns."

This controls the structure.

---

# 13. Output Format

Different tasks require different output formats.

Common formats include:

- Paragraph
- Bullet points
- Numbered list
- Table
- JSON
- Structured sections
- Question-answer format
- Step-by-step format

---

# 13.1 Paragraph Format

Prompt:

> "Explain Artificial Intelligence in one paragraph."

---

# 13.2 Bullet Point Format

Prompt:

> "List five applications of Artificial Intelligence using bullet points."

---

# 13.3 Numbered Format

Prompt:

> "Explain the process in five numbered steps."

---

# 13.4 Table Format

Prompt:

> "Compare AI, ML, and Deep Learning in a table."

---

# 13.5 Structured Format

Prompt:

> "Use the following structure:
>
> Definition
>
> Features
>
> Applications
>
> Advantages
>
> Limitations"

---

# 14. JSON Output

## 14.1 What is JSON?

**JSON** stands for:

> **JavaScript Object Notation**

It is a structured data format commonly used for storing and exchanging information between systems.

---

## 14.2 Example

Prompt:

> "Provide information about a programming language in JSON format with the fields: name, type, creator, and applications."

Possible structure:

```text
{
  "name": "Python",
  "type": "Programming Language",
  "creator": "Guido van Rossum",
  "applications": [
    "Web Development",
    "Data Science",
    "Artificial Intelligence"
  ]
}

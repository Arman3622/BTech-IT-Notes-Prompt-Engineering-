# Introduction to LLM (Generative AI) and Prompt Engineering
1. Introduction to Artificial Intelligence (AI)
### What is Artificial Intelligence?

Artificial Intelligence (AI) is a branch of computer science that focuses on creating machines and software capable of performing tasks that normally require human intelligence.

These tasks may include:

Learning
Reasoning
Problem-solving
Understanding language
Recognizing images
Making decisions
Understanding patterns
Generating content
Simple Definition

AI is the ability of a computer system to perform tasks that normally require human intelligence.

Example

When your phone:

recognizes your face,
recommends a YouTube video,
translates a sentence,
detects spam,
predicts the next word while typing,

AI may be involved.

Easy Analogy

Think of AI as a large umbrella.

Under this umbrella are different technologies such as:

AI → Machine Learning → Deep Learning → Generative AI

But these are not exactly the same thing.

2. Types / Areas of AI

AI can be broadly understood through different capabilities.

2.1 Narrow AI

Also called Weak AI.

It is designed to perform a specific task or a limited set of tasks.

Examples:

Face recognition
Spam detection
Recommendation systems
Voice assistants
Chess-playing programs

Most AI systems used today are forms of narrow AI.

2.2 General AI

Also called Artificial General Intelligence (AGI).

The idea is of an AI system capable of performing a very broad range of intellectual tasks at a human-like level.

AGI remains a research goal rather than an established everyday technology.

2.3 Superintelligence

A hypothetical form of AI that would exceed human capabilities across essentially all intellectual domains.

Important: It is mainly a theoretical/future concept.

3. Artificial Intelligence vs Machine Learning vs Deep Learning vs Generative AI

This is a VERY IMPORTANT EXAM TOPIC.

The relationship
Artificial Intelligence (AI)
│
└── Machine Learning (ML)
    │
    └── Deep Learning (DL)
        │
        └── Some Generative AI systems

However, remember:

Generative AI is not simply another level of ML/DL. It is a category of AI systems designed to generate new content, and many modern generative systems use deep learning.

3.1 Artificial Intelligence

AI is the broadest concept.

It includes techniques that enable computers to perform intelligent tasks.

Examples
Rule-based systems
Expert systems
Machine learning
Deep learning
Generative AI
3.2 Machine Learning
Definition

Machine Learning (ML) is a subset of AI in which computers learn patterns from data and use those patterns to make predictions or decisions.

Instead of explicitly programming every rule, we provide data and allow the system to learn patterns.

Traditional programming
Rules + Data
     ↓
   Program
     ↓
   Output
Machine Learning
Data + Expected Outputs
        ↓
   ML Algorithm
        ↓
      Model
        ↓
 Prediction on New Data
Example

Suppose we want to detect spam emails.

Instead of manually writing thousands of rules:

"If email contains X, Y and Z → spam"

we can train a model using many examples of:

Spam emails
Normal emails

The model learns patterns associated with spam.

4. Deep Learning
Definition

Deep Learning (DL) is a subset of Machine Learning that uses artificial neural networks with multiple layers to learn complex patterns from large amounts of data.

Common applications
Image recognition
Speech recognition
Natural language processing
Autonomous systems
Generative AI
Example

For face recognition:

Image
 ↓
Input Layer
 ↓
Hidden Layers
 ↓
Features
 ↓
Output
 ↓
Recognized Face

Deep learning is particularly powerful when dealing with complex, high-dimensional data.

5. Generative AI
Definition

Generative AI is a type of AI that can create new content based on patterns learned from data.

It can generate:

Text
Images
Audio
Video
Code
Music
Synthetic data
Examples

A generative AI system can:

"Write a C program to calculate the factorial of a number."

and produce new code.

Or:

"Create an image of a futuristic city."

and generate an image.

Traditional AI vs Generative AI
Traditional AI	Generative AI
Often predicts/classifies	Generates new content
Spam/not spam	Writes an email
Cat/dog classification	Creates an image
Fraud/not fraud	Generates a report
Predict house price	Generates text/code
Easy Analogy

Think of:

Traditional AI = Judge

It decides:

"This is spam."

Generative AI = Creator

It produces:

"Here is a new email."

6. AI vs ML vs DL vs Generative AI — Quick Comparison
Feature	AI	ML	DL	Generative AI
Meaning	Broad field of intelligent machines	Learning from data	ML using deep neural networks	AI that generates content
Main purpose	Intelligent behavior	Prediction/decision	Complex pattern learning	Content generation
Data requirement	Varies	Usually data-driven	Usually large datasets	Often very large datasets
Example	Expert system	Spam detector	Face recognition	ChatGPT
Relationship	Broadest	Subset of AI	Subset of ML	Category of AI; often powered by DL
⭐ Exam Memory Trick

AI = Intelligence
ML = Learning
DL = Deep neural learning
GenAI = Generation

7. What is an LLM?
LLM = Large Language Model

A Large Language Model (LLM) is an AI model trained on very large amounts of text/data so that it can understand and generate human-like language.

LLMs can perform tasks such as:

Answering questions
Summarizing text
Translation
Writing
Coding
Classification
Information extraction
Brainstorming
Conversational interaction

Examples include models used in:

ChatGPT
Claude
Gemini
Grok
DeepSeek
8. Why is it called "Large Language Model"?

Let's break the term down.

Large

The model contains a very large number of learned parameters and is generally trained using substantial computational resources and datasets.

Language

It is designed to work with human language and, depending on the model, other modalities such as code, images, audio, etc.

Model

It is a mathematical/computational system that learns patterns from data.

Therefore:

Large + Language + Model = Large Language Model

9. How Does an LLM Basically Work?

A simplified view:

User Prompt
     ↓
Tokenization
     ↓
Tokens
     ↓
Neural Network / Transformer
     ↓
Pattern & Context Processing
     ↓
Next-token prediction
     ↓
Generated Output
Step 1 — Input

The user provides a prompt.

Example:

"Explain machine learning in simple words."

Step 2 — Tokenization

The text is converted into smaller units called tokens.

A token may represent:

A word
Part of a word
A punctuation mark
Other pieces of text
Step 3 — Processing

The model processes these tokens using its learned parameters and architecture.

Many modern LLMs are based on the Transformer architecture.

The Transformer architecture was introduced in the 2017 research paper "Attention Is All You Need."

Step 4 — Prediction

At a simplified level, the model predicts what token is likely to come next based on the context.

For example:

The sun rises in the ___

Possible prediction:

east

The model repeats this process to generate a sequence of tokens.

Important clarification

An LLM is not simply searching a database and copying an answer.

It generates output using patterns learned during training and the context provided at inference time.

10. What is a Transformer?

A Transformer is a neural-network architecture that became highly influential in modern language models.

Its important idea is attention.

Attention

Attention helps a model determine which parts of the input are important when processing a particular part of the sequence.

Simple example

Consider:

"The student put the laptop on the table because it was heavy."

To understand what "it" refers to, the model needs to consider the surrounding context.

Attention mechanisms help models capture relationships between different parts of a sequence.

Exam Definition

Transformer is a neural-network architecture based primarily on attention mechanisms and widely used in modern language models.

11. What is Prompt Engineering?
Definition

Prompt Engineering is the process of designing, structuring, and refining instructions given to an AI model to obtain useful, accurate, relevant, and well-formatted outputs.

Simple definition

Prompt Engineering = Asking AI the right way to get the desired result.

12. Why is Prompt Engineering Important?

A vague prompt may produce a vague answer.

Weak prompt

"Tell me about AI."

The AI doesn't know:

How detailed?
For whom?
Exam or general knowledge?
Which topics?
What format?
Better prompt

"Explain Artificial Intelligence for a first-year B.Tech student in simple language. Include definition, applications, advantages, limitations, examples, and a short exam-oriented summary."

This gives the AI much clearer instructions.

13. RTCCO Prompt Framework

This is an important framework for writing structured prompts.

RTCCO
Letter	Meaning	Purpose
R	Role	Tell AI who it should act as
T	Task	Tell AI what to do
C	Context	Provide background information
C	Constraints	Define limitations/rules
O	Output	Define the desired format
R — Role

Tell the AI what role or perspective it should take.

Example

"Act as a B.Tech professor."

T — Task

Clearly state what you want.

Example

"Explain Machine Learning."

C — Context

Give useful background.

Example

"The students are first-year B.Tech IT students with basic programming knowledge."

C — Constraints

Specify limitations.

Example

"Use simple English. Avoid unnecessary technical jargon. Keep the explanation exam-oriented."

O — Output

Tell the AI how you want the response.

Example

"Use headings, tables, examples, and a short revision section."

14. Complete RTCCO Example
Prompt

Role: Act as a B.Tech professor.
Task: Explain Machine Learning.
Context: The learners are first-year B.Tech IT students.
Constraints: Use simple language and practical examples. Keep it suitable for university exams.
Output: Give definition, working, types, examples, advantages, limitations, and five revision questions.

Final Prompt

"Act as a B.Tech professor. Explain Machine Learning to first-year B.Tech IT students. Use simple language and practical examples, avoid unnecessary jargon, and make it suitable for university exams. Structure the answer with definitions, working, types, examples, advantages, limitations, and five revision questions."

15. Important Elements of a Good Prompt

A strong prompt generally contains:

Clear Goal
    +
Relevant Context
    +
Specific Instructions
    +
Constraints
    +
Desired Output Format
Weak

"Explain programming."

Strong

"Act as a programming instructor. Explain C loops to a first-year B.Tech student who knows basic C syntax. Use simple examples, compare for/while/do-while loops in a table, and finish with five practice questions."

16. Common Prompting Techniques
16.1 Zero-Shot Prompting

The model is asked to perform a task without examples.

Example

"Classify this review as positive or negative: 'The movie was excellent.'"

No examples are provided.

16.2 Few-Shot Prompting

The prompt provides a few examples before asking the model to perform the task.

Example
Happy → Positive
Terrible → Negative
Excellent → Positive

Amazing → ?

Expected output:

Positive

16.3 Role Prompting

Give the AI a role.

"Act as a mathematics professor."

Useful when a specific perspective, tone, or teaching style is required.

16.4 Instruction Prompting

Clearly tell the AI what action to perform.

"Summarize this paragraph in five bullet points."

16.5 Structured Output Prompting

Specify the output format.

"Give the answer in a table with columns: Topic, Definition, Example."

This is especially useful for notes and data extraction.

16.6 Iterative Prompting

Instead of trying to create the perfect prompt in one attempt:

Prompt
 ↓
Output
 ↓
Review
 ↓
Improve Prompt
 ↓
Better Output

This is often called an iterative approach to prompting.

17. Good Prompt vs Bad Prompt
Bad Prompt	Better Prompt
Tell me AI	Explain AI for a first-year B.Tech student
Write something	Write a 200-word introduction to AI
Explain C	Explain C loops with examples
Make notes	Make exam-oriented notes with headings and tables
Tell me about ML	Compare ML and DL with examples and a difference table
Golden Rule

The clearer your instructions, the easier it is for the model to produce the type of answer you want.

However, a detailed prompt does not automatically guarantee a correct answer. AI output should still be checked.

18. History of Large Language Models

Understanding LLM history helps us understand how today's generative AI developed.

Simplified Timeline
Early AI & NLP
     ↓
Statistical Language Models
     ↓
Neural Language Models
     ↓
Transformer — 2017
     ↓
GPT-3 — 2020
     ↓
InstructGPT — 2022
     ↓
ChatGPT — 2022
     ↓
Rapid growth of LLMs
     ↓
Multimodal & reasoning-oriented models
     ↓
Modern AI assistants
19. Transformer — 2017

The 2017 paper "Attention Is All You Need" introduced the Transformer architecture, which became foundational to the development of many modern language models.

Why was it important?

Transformers made it easier to process relationships between tokens and efficiently train large models.

This became one of the major technological foundations behind modern LLMs.

20. GPT-3 — 2020

OpenAI introduced GPT-3 in 2020.

GPT-3 demonstrated strong few-shot learning, where a model could perform tasks from instructions and a small number of examples without task-specific parameter updates.

Importance

GPT-3 helped demonstrate that scaling language models could produce surprisingly broad capabilities.

21. InstructGPT — 2022

A major development was improving models so that they could better follow human instructions.

OpenAI described InstructGPT as using human feedback to improve instruction following, truthfulness, and safety.

This idea became important for conversational AI.

22. ChatGPT

ChatGPT was publicly introduced by OpenAI on November 30, 2022 as a conversational AI system.

It became highly influential because users could interact with an AI using natural language rather than traditional programming interfaces.

Major capabilities
Question answering
Writing
Summarization
Coding
Brainstorming
Translation
Learning assistance
Conversational interaction
Why ChatGPT became important

It made generative AI accessible to ordinary users through a simple chat interface.

23. GPT-4

OpenAI introduced GPT-4 in March 2023. OpenAI described it as a major improvement over earlier GPT systems in areas including reasoning and safety.

This represented another major stage in the evolution of general-purpose LLMs.

24. Claude

Claude is an AI assistant developed by Anthropic.

Anthropic introduced Claude more broadly in March 2023.

Claude was designed around Anthropic's emphasis on helpful, honest, and harmless AI.

Constitutional AI

Anthropic developed an approach called Constitutional AI, where explicit principles are used to guide model behavior.

Claude can be used for:
Writing
Summarization
Coding
Question answering
Document analysis
Reasoning
Research assistance

Claude has evolved significantly since its initial release, so model-specific capabilities change over time.

25. Google Gemini

Gemini is Google's family of generative AI models and products.

Google announced Gemini in December 2023, describing it as a multimodal model family available in different sizes such as Ultra, Pro, and Nano at launch.

Gemini is associated with Google's broader ecosystem and can handle tasks involving different types of information depending on the specific model/product.

Common uses
Question answering
Writing
Coding
Summarization
Multimodal understanding
Research assistance
26. Grok AI

Grok is an AI assistant developed by xAI.

The current Grok ecosystem includes conversational interaction, coding, file analysis, image/video generation, voice interaction, and tool connections; capabilities depend on the current product/model version.

Common uses
General questions
Brainstorming
Coding
Content creation
File analysis
Multimodal tasks
27. DeepSeek

DeepSeek is an AI company and model family known particularly for research into efficient and capable language models.

DeepSeek released DeepSeek-V3 in December 2024 and DeepSeek-R1 in January 2025. DeepSeek described R1 as a reasoning-focused model and released its model and technical report under an open-access-oriented approach, including MIT licensing for R1.

DeepSeek's model family has continued to evolve; its official transparency page currently lists later releases including V4.

Common areas
Mathematics
Coding
Reasoning
General question answering
Research
AI development
28. ChatGPT vs Claude vs Gemini vs Grok vs DeepSeek

Important: AI models are updated frequently. Therefore, don't memorize a particular model version or benchmark ranking as a permanent fact. For exams, focus on the general characteristics and differences.

AI	Developed by	General identity / strengths
ChatGPT	OpenAI	General-purpose AI assistant, writing, coding, reasoning and multimodal capabilities
Claude	Anthropic	Strong emphasis on helpfulness, safety, long-context work, writing and coding
Gemini	Google	Multimodal AI closely connected with Google's AI ecosystem
Grok	xAI	General AI assistant with conversational, coding and multimodal capabilities
DeepSeek	DeepSeek	Known for efficient/open-access-oriented model development and strong reasoning/coding models
Easy Memory
ChatGPT → General-purpose assistant
Claude  → Writing / long-context / safety-oriented approach
Gemini  → Google ecosystem + multimodal
Grok    → xAI + conversational/multimodal
DeepSeek → Efficient models + reasoning/coding

These are broad study-level descriptions, not permanent rankings.

29. Applications of Prompt Engineering

Prompt engineering is useful in many fields.

29.1 Education

AI can help:

Create study notes
Generate practice questions
Explain difficult topics
Create revision summaries
Generate examples
Example

"Explain Kirchhoff's laws as if teaching a first-year engineering student. Give one real-life analogy and three numerical practice questions."

29.2 Software Development

Prompts can help with:

Code generation
Debugging
Code explanation
Documentation
Test-case generation
Learning programming
Example

"Explain this C program line by line and identify syntax and logical errors."

29.3 Content Creation

AI can assist with:

Blog writing
Social media content
Email drafts
Scripts
Ideas
Summaries
29.4 Business

Applications include:

Report generation
Customer support
Data analysis assistance
Market research
Documentation
Communication
29.5 Healthcare

Potential applications include:

Summarizing medical documents
Administrative assistance
Information extraction
Patient communication support

Important: AI output in healthcare should be reviewed by qualified professionals; AI should not automatically replace professional judgment.

29.6 Research

AI can assist with:

Literature summarization
Brainstorming
Data interpretation
Coding assistance
Draft organization
30. Advantages of Generative AI
1. Productivity

Can automate repetitive content-related tasks.

2. Accessibility

Natural language makes advanced tools easier to interact with.

3. Learning assistance

Can explain concepts at different levels.

4. Creativity

Can generate ideas and drafts.

5. Coding assistance

Can explain, generate and debug code.

6. Personalization

Responses can be adapted according to user instructions.

31. Limitations of Generative AI

This is very important for exams.

1. Hallucination

AI may generate information that sounds convincing but is incorrect or unsupported.

2. Bias

Models can reflect biases present in their training data or development process.

3. Lack of guaranteed accuracy

AI output should not automatically be treated as fact.

4. Privacy concerns

Sensitive information should not be casually entered into AI systems.

5. Dependence

Excessive reliance can reduce independent thinking and learning.

6. Copyright and intellectual-property concerns

AI-generated or AI-assisted content can raise questions about ownership, licensing, attribution and use of training material.

7. Security risks

AI systems can potentially be misused or manipulated.

32. Hallucination in LLMs
Definition

An AI hallucination occurs when an AI system produces information that appears plausible but is incorrect, fabricated, or unsupported.

Example

User:

"Give me a research paper by XYZ published in 2012."

If no such paper exists, an AI might sometimes incorrectly invent a title, author, or publication details.

How to reduce the risk
Ask for sources when appropriate.
Verify important facts.
Cross-check dates and statistics.
Use reliable primary sources.
Don't blindly trust confident wording.
Exam Definition

Hallucination is the generation of false, inaccurate, or unsupported information by an AI model, often presented in a convincing manner.

33. Prompt Engineering and Hallucination

Good prompting can reduce some errors but cannot guarantee correctness.

Better prompt

"Answer only using the information provided below. If the information is insufficient, say 'insufficient information' instead of guessing."

This encourages the model to avoid unsupported assumptions.

34. Opportunities and Career Scope

Generative AI and LLMs are creating opportunities across many technology roles.

34.1 AI/ML Engineer

Works on:

Machine learning models
AI systems
Data
Model deployment
Evaluation
34.2 Generative AI Engineer

Works on:

LLM applications
AI assistants
RAG systems
AI APIs
Evaluation
Prompting
AI workflows
34.3 Prompt Engineer / AI Workflow Specialist

Focuses on:

Prompt design
Prompt evaluation
AI workflows
Output quality
Task automation

Important: Prompt engineering is increasingly becoming one skill within broader AI/product/development roles rather than necessarily being a completely isolated career for every organization.

34.4 Data Scientist

Uses:

Statistics
Programming
Machine learning
Data analysis
Visualization
34.5 NLP Engineer

NLP = Natural Language Processing

Works with technologies involving:

Text
Speech
Language understanding
Information extraction
Translation
Language models
34.6 AI Product Manager

Combines:

Technology
User needs
Product design
Business requirements
AI capabilities
34.7 AI Researcher

Works on:

New AI algorithms
Model architectures
Training methods
Evaluation
Safety
Reasoning
35. Skills Needed for a Career in Generative AI

For a B.Tech IT student, a useful progression is:

Programming
     ↓
Python
     ↓
Data Structures & Algorithms
     ↓
Math + Statistics
     ↓
Machine Learning
     ↓
Deep Learning
     ↓
NLP
     ↓
LLMs
     ↓
Generative AI
     ↓
Projects
Useful skills
Python
Data Structures
Machine Learning
Deep Learning
NLP
SQL
Git/GitHub
APIs
Prompt Engineering
RAG
Model evaluation
Basic cloud/deployment knowledge
36. Prompt Engineering vs Programming
Prompt Engineering	Programming
Uses natural-language instructions	Uses programming languages
Guides an existing AI model	Builds software/system logic
Faster to experiment	More control and precision
Useful for AI interaction	Essential for software development
Can be learned alongside coding	Core B.Tech IT skill
Important for you as a B.Tech IT student

Don't think:

"If I learn prompting, I don't need programming."

Instead:

Programming + AI + Prompt Engineering = stronger combination.

37. Case Study — AI Study Assistant
Problem

A B.Tech student has difficulty understanding a difficult engineering topic.

Traditional approach

The student:

Searches the internet.
Opens multiple websites.
Reads long explanations.
Creates notes manually.
Generative AI approach

The student gives a structured prompt:

"Act as a B.Tech professor. Explain resonance in an RLC circuit for a first-year engineering student. Start with a simple analogy, then explain the technical definition, formula, conditions, graph, applications, and exam-important points. End with five practice questions."

Result

The AI can generate a structured learning resource.

But the student should:
AI Explanation
      ↓
Check textbook/teacher material
      ↓
Verify formulas
      ↓
Understand concept
      ↓
Make final notes
      ↓
Practice questions
Lesson

AI should be used as a learning assistant, not as a replacement for learning.

38. Real-Life Example of RTCCO
Scenario

You want AI to explain C programming.

R — Role

"Act as a C programming professor."

T — Task

"Explain for loops."

C — Context

"I am a first-year B.Tech IT student and know basic C syntax."

C — Constraints

"Use simple English and beginner-friendly examples."

O — Output

"Give definition, syntax, flow, example program, common mistakes, and five practice questions."

Complete Prompt

Act as a C programming professor. Explain for loops to a first-year B.Tech IT student who knows basic C syntax. Use simple English and beginner-friendly examples. Include definition, syntax, working, example program, common mistakes, and five practice questions.

That's a well-engineered prompt.

39. Important Terminology
Term	Meaning
AI	Artificial Intelligence
ML	Machine Learning
DL	Deep Learning
GenAI	Generative Artificial Intelligence
LLM	Large Language Model
NLP	Natural Language Processing
Prompt	Instruction/input given to an AI model
Prompt Engineering	Designing effective prompts
Token	Unit of text processed by a model
Transformer	Neural-network architecture widely used in modern LLMs
Parameter	Learned value within a model
Inference	Using a trained model to generate an output
Training	Process of learning patterns from data
Hallucination	Incorrect or unsupported AI-generated information
Multimodal AI	AI capable of working with multiple modalities such as text, images, audio, etc.
40. Most Important Differences for Exams
AI vs ML

AI is the broader field of creating intelligent systems, while ML is a subset of AI where systems learn patterns from data.

ML vs DL

ML includes many learning techniques, whereas DL specifically uses multi-layer neural networks to learn complex patterns.

DL vs GenAI

Deep Learning is a method/approach based on deep neural networks, whereas Generative AI refers to AI systems designed to generate new content. Many modern GenAI systems use deep learning.

AI vs GenAI

AI can perform tasks such as prediction, classification and decision-making, while Generative AI focuses on producing new content such as text, images, audio, video or code.

41. Important Exam Questions
Short-answer questions
Define Artificial Intelligence.
What is Machine Learning?
Define Deep Learning.
What is Generative AI?
What is an LLM?
What is Prompt Engineering?
What is a Transformer?
What is a token?
What is AI hallucination?
What is RTCCO?
Medium-answer questions
Differentiate AI, ML, DL and Generative AI.
Explain the working of an LLM.
Explain Prompt Engineering with an example.
Explain the RTCCO framework.
Explain zero-shot and few-shot prompting.
Explain the evolution of LLMs.
Explain the development of ChatGPT.
Explain Claude and Constitutional AI.
Discuss applications of Generative AI.
Discuss career opportunities in Generative AI.
Long-answer questions
Q1. Explain AI, Machine Learning, Deep Learning and Generative AI with suitable examples.
Q2. Explain Large Language Models and their basic working.
Q3. What is Prompt Engineering? Explain the RTCCO framework with a suitable example.
Q4. Explain the evolution of LLMs from Transformers to modern AI assistants.
Q5. Compare ChatGPT, Claude, Gemini, Grok and DeepSeek.
Q6. Discuss the applications, advantages and limitations of Generative AI.
Q7. Discuss the opportunities and career scope in Generative AI.

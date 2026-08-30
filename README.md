# LBF Assistant - AI Study Assistant for Primary School Students

**AnalystLab Africa | Generative AI Internship Programme**

The name LBF stands for "Leave Better Found" - a personal value meaning to leave people better than you found them. The assistant follows this idea by helping students understand a topic more deeply than before they asked.

![Assistant architecture](Assistant%architecture.png)

## Overview

LBF Assistant is an AI study assistant designed to help primary school students and their tutors.
It supports four tasks: explaining concepts, creating quizzes, summarizing notes, and recommending study plans.
All responses are based strictly on documents the user provides, to keep the content accurate and aligned with what the student is actually studying.

## Business Problem

Students understand concepts differently, and a teacher cannot always be available to adjust their teaching style for every student. This is even harder for primary school students, who do not yet have much background knowledge to build new explanations on. LBF Assistant helps close this gap by offering support that adapts to the student's level, any time a teacher is not available.

**Target users:** Primary school students and their tutors/teachers.

## What the Assistant Can Do

- **Explain concepts** 
- **Create quizzes** 
- **Summarize notes** 
- **Recommend study plans** 

## How It Works

The system is built in layers:

1. **Global layer** : shared by all four tasks: who the assistant is, how it greets the user, and the safety rules it must always follow.

2. **Task loader** : picks the right task (Concept Explanation, Quizzes, Summarization, or Study Plan) based on what the user selects.

3. **Task-specific rules** : each task has its own step-by-step checklist the assistant must follow, in order, before it is allowed to respond.

4. **Formatted response** : the final answer is sent back to the user in a clear, structured format.

## Repository Structure

```
├── README.md                          
├── AI Solution.pdf                    
├── System Prompt.pdf                  
├── Prompt Library.pdf                 
├── Conversation Flow.pdf             
├── Prompt Evaluation.pdf              
└── Responsible AI Assessment.pdf     
```



##️ Responsible AI

The assistant was reviewed against six risk areas: hallucination, bias, privacy, security, ethical use, and the need for human oversight. Key safeguards include:

- Every response must be grounded in a user-provided document.

- Examples that could emotionally harm a student (e.g. referencing parents in a way that could distress student without ones ) are explicitly avoided.

- The assistant refuses to discuss its own configuration or be redirected away from its assigned task, even under pressure.

- Quiz answers are kept in a separate section so a tutor can hide them from the student until they've attempted the questions.

Full details, including known gaps and recommendations, are in `Responsible_AI_Assessment.pdf`.

## Future Improvements

- Build a working app (e.g. with Streamlit) around this design.
- Add checks for personally identifiable information in uploaded documents.

##️ Tools Used

Google Gemini

## Author

Luc Agbognisso

Generative AI Intern, AnalystLab Africa


*#AnalystLabAfrica*

# agile-professional-project

A Python web assistant prototype that uses an LLM and retrieval-augmented generation (RAG) to help STAR programme students find university information with clear source links.

## Project aim

This second-year CO2007 Agile Professional team project aims to make university information easier to find for disabled students preparing for the Student Transition and Residential (STAR) programme. Answers to common questions are spread across many university web pages. We intend to bring that information together through a simple, accessible question-and-answer interface that works on computers and mobile devices.

## How it will likely work

1. Save a dated copy of the approved public Lancashire.ac.uk web pages and keep it in the repository. The prototype will use this fixed collection rather than fetch live pages when answering questions.
2. Split the saved content into smaller passages and make them searchable.
3. When someone asks a question, retrieve the most relevant passages and pass them to a language model with instructions to answer using only that information.
4. Show a clear answer alongside links to its source pages. If the pages do not contain an answer, say so rather than guess.

The planned application will use Python with a browser-based interface. The exact tools are still to be decided, with a free or local language model that can be replaced through configuration. Accessibility and plain language will guide the design. For distress or crisis questions, the assistant should direct users to appropriate human support instead of trying to give advice.

## Why use RAG?

RAG combines searching trusted information with generating a readable answer. A language model on its own may invent details or rely on outdated information about university services. Retrieving passages from the approved pages gives it relevant evidence and lets users check where an answer came from.

This matters when students are looking for support: misleading information could create confusion or prevent them from finding the right help. RAG can reduce unsupported answers, but it does not guarantee accuracy. We plan to test answers against expected responses and compare the assistant with a simple keyword-search baseline to see what the language model adds.

## Current status

The project is at the planning stage; no application has been implemented yet. This is a prototype, with testing limited to students on the module and the client, using made-up questions rather than personal or health information.

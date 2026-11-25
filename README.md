# agile-professional-project

We’re building a small Python assistant to help students find university support information using saved university pages, with clear source links. We’re currently exploring initial prototypes using Disability and Inclusive Support.

## Project aim

This second-year CO2007 Agile Professional team project aims to make university support information easier to find, starting with Disability and Inclusive Support, including STAR, and Mental Health and Wellbeing. We intend to provide a simple, accessible question-and-answer interface that works on computers and mobile devices.

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

Sprint 2 runs from 25 November to 8 December 2026. Each team member is attempting an initial prototype using the saved Disability and Inclusive Support page, aiming to answer at least one question with its source. Console and local web versions are both welcome during this phase. Our internal review is on 9 December.

See the [wiki](https://github.com/amounderness/agile-professional-project/wiki/Start-Here) for the requirements and build plan, and [Team Planning](https://github.com/users/amounderness/projects/3) for current tasks. Testing is limited to students on the module and the client, using fictional questions rather than personal or health information.

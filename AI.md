# AI.md

## Overview

This document describes the AI components used in this project, including archetecture, prompt structure, and guidelines for the use of AI capabilities.

## AI Capabilities

- Natural Language Processing: Generates summaries, anwsers questions, and assists with content creation.
- Classification Tasks: Categorizes inputs such as text and user quieres.
- Automation: Supports data visualizations based on AI predictions.

## Model Details

|  Model Provider           |  Model Name  |    Versioning      |
| ------------------------- |:------------:|:------------------:|
| Tableau                   | Tableau Prep | 2025.3.1 12/17/2025 |
| Microsoft 365 integration | Copilot      | GPT-5    08/07/2025|
| OpenAI                    | Chat GPT     | GPT-5.2  01/19/2026|
| Google Deepmind           | Gemini       | Gemini-3 12/17/2025|

## Safety and Gaurdrail

- AI cannot perform full set coding opperations
- AI will not be used to perform analysis for users
- AI can be used for assistance, inquiries, and automated visualizations via Tableau
- Outputs will be filtered for hallucinations and bias
- Logs of usage will be stored in AI.md

## AI Usage Logs

- Model: Tableau
  - Prompter: Elton
  - Prep Builder provides features such as automated filtering, data cleaning tools, and "Smart Features".
  - Used the Tableau "forecast" feature to develop a predicted forecast of our sales for the next year.
- Model: Google (Gemini generation when perfomring a search)
  - Prompter : Elton
  - When searching how to forcast in Tableau, AI provided insights on how to use the forcasting tool.

- Model: Gemini
  - Prompter: Bea
  - Prompt: "What types of calculations could be used for sales tracking in Tableau?"
  - Response: Provided a run down of basic calculations used, how some expressions would look when typed into "create a field", provided LOD expressions, explained how to handle nulls, and provided video links on how to implement certain calculated fields in Tableau.

- Model: chat GPT
  - Prompter: Bea
  - Prompt: "My companies name it Timeless Transport Models. Can you make me a simplistic logo of a classic car."
  - Response: Provided an image generation of a car with the name "Timeless Transport Models." This image is used as the logo throughout the project. All imagery presented in this project is AI generated. (Except the visualizations)
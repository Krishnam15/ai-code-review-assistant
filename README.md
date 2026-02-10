# AI Code Review Assistant

## Problem Statement
Code reviews are time-consuming and often inconsistent, especially in fast-paced development environments. Developers need quick, actionable feedback on code quality, potential issues, and best practices before submitting changes for human review.

## Solution Overview
AI Code Review Assistant is an AI-powered tool that analyzes source code and provides structured feedback on code quality, readability, potential bugs, and improvement suggestions. The system leverages large language models (LLMs) to simulate an automated first-pass code review, helping developers catch issues early and improve overall code quality.

## Key Features
- AI-generated code review feedback for submitted code snippets
- Suggestions related to readability, best practices, and potential issues
- Code optimization submissions for better time and space complexity.
- Prompt-driven analysis tailored for developer-oriented feedback
- Clean and minimal interface for submitting and reviewing code
- Secure handling of API keys using environment variables

## System Design / Architecture
1. User submits a code snippet through the interface  
2. The input code is formatted into a structured review prompt  
3. The prompt is sent to the OpenAI API for analysis  
4. The model generates a detailed review response  
5. The feedback is displayed back to the user in a readable format  

The architecture is designed to be modular, allowing future extensions such as language-specific reviews, diff-based reviews, or multi-file analysis.

## Tech Stack
- React
- Vite
- OpenAI API
- LangChain
- Bun (package manager)
  
## Getting Started

To get your local environment set up and running, follow these simple steps:

1.  **Clone the repository:**

```
  git clone https://github.com/jjxmonster/ai-code-review-assistant
```

2.  **Install dependencies:**

Navigate to the project directory and run:

```
  bun install
```

3.  **Set up your `.env` file:**

Create a `.env` file in the root of your project and add your OpenAI API key:

```
  VITE_OPENAI_API_KEY=your_openai_api_key_here
```

Replace `your_openai_api_key_here` with your actual OpenAI API key.

## Results 

- Enables faster feedback loops during development
- Helps identify common code quality issues before human review
- Demonstrates practical application of LLMs in developer tooling
- Reduces manual effort for basic code review tasks

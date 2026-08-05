# 🤖 AI Software Engineer Multi-Agent

An AI-powered multi-agent system that automates software engineering tasks on Python repositories using Large Language Models (LLMs).

The project analyzes a GitHub repository, reviews the source code, generates unit tests, executes them, fixes detected issues, validates the corrections, and produces a final engineering report.

---

# 🚀 Features

- Clone any public GitHub repository
- Analyze Python source code
- Generate AI-powered code reviews
- Automatically generate pytest unit tests
- Execute all generated tests
- Fix detected issues using an LLM
- Validate the corrected code
- Generate engineering reports

---

# 🏗 Multi-Agent Architecture

## 🤖 Agent 1 — Repository Manager

Responsibilities:

- Clone the GitHub repository
- Prepare the local workspace
- Locate Python source files
- Load source code

---

## 🤖 Agent 2 — AI Code Reviewer

Responsibilities:

- Analyze every Python source file
- Detect bugs
- Detect code smells
- Detect security issues
- Detect performance problems
- Produce AI code reviews

Outputs:

- Code review report

---

## 🤖 Agent 3 — AI Test Generator

Responsibilities:

- Read source code
- Read code review
- Generate pytest unit tests
- Save generated tests
- Execute pytest

Outputs:

- Generated tests
- Pytest execution report

---

## 🤖 Agent 4 — Validation Agent

Responsibilities:

- Analyze pytest results
- Determine repository health
- Count passed tests
- Count failed tests
- Prepare validation summary

Outputs:

- Validation report

---

## 🤖 Agent 5 — AI Bug Fixer

Responsibilities:

- Read original source code
- Read AI code review
- Read pytest failures
- Generate corrected Python code
- Save corrected files

Outputs:

- Fixed source code

---

## 🤖 Agent 6 — Final Report Generator

Responsibilities:

- Compare repository status before and after fixes
- Generate final engineering report
- Summarize improvements

Outputs:

- Final AI Software Engineering Report

---

# 🔄 Workflow

```text
GitHub Repository
        │
        ▼
Agent 1
Repository Manager
        │
        ▼
Agent 2
AI Code Review
        │
        ▼
Agent 3
Generate Tests + Run Pytest
        │
        ▼
Agent 4
Validation
        │
        ▼
Agent 5
AI Bug Fixer
        │
        ▼
Run Tests Again
        │
        ▼
Agent 6
Final Engineering Report
```

---

# 📁 Generated Outputs

The notebook automatically creates:

```
workspace/
│
├── generated_tests/
│     ├── test_*.py
│
├── reports/
│     ├── code_reviews.md
│     ├── test_results.md
│     ├── validation_report.md
│     └── final_report.md
│
└── fixed_code/
      └── corrected source files
```

---

# 🛠 Technologies

- Python
- OpenAI API
- GPT Models
- Pytest
- GitPython
- Google Colab
- tqdm

---

# 📊 Example Final Report

```
============================================================
FINAL AI SOFTWARE ENGINEER REPORT
============================================================

Repository:
sampleproject

Files Reviewed:        5
Tests Generated:       27

Before Fix
------------
Passed: 22
Failed: 5

After Fix
-----------
Passed: 27
Failed: 0

Repository Status
-----------------
✅ Repository successfully repaired.
```

---

# 🎯 Future Improvements

- Multi-language support (Java, JavaScript, Go, Rust, C#)
- Automatic pull request generation
- GitHub Actions integration
- Coverage reporting
- Security vulnerability scanning
- Docker support
- Streamlit web interface
- Multi-LLM support (GPT, Claude, Gemini, Llama)

---

# 👨‍💻 Author

**Saloum Dieng Seck**

AI Engineer | Multi-Agent Systems | RAG | LLM Applications

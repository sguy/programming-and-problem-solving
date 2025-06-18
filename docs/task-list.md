# PAPS Project Plan & Task List

This document outlines the phased project plan and associated tasks for implementing the PAPS project, as derived from the `copilot-instructions.md` document.

This plan is designed to be iterative. Some tasks, especially around notebook development and refinement, will be ongoing.

## Phase 1: Foundation & Development Environment Setup

* **Goal:** Establish a robust development environment, CI/CD pipeline, and core project structure.
* **Tasks:**
    1. **Project Setup:**
        * [x] Initialize GitHub repository.
        * [x] Create `README.md` with basic project overview.
        * [x] Set up `.gitignore` for Python and common OS files.
        * [x] Establish project directory structure (e.g., `src/`, `tests/`, `docs/`, `notebooks/`).
    2. **Python Environment:**
        * [x] Set up `venv` and create initial ``pyproject.toml`
    3. **Development Tooling Configuration:**
        * [x] Configure Ruff for linting (e.g., `pyproject.toml` or `ruff.toml`).
        * [x] Configure Black for formatting (e.g., `pyproject.toml`).
        * [x] Ensure PEP-8 compliance is enforced by linters.
        * [x] Configure Mypy for static type checking (in `pyproject.toml`).
        * [x] Configure pre-commit hooks for Ruff and Black.
    4. **Continuous Integration (GitHub Actions):**
        * [x] Create a basic GitHub Actions workflow for:
            * [x] Checking out code.
            * [x] Setting up Python.
            * [x] Installing dependencies.
            * [x] Running Ruff linter.
            * [x] Running Black formatter (check mode).
            * [x] Running Pytest.
    5. **Documentation:**
        * [x] Confirm `copilot-instructions.md` is up-to-date and in the repository.
        * [x] Establish a `docs/` directory for further Markdown documentation.

## Phase 2: Brainstorm Ideas for Notebooks

  1. **Programming Concepts to cover**

  2. **Problem solveing techniques**

  3. **Tie-ins to other disciplines**

    - Mathematics
      - Calculus
      - Set Theory
      - Factoring
    - Biology
      - Genetics
    - Physics
      - Projectiles
      - Orbits
    - Computer Science
      - Sorting
      - Encoding & Encryption
    - Finance
      - Compound interest

## Phase 3: Initial Notebooks

* **Goal:** Write the first 2-3 notebooks which will provide an introduction to the Jupyter notebook environment and the Python programming language.
* **Tasks:**
    1. **Notebook 1**
        * [x] Create `notebooks/01-getting-started.ipynb`which covers the following:
          * [x] Understanding Jupyter Notebooks and their cell-based structure (Markdown vs. Code cells).
          * [x] Navigating and using the Google Colab interface (e.g., adding/deleting cells, using the Table of Contents, saving to Google Drive, managing AI assistant settings).
          * [x] Writing, editing, and rendering basic Markdown (e.g., headings, lists).
          * [x] Running Python code cells and observing their output.
    2. **Notebook 2**
        * [ ] Create `notebooks/02-first-steps-with-python.ipynb`which covers the following:
          * [ ] What is programming? (Conceptual introduction)
          * [ ] Using the `print()` function for output
          * [ ] Variables
          * [ ] Introduction to Types
            * Strings (str)
            * Numbers - for the first lesson don't make a distinction between int and float
          * [ ] Basic "Reading errors": understanding simple error messages
    3. **Notebook 3**
    4. **Notebook 4 - Prime Numbers**
        * This notebook will work up to calculating a list of prime numbers.  Along the way, it will introduce some basic problem solving techniques and explain new programming tools that we will need to solve the problem.
        * [ ] Introduce the problem of finding prime numbers.
        * [ ] Discuss the problem solving technique of specifying the problem, understanding it, and breaking it into smaller pieces.
        * [ ] Discussion - how would you break up this problem?  Use a click-to-reveal cell that shows how we will be solving the problem in this lesson.
        * [ ] Basic arithmetic (+, -, *, /) on Numbers (int or float) in Python
        * [ ] A closer look at divisibility - introducing the modulo operator (`%`).
        * [ ] Logic: How to determine if a single number is prime? (Algorithm: e.g., check for divisors from 2 up to number-1).
        * [ ] Python Tool: Introduction to Loops (e.g., `for` loops with `range()`).
        * [ ] Python Tool: Declaring Python Functions (`def`, parameters, `return`).
        * [ ] Building Block: The `is_prime(number)` function. (Implement the logic, using a loop to check divisors).
        * [ ] What is a list?
        * [ ] Putting It All Together: Generating a list of prime numbers. (Use a loop to iterate through a range, call `is_prime()`, and add primes to a list).
        * [ ] Reflecting on the problem solving process - an important step

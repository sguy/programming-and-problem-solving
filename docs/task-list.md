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
        * [ ] Create `notebooks/01-getting-started.ipynb`which covers the following:
          * [ ] Working with Jupyter notebooks
          * [ ] The Google Colab platform
          * [ ] What is programming? (Conceptual introduction)
          * [ ] Basic Markdown Syntax
          * [ ] How to run Python code cells
          * [ ] Introduction to "Tools for problem solving" (e.g., mental models, layers of abstraction) - brief overview
    2. **Notebook 2**
        * [ ] Create `notebooks/02-first-steps-with-python.ipynb`which covers the following:
          * [ ] Using the `print()` function for output
          * [ ] Variables
          * [ ] Introduction to Types
            * Strings (str)
            * Numbers - for the first lesson don't make a distinction between int and float
          * [ ] Basic "Reading errors": understanding simple error messages
    3. **Notebook 3 (or integrate into 1 & 2)**
        * [ ] Deeper dive into "Reading errors" and basic debugging strategies
        * [ ] Further exploration of "Tools for problem solving" with simple examples
        * [ ] Reinforce "What is programming?" with practical context

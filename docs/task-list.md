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

## Phase 3: Core Curriculum and Thematic Series

* **Goal:** Guide students from basic programming concepts to advanced, project-based applications.
* **Structure:** The curriculum is now organized into thematic series, with each number representing a major topic or project.

*   **Series 1-9: Python Fundamentals**
    *   [ ] **As-is:** Notebooks 1 through 9 will be preserved, covering the initial introduction to Python, calculations, functions, decisions, lists, and loops.

*   **Series 10: Dictionaries and F-Strings**
    *   [x] **New Notebook:** Create a new notebook `10-dictionaries.ipynb`.
    *   [x] **Content:** Use a fun, game-based example to teach dictionaries.
        *   [x] Introduce dictionaries by creating a `player` data structure to hold stats (`health`, `gold`, etc.).
        *   [x] Reinforce functions by creating "game engine" functions that operate on the player dictionary (e.g., `take_damage()`, `is_alive()`, `pickup_coin()`).
        *   [x] Introduce f-strings as a clean way to create a `display_status()` function.
        *   [x] Introduce nested dictionaries to handle more complex data like a player's inventory or a list of multiple players.

*   **Series 11.x: The Secrets of Encryption**
    *   [ ] **Refactor:** Combine and replace the old notebooks 10 and 11.
    *   [ ] **Content:** Create a narrative-driven series on cryptography.
    *   [ ] **Concepts:** Cover encoding vs. encryption, Caesar ciphers, integer factorization (introducing `tuples`), GCF/LCM (introducing `sets`), finding prime numbers, and an intuitive look at public-key crypto.

*   **Series 12.x: Exponential Growth and Financial Literacy**
    *   [ ] **New Series:** Create a new series focused on exponential growth.
    *   [ ] **Content:** Students will numerically discover `e` and `limits` through the lens of compound interest.
    *   [ ] **Concepts:** Introduce logarithms for solving "how long?" problems (e.g., doubling time), the Rule of 72, and other growth/decay models.
    *   [ ] **Library Intro:** This series will be the new home for introducing third-party libraries (`matplotlib`) and the associated concepts of `named` and `optional` arguments.

*   **Series 13.x: The Calculus of Derivatives**
    *   [ ] **Adapt:** This series will consist of the content from the *original* 12.x series.
    *   [ ] **Content:** Focus on the Method of Differences and finding numerical derivatives.
    *   [ ] **Refactor:** Remove the introduction to `matplotlib` and libraries, as that content has been moved to the new 12.x series.

*   **Series 14.x: Data Analysis with Pandas**
    *   [ ] **New Series:** Create a series on practical data analysis.
    *   [ ] **Content:** Introduce the Pandas library, `DataFrames`, reading data from files, and performing common operations like sorting, filtering, grouping, and basic statistics.

*   **Series 15.x: The Calculus of Integration**
    *   [ ] **New Series:** Create a companion series to the derivatives lessons.
    *   [ ] **Content:** Focus on numerical integration (Riemann sums) to find the area under a curve.

*   **Series 16.x: Introduction to Classes (Object-Oriented Programming)**
    *   [ ] **New Series:** Create a gentle introduction to classes and OOP.
    *   [ ] **Content:** Motivate the need for classes by modeling a practical system (e.g., a simple simulation) to show how classes bundle data and behavior.

*   **Series 17.x: Markov Chains and Language Models**
    *   [ ] **New Capstone Series:** Create a final project that demystifies the basic principles of LLMs.
    *   [ ] **Content:** Build a simple Markov chain from a text corpus.
    *   [ ] **Concepts:** Use this project to teach file I/O and advanced string manipulation.

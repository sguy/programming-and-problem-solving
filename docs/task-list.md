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

## Phase 3: Notebooks

* **Goal:** Write notebooks which will provide an introduction to the Jupyter notebook environment, the Python programming language, and problem solving techniques.
* **Note:** A notebook will only be added to the `table-of-contents.ipynb` after its corresponding "Publish to TOC" task has been manually checked off (`[x]`). This ensures only completed and reviewed notebooks are visible to students.
* **Tasks:**
    1. **Notebook 1 - Getting Started**
        * [x] Create `notebooks/01-getting-started.ipynb`which covers the following:
          * [x] Understanding Jupyter Notebooks and their cell-based structure (Markdown vs. Code cells).
          * [x] Navigating and using the Google Colab interface (e.g., adding/deleting cells, using the Table of Contents, saving to Google Drive, managing AI assistant settings).
          * [x] Writing, editing, and rendering basic Markdown (e.g., headings, lists).
          * [x] Running Python code cells and observing their output.
        * [x] Publish to TOC
    2. **Notebook 2 - First Steps with Python**
        * [x] Create `notebooks/02-first-steps-with-python.ipynb`which covers the following:
          * [x] What is programming? (Conceptual introduction)
          * [x] Comments
          * [x] Using the `print()` function for output
          * [x] Variables
          * [x] Introduction to Types
            * [x] Strings (str)
            * [x] Numbers - for the first lesson don't make a distinction between int and float
          * [x] Syntax Highlighting
          * [x] Basic "Reading errors": understanding simple error messages
        * [x] Publish to TOC
    3. **Notebook 3 - Shapes and Calculations**
        * [x] Create `notebooks/03-basic-calculations.ipynb` which covers:
            * [x] Introduction: Why calculate perimeter, area, volume?
            * [x] Basic Arithmetic in Python (`+`, `-`, `*`, `/`).
            * [x] Performing calculations with hardcoded values (e.g., `length = 5`, `area = length * width`).
            * [x] Highlight that `(` and `)` were used in the perimeter example to ensure that the `+` was applied before the `*`
        * [x] Publish to TOC
    4. **Notebook 4 - Interactive Programs**
        * [x] Create `notebooks/04-interactive-programs.ipynb` which covers:
            * [x] Introducing `input()` to get information from the user.
            * [x] Emphasizing string-to-number conversion (`int()`, `float()`).
        * [x] Publish to TOC
    5. **Notebook 5 - Reusable Code with Functions**
        * [x] Create `notebooks/05-reusable-code-with-functions.ipynb` which covers:
            * [x] Why use functions? (DRY principle).
            * [x] Defining functions with `def`, parameters, and `return`.
            * [x] Exploring different function patterns (e.g., with/without parameters, with/without return values).
            * [x] Case Study: Using function **composition** to solve a larger problem (surface area of a pyramid).
        * [x] Publish to TOC
    6. **Notebook 6 - Python's Decision Power**
        * [ ] Create `notebooks/06-decisions.ipynb` which covers:
            * [ ] Introduction: Making decisions.
            * [ ] Understanding Boolean values (`True`, `False`).
            * [ ] Using Comparison Operators (`==`, `!=`, `>`, `<`, `>=`, `<=`) to create Boolean expressions.
            * [ ] Conditional Statements: `if`, `else`, `elif`.
            * [ ] Mini-Challenge: e.g., "Movie Ticket Pricer" using conditionals.
        * [x] Publish to TOC
    7. **Notebook 7 - Organizing with Lists**
        * [ ] Create `notebooks/07-lists.ipynb` which covers:
            * [ ] Introduction to Lists for organizing information.
            * [ ] Creating empty lists and lists with initial items.
            * [ ] Adding items to a list using `.append()`.
            * [ ] Python Tool: New Syntax alert - calling methods on objects (`list.append()`).
            * [ ] Getting the length of a list using `len()`.
            * [ ] Mini-Challenge: e.g., "My Favorite Things" using lists.
        * [ ] Publish to TOC
    8. **Notebook 8 - Mastering Loops**
        * [x] Create `notebooks/08-for-loops.ipynb` which covers:
          * [x] Introduction to loops and the concept of iteration (DRY principle).
          * [x] Using `for` loops to iterate directly over items in a list.
          * [x] Using `for` loops with `range()` to repeat actions a specific number of times.
          * [x] Mini-Challenges: e.g., filtering a list, calculating statistics, and generating a multiplication table.
        * [ ] Publish to TOC
    9. **Notebook 9 - The Game Loop**
        * [ ] Create `notebooks/09-the-game-loop.ipynb` which covers:
          * [ ] Introduction to the "game loop" concept (e.g., initialize, loop, update, check for end).
          * [ ] Introducing `while` loops for indefinite repetition.
          * [ ] The concept of a "black box" function.
          * [ ] Using a provided `random_number()` function without needing to understand its internal workings.
          * [ ] Mini-Challenge 1: "Guess the Number" game (Hi/Low).
          * [ ] Mini-Challenge 2: "Random Math Test" game (e.g., 5 random addition problems).
        * [ ] Publish to TOC
    10. **Notebook 10 - Caesar Cipher**
        * [ ] Create `notebooks/10-the-caesar-cipher.ipynb` which covers:
          * [ ] Brief explanation of the Caesar Cipher and its history
          * [ ] Statement of problem - we want a system that lets two parties exchange secret messages
          * [ ] Let's Plan - how should we break up this problem?
          * [ ] Learning more about strings
            * [ ] string.upper()
            * [ ] Deeper dive into how strings are represented (do not get into the complexity of unicode)
              * [ ] Strings as sequences of characters
              * [ ] Special characters / ignoring characters that are not in A-Z
          * [ ] Encoding a character
            * [ ] Changing characters to ints with ord()
            * [ ] The modulo `%` operator - wrapping around fixed size lists.
            * [ ] Your turn to code: the `encode_char()` function.
          * [ ] Encoding a message
            * [ ] Using a for loop to iterate over a message.
            * [ ] Your turn to code: the `encode_message()` function
          * [ ] Decoding a message
            * [ ] Your turn to code: the `decode_char()` function
            * [ ] Stop and think: How are `encode_char()` and `decode_char()` different?
              * [ ] Can they share implementation? DRY
              * [ ] Tip: testing `a == decode_char(offset, encode_char(offset, a))`
            * [ ] Your turn to code: the `decode_message()` function
            * [ ] Stop and Think: is the relationship between `encode_message()` and `decode_message()` similar to the one between `encode_char()` and `decode_char()`?
              * [ ] Can we reuse code?
              * [ ] What about testing?
        * [ ] Publish to TOC
    11. **Notebook 11 - Prime Numbers**
        * [ ] Create `notebooks/11-prime-numbers.ipynb` which covers:
          * This notebook will work up to calculating a list of prime numbers.  Along the way, it will introduce some basic problem solving techniques and explain new programming tools that we will need to solve the problem.
          * [ ] Introduce the problem of finding prime numbers.
          * [ ] Discuss the problem solving technique of specifying the problem, understanding it, and breaking it into smaller pieces.
          * [ ] Discussion - how would you break up this problem?  Use a click-to-reveal cell that outlines how we will be solving the problem in this lesson.
          * [ ] Revise the modulo operator (`%`) - using it for divisibility instead of wrapping around a fixed size list.  How are these ideas related?
          * [ ] Your turn to code: The is_divisible function
          * [ ] Logic: How to determine if a single number is prime? (Algorithm: e.g., check for divisors from 2 up to number - 1).
          * [ ] Python Tool: Reminder of how to use Loops (e.g., `for` loops with `range()`).
          * [ ] Mini-challenge: print the multiples of 3 from 3 * 1 to 3 * 6.
          * [ ] Tip: Remember range goes from 0 to n-1 inclusive.
          * [ ] Building Block: The `is_prime(number)` function. (Implement the logic, using a loop to check divisors).
          * [ ] Revise lists.
          * [ ] Mini-challenge: make a list of multiples of 3 from 3 * 1 to 3 * 6.
          * [ ] Your turn to code: Putting It All Together: Generating a list of prime numbers. (Use a loop to iterate through a range, call `is_prime()`, and add primes to a list).
          * [ ] Reflecting on the problem solving process - an important step.  How do you think?  What clicks with you?  Meta-cognition.
        * [ ] Publish to TOC

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
    4. **Notebook 3 - Extended Practice**
        * [x] Create `notebooks/03-basic-calculations.extended-practice.ipynb` which covers:
          * [x] Advanced problem-solving with basic arithmetic.
          * [x] Multi-step problems requiring formula derivation (e.g., area of equilateral triangle).
          * [x] Complex word problems involving unit conversions and multiple geometric shapes (e.g., Juice Glass Mystery).
        * [x] Publish to TOC
    5. **Notebook 4 - Interactive Programs**
        * [x] Create `notebooks/04-interactive-programs.ipynb` which covers:
            * [x] Introducing `input()` to get information from the user.
            * [x] Emphasizing string-to-number conversion (`int()`, `float()`).
        * [x] Publish to TOC
    6. **Review Notebook (02-04)**
        * [x] Create `notebooks/02-04.review-notebook.ipynb` which covers:
          * [x] A concise list of topics from notebooks 02, 03, and 04.
          * [x] "Check Your Understanding" questions to reinforce concepts.
          * [x] "Mini-Challenge" problems combining skills.
          * [x] A brief discussion on problem-solving skills.
        * [x] Publish to TOC
    7. **Notebook 5 - Reusable Code with Functions**
        * [x] Create `notebooks/05-reusable-code-with-functions.ipynb` which covers:
            * [x] Why use functions? (DRY principle).
            * [x] Defining functions with `def`, parameters, and `return`.
            * [x] Exploring different function patterns (e.g., with/without parameters, with/without return values).
            * [x] Case Study: Using function **composition** to solve a larger problem (surface area of a pyramid).
            * [x] Parameters vs. Arguments.
            * [x] Functions in Python vs. Functions in Math.
            * [x] Combining Functions and User Input.
            * [x] Check Your Understanding: Parameters vs. Arguments.
            * [x] Discussion Question: Expanding Our Toolkit.
        * [x] Publish to TOC
    8. **Notebook 6 - Python's Decision Power**
        * [x] Create `notebooks/06-decisions.ipynb` which covers:
            * [x] Introduction: Making decisions.
            * [x] Understanding Boolean values (`True`, `False`).
            * [x] Using Comparison Operators (`==`, `!=`, `>`, `<`, `>=`, `<=`) to create Boolean expressions.
            * [x] Conditional Statements: `if`, `else`, `elif`.
            * [x] Mini-Challenge: e.g., "Movie Ticket Pricer" using conditionals.
            * [x] Code Structure and Indentation.
            * [x] Visualizing Decisions with Flowcharts.
            * [x] Extending the Movie Ticket Pricer - Discount Days.
            * [x] Refactoring - Improving Your Code's Design.
            * [x] Simplifying Movie Ticket Prices.
            * [x] Discussion Question: Real-world examples of decisions.
        * [x] Publish to TOC
    9. **Notebook 7 - Organizing with Lists**
        * [x] Create `notebooks/07-lists.ipynb` which covers:
            * [x] Introduction to Lists for organizing information.
            * [x] Creating empty lists and lists with initial items.
            * [x] Adding items to a list using `.append()`.
            * [x] Accessing items in a list using **indexing** (e.g., `my_list[0]`).
            * [x] Understanding the concept of a **method** as a function that belongs to an object.
            * [x] Getting the length of a list using `len()`.
            * [x] Mini-Challenge: Score Keeper.
            * [x] Mini-Challenge: Guest List.
            * [x] Mini-Challenge: Build a List from Scratch.
            * [x] Mini-Challenge: Simple Shopping Cart.
        * [ ] Publish to TOC
    10. **Notebook 8 - Mastering Loops**
        * [x] Create `notebooks/08-for-loops.ipynb` which covers:
          * [x] Introduction to loops and the concept of iteration (DRY principle).
          * [ ] Add a reminder about indented code blocks and where they have been seen before (functions, if/else statements).
          * [x] Using `for` loops to iterate directly over items in a list.
          * [x] Using `for` loops with `range()` to repeat actions a specific number of times.
          * [x] Mini-Challenge: Build Your Own `len()`.
          * [x] Mini-Challenge: Filter the Pets.
          * [x] Mini-Challenge: Simple Statistics.
          * [x] Mini-Challenge: Multiples.
          * [x] Mini-Challenge: Multiplication Table.
          * [x] The Perfect Trio - `len()`, `range()`, and Indexing.
        * [ ] Publish to TOC
    11. **Notebook 9 - The Game Loop**
        * [x] Create `notebooks/09-the-game-loop.ipynb` which covers:
          * [x] Introduction to the "game loop" concept (e.g., initialize, loop, update, check for end).
          * [x] Introducing `while` loops for indefinite repetition.
          * [x] The concept of a "black box" function.
          * [x] Using a provided `random_number()` function without needing to understand its internal workings.
          * [x] Mini-Challenge 1: "Guess the Number" game (Hi/Low).
          * [x] Mini-Challenge 2: "Random Math Test" game (e.g., 5 random addition problems).
        * [ ] Publish to TOC
    12. **Notebook 10 - Caesar Cipher**
        * [x] Create `notebooks/10-the-caesar-cipher.ipynb` which covers:
          * [x] Brief explanation of the Caesar Cipher and its history
          * [x] Statement of problem - we want a system that lets two parties exchange secret messages
          * [x] Let's Plan - how should we break up this problem?
          * [x] Learning more about strings
            * [x] string.upper()
            * [x] Deeper dive into how strings are represented (do not get into the complexity of unicode)
              * [x] Strings as sequences of characters
              * [x] Handling non-alphabetic characters
          * [x] Encoding a character
            * [x] Changing characters to ints with ord()
            * [x] The modulo `%` operator - wrapping around fixed size lists.
            * [x] Helper function: `is_uppercase(char)`
            * [x] Your turn to code: the `encode_char()` function.
          * [x] Encoding a message
            * [x] Using a for loop to iterate over a message.
            * [x] Your turn to code: the `encode_message()` function
          * [x] Decoding a message
            * [x] Your turn to code: the `decode_char()` function
            * [x] Stop and think: How are `encode_char()` and `decode_char()` different?
              * [x] Can they share implementation? DRY
              * [x] Tip: testing `a == decode_char(offset, encode_char(offset, a))`
            * [x] Your turn to code: the `decode_message()` function
            * [x] Stop and Think: is the relationship between `encode_message()` and `decode_message()` similar to the one between `encode_char()` and `decode_char()`?
              * [x] Can we reuse code?
              * [x] What about testing?
        * [ ] Publish to TOC
    13. **Notebook 11 - Prime Numbers**
        * [x] Create `notebooks/11-prime-numbers.ipynb` which covers:
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

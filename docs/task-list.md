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
    *   [ ] **Refactor:** The 11.x series will be restructured into a 5-part narrative on cryptography, building concepts from the ground up.
    *   [ ] **Goal:** To introduce core cryptographic concepts, show their real-world relevance, and practice Python skills like string manipulation, modular arithmetic, and working with tuples.

    *   [ ] **Notebook 11.a: An Introduction to Secret Messages**
        *   **Concepts:** Introduce foundational vocabulary.
            *   **Encoding vs. Encrypting:** Frame encoding as enhancing a message for a public purpose (e.g., compression like JPEG/ZIP, error resilience) and encrypting as hiding a message's content for a private purpose.
            *   **Plaintext & Ciphertext.**
        *   **Mini-Challenge: The ASCII Codec:** Implement `encode` and `decode` functions using `ord()` and `chr()` to give a hands-on example of a public, reversible transformation.
        *   **Visuals:** Add a diagram illustrating the difference between an encoding/decoding process and an encryption/decryption process.

    *   [ ] **Notebook 11.b: The Caesar Cipher**
        *   **Concepts:** Implement a simple symmetric encryption algorithm, reinforcing the new vocabulary.
        *   **Mini-Challenge: The Encryption Pipeline:**
            *   **1. The Codec:** Write `letter_to_number` and `number_to_letter` functions (the encoding/decoding step).
            *   **2. The Cipher:** Write `shift_number` and `unshift_number` functions that operate only on numbers (the encrypting/decrypting step).
            *   **3. The Pipeline:** Combine the helper functions into `encrypt_message` and `decrypt_message` functions to process full strings.
        *   **Visuals:** Add a diagram showing the full pipeline: `Letter -> Encode -> Number -> Encrypt -> Shifted Number`.

    *   [ ] **Notebook 11.c: The Key Exchange Problem & One-Way Functions**
        *   **Concepts:** Introduce the problem of sharing keys secretly and the concept of a one-way function as a solution. Introduce Python `tuples` as a way to store structured data.
        *   **Mini-Challenge: Advanced Prime Factorization:** Write a function `get_prime_factorization(n)` that returns a list of `(prime, count)` tuples (e.g., `12` -> `[(2, 2), (3, 1)]`). This provides a strong motivation for using tuples.

    *   [x] **Notebook 11.d (Optional): Practice with Factoring**
        *   **Concepts:** Provide optional, deeper practice with number theory problems.
        *   **Mini-Challenge 1: The Age Puzzle:** "Alice's age is between 30-40, Bob's is 40-50. The product of their ages is a perfect cube. Find their ages." Guide students to use prime factorization to solve this, reinforcing the concepts from 11.c.
        *   **Mini-Challenge 2: Greatest Common Factor (GCF):** Write a `gcf(a, b)` function that uses the `(prime, count)` tuple data from the previous notebook, reinforcing the utility of the data structure.

    *   [ ] **Notebook 11.e: Public-Key Cryptography in the Real World**
        *   **Concepts:** Explain how a key exchange works conceptually and connect it to real-world applications like HTTPS.
        *   **The Analogy (Conversational Paint Mixing):** Present the paint mixing analogy in a step-by-step conversational format between Alice and Bob, clarifying what the eavesdropper Eve can see vs. what remains private.
        *   **Closing the Loop:** Conclude the analogy by explaining that the final shared secret "paint" is used as the key for a faster symmetric cipher to encrypt the actual messages.
        *   **Mini-Challenge: The Clockwork Modulo:** Give students a hands-on taste of the real math by having them calculate `public_value = (base ** secret) % modulus` with small numbers, demystifying the "transformation" step of the analogy.

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

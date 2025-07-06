# Gemini Agent Instructions for "Programming and Problem Solving"

This document provides guidelines for the Gemini agent when working on this project.

## 1. Project Mission and Core Principles

- **Primary Goal:** To create high-quality, beginner-friendly educational materials for learning Python and problem-solving using Jupyter Notebooks.
- **Target Audience:** Beginners with little to no programming experience. All content, especially code examples and explanations, must be simple, clear, and easy to understand.
- **Pedagogical Style:** The tone should be encouraging, supportive, and educational. Use analogies and simple explanations. Avoid complex jargon or overly "clever" code. Refer to the existing notebooks to match this style.
- **Convention Adherence:** Strictly follow the existing coding style, formatting, and project structure.

## 2. Technical Guidelines

- **Linting and Formatting:** Before committing any code changes, always run the following commands from the project root to ensure code quality and consistency:
    - `ruff check . --fix`
    - `black .`
- **Dependencies:** The project uses a `venv` for its environment and manages dependencies via `pyproject.toml`.
- **Testing:** While most work is in notebooks, any changes to Python source code in `src/` should be accompanied by tests in the `tests/` directory. Run tests with `pytest`.
- **Git Commits:** Follow the style of existing commit messages. They are typically concise and written in the imperative mood (e.g., "Fix layout for flowcharts," "Add notebook on decisions").

## 3. Workflow for Modifying Notebooks

- **Understand the Task:** Before creating or modifying a notebook, consult the `docs/task-list.md` file to understand the specific requirements, learning objectives, and scope for that notebook.
- **Match Existing Style:** Read through several existing notebooks (e.g., `notebooks/01-getting-started.ipynb`, `notebooks/02-first-steps-with-python.ipynb`) to internalize the structure, tone, and style. Pay special attention to `notebooks/03-basic-calculations.ipynb` to see how SVG diagrams are used to illustrate concepts. For detailed rules on notebook formatting, refer to `docs/styleguide-ipynb.md`.
- **Cell-Based Structure:** Remember that notebooks are a mix of Markdown cells for explanation and Python code cells for examples. Balance these appropriately.
- **Table of Contents (`TOC`):** **CRITICAL:** A notebook is only added to `table-of-contents.ipynb` after its corresponding "Publish to TOC" task has been manually checked off (`[x]`) in `docs/task-list.md`. **Do not add a notebook to the TOC unless explicitly instructed to do so.** This ensures only completed and reviewed notebooks are visible to students.

## 4. Generating Explanatory Diagrams

- **Purpose:** Whenever a concept or problem can be clarified with a visual aid, generate a simple, clean SVG diagram.
- **Location:** Store all generated diagrams in the `notebooks/images/` directory.
- **Style:** Diagrams should be clear, uncluttered, and consistent with the visual style of existing diagrams in the project. Use them to illustrate problems (e.g., `picture-frame-problem.svg`) or visualize concepts (e.g., `flowchart_if_else_simple.svg`).
- **Implementation:** When adding a diagram to a notebook, use a Markdown image tag with a fully qualified URL pointing to the raw GitHub content. Refer to `docs/styleguide-ipynb.md` for the exact URL format.

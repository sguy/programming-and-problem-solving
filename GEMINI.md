# Gemini Agent Instructions for "Programming and Problem Solving"

This document provides guidelines for the Gemini agent when working on this project.

## 1. Project Mission and Core Principles

- **Project Requirements:** Refer to `docs/PRD.md` for a detailed overview of project goals, target audience, core features, and technical requirements.
- **Primary Goal:** To create high-quality, beginner-friendly educational materials for learning Python and problem-solving using Jupyter Notebooks.
- **Target Audience:** Beginners with little to no programming experience. All content, especially code examples and explanations, must be simple, clear, and easy to understand.
- **Pedagogical Style:** The tone should be encouraging, supportive, and educational. Use analogies and simple explanations. Avoid complex jargon or overly "clever" code. Refer to the existing notebooks to match this style.
- **Convention Adherence:** Strictly follow the existing coding style, formatting, and project structure.

## 2. Technical Guidelines

- **Code Quality:** Adhere to the project's code style and linting rules as defined in `docs/styleguide-python.md`.
- **Dependencies:** The project uses a `venv` for its environment and manages dependencies via `pyproject.toml`.
- **Testing:** For Python source code in `src/`, ensure changes are accompanied by tests. Refer to `docs/styleguide-python.md` for testing guidelines.
- **Git Commits:** Follow the style of existing commit messages (concise, imperative mood, e.g., "Fix layout for flowcharts," "Add notebook on decisions").

## 3. Workflow for Modifying Notebooks

- **Understand the Task:** Before creating or modifying a notebook, consult the `docs/task-list.md` file to understand the specific requirements, learning objectives, and scope for that notebook.
- **Adhere to Style:** For detailed rules on notebook formatting, tone, and structure, refer to `docs/styleguide-ipynb.md`.
- **Table of Contents (`TOC`):** **CRITICAL:** Only notebooks with their corresponding "Publish to TOC" task manually checked off (`[x]`) in `docs/task-list.md` are to be included in `table-of-contents.ipynb`. **Do not add a notebook to the TOC unless explicitly instructed to do so.** This ensures only completed and reviewed notebooks are visible to students.

## 4. Editing Jupyter Notebooks (`.ipynb` files)

When modifying Jupyter Notebooks, it is crucial to understand their underlying JSON structure to avoid corruption. Notebooks are composed of a list of "cells," each with a `cell_type` (e.g., "markdown" or "code") and a `source` field. The `source` field is an array of strings, where each string represents a line of content within that cell.  Cells are uniquely labeled with the 'id' field.

**Strategy for Editing:**
1.  **Read the entire notebook file** and parse its JSON content into a dictionary.
2.  **Identify the specific cell** that needs to be modified (e.g., by its `id` field).
3.  **Modify the cell's content in memory:**
    *   Access the `source` field of the target cell. This will be a JSON array of strings.
    *   Join the `source` array into a single string (e.g., `source_text = "".join(cell["source"])`).
    *   Perform the desired text modifications on `source_text`.
    *   Split the modified `source_text` back into an array of strings, ensuring each line ends with `\n` (e.g., `new_source_array = [line + "\n" for line in modified_source_text.splitlines()]`).
    *   Update the cell's `source` field with `new_source_array`.
4.  **Generate JSON strings for replacement:**
    *   Convert the *original* cell dictionary (before modification) into a perfectly formatted JSON string.
    *   Convert the *modified* cell dictionary into a perfectly formatted JSON string.
5.  **Use the `replace` tool:** Use the JSON string of the original cell as the `old_string` and the JSON string of the modified cell as the `new_string`. This ensures the change is precise and maintains the integrity of the notebook's JSON structure.

This cell-by-cell approach ensures that changes are localized, easier to debug, and result in cleaner `git diff` outputs.

## 5. Generating Explanatory Diagrams

- **Purpose:** Whenever a concept or problem can be clarified with a visual aid, generate a simple, clean SVG diagram.
- **Location:** Store all generated diagrams in the `notebooks/images/` directory.
- **Style:** Diagrams should be clear, uncluttered, and consistent with the visual style of existing diagrams in the project. Use them to illustrate problems (e.g., `picture-frame-problem.svg`) or visualize concepts (e.g., `flowchart_if_else_simple.svg`).
- **Implementation:** When adding a diagram to a notebook, use a Markdown image tag with a fully qualified URL pointing to the raw GitHub content. Refer to `docs/styleguide-ipynb.md` for the exact URL format.

## 6. Reviewing Notebooks

- **Activity:** When asked to "Review Lesson X" (where X is a number), open the corresponding notebook (e.g., "Review Lesson 4" means `notebooks/04-interactive-programs.ipynb`).
- **Rubric:** Ensure the notebook is in full compliance with the style guide defined in `docs/styleguide-ipynb.md`.
- **Focus Areas:** Pay special attention to the narrative flow, tone, quality of challenges, and appropriate cognitive load.
- **Feedback Format:** Initially, provide a human-readable summary of the notebook's evaluation (similar to a code review), followed by a numbered plan of steps to improve the notebook. Each step in the plan should then be addressed as a series of small, self-contained changes.
- **Collaboration:** Before making each change, ask for approval and allow for additional feedback to work collaboratively.

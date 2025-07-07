# Project Requirements Document: Programming and Problem Solving (PAPS)

## 1. Introduction

This document outlines the project goals, target audience, core features, technical requirements, and pedagogical approach for the Programming and Problem Solving (PAPS) project. It serves as a guiding document for all contributors, including AI agents, to ensure consistency and alignment with the project's vision.

## 2. Project Goals

The PAPS project aims to provide a comprehensive set of self-study Jupyter notebooks for students aged 13-16, serving as a complete introduction to programming and problem-solving.

*   **Primary Goal:** To create high-quality, beginner-friendly educational materials for learning Python and problem-solving using Jupyter Notebooks.
*   **Key Objectives:**
    *   Assume no prior exposure to programming.
    *   Assume students will run notebooks on Google Colab (zero-installation platform).
    *   Present programming as a versatile tool applicable across many disciplines (mathematics, finance, science, language arts).
    *   Each notebook should take approximately 30-60 minutes for a student to work through.
    *   Each notebook should provide many opportunities for student experimentation.

## 3. Target Audience

*   **Primary Learners:** Students between 13-16 years old with little to no prior programming experience.
*   **Assumed Prior Knowledge:** None in programming. Basic computer literacy.
*   **Learning Styles:** The materials should cater to interactive learning, with a balance of theoretical explanation and practical application.

## 4. Core Features / Content Areas (Project Deliverables)

The project will deliver a set of Jupyter notebooks covering fundamental programming and problem-solving concepts. For a detailed breakdown of the content for each notebook, refer to the [PAPS Project Plan & Task List](task-list.md).

*   **Initial Notebooks:** Focus on introducing Jupyter Notebooks, Google Colab, basic Markdown, and Python fundamentals (variables, types, `print()`, error handling).
*   **Additional Notebooks (Extended Case Studies):** Introduce new Python concepts and problem-solving techniques through engaging challenges, including functions, data structures (tuples, lists, dictionaries, classes), and open-ended discussion questions.

## 5. Technical Requirements

*   **Platform:** Jupyter Notebooks, primarily run on Google Colaboratory (Colab). All descriptions of the Jupyter notebook interface should refer to what Google Colab presents.
*   **Primary Language:** Python.
*   **Code Style/Linting:** Adherence to project conventions, enforced by `ruff` and `black`.
*   **Dependency Management:** Managed via `pyproject.toml` within a `venv`.
*   **Testing:** `pytest` for any Python source code in the `src/` directory.
*   **Version Control:** Git/GitHub.

## 6. Pedagogical Approach & Style Guidelines

*   **Tone:** Encouraging, supportive, and educational.
*   **Explanation Style:** Simple, clear, and easy to understand. Use analogies. Avoid complex jargon or overly "clever" code.
*   **Notebook Structure:** A balanced mix of Markdown cells for explanation and Python code cells for examples and exercises.
*   **Diagrams:** Simple, clean SVG diagrams stored in `notebooks/images/` to clarify concepts. Referenced using fully qualified GitHub raw content URLs.
*   **Interactive Elements:** Mini-challenges, discussion questions, and opportunities for experimentation.
*   **Comments:** Add comments sparingly, focusing on *why* something is done.
*   **Convention Adherence:** Strictly follow existing coding style, formatting, and project structure.

## 7. Success Metrics

Success will be measured by:
*   The completeness of the planned set of Jupyter notebooks.
*   Adherence to the defined pedagogical and technical standards.
*   Feedback from target audience (e.g., clarity, engagement, effectiveness in teaching).

## 8. Future Considerations / Out of Scope

*   **Out of Scope for Initial Phase:** Deployment to platforms other than Google Colab, advanced topics beyond the scope of introductory programming for the target age group.
*   **Potential Future Expansions:** Additional case studies, integration with other learning platforms, advanced topics for older students.

## 9. Research Background / References

Research these books for background information. These are only pointers, **check for copyright status before using**.

* [The Coder's Apprentice: Learning Programming with Python 3 (Version 1.1)](https://annas-archive.org/md5/8212681b58208f9d05dfc99192901350)
* [Zero to Py : A Comprehensive Guide to Learning the Python Programming Language](https://annas-archive.org/md5/944741a690c5cfa1e67ba614981767ec)
* [Make Your Own Python Text Adventure : A Guide to Learning Programming](https://annas-archive.org/md5/334655ad8f40397710bf1394c947cd6e)
* [Cognitive Models and Intelligent Environments for Learning Programming (Nato ASI Subseries F:, 111)](https://annas-archive.org/md5/f3089258ecac737d96ed51f4151c79f0)
* [Seven Languages in Seven Weeks: A Pragmatic Guide to Learning Programming Languages (Pragmatic Programmers)](https://annas-archive.org/md5/273f1bdd83328f3dc08de8b767ec)
* [Python: Introduction To Python Programming: Beginner's Guide To Computer Programming And Machine Learning (Python Programming, Machine Learning, Programming for Beginners)](https://annas-archive.org/md5/34994d824c4a5143016649a3cff7b963)
* [Learning Algorithms Through Programming and Puzzle Solving.](https://annas-archive.org/md5/ccf5c7cc60b885fecb510b84f52adcfb)

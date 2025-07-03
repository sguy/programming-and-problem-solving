# iPython Notebook Style Guide

This document outlines the best practices and conventions for creating iPython notebooks for this project. Adhering to this guide will ensure consistency, clarity, and an optimal learning experience for our target audience.

**Note for Gemini Code Assist:** This file (`./gemini/styleguide-ipynb.md`) should be automatically included in the context when working on iPython notebooks within this project.

## 1. Target Audience

* **Level:** Late middle school / early high school students.
* **Prior Experience:** Assumed to have no prior programming experience.
* **Language:** Use clear, concise, and age-appropriate language. Avoid jargon where possible, or explain it thoroughly if necessary.
* **Engagement:** Content should be engaging, relatable, and encouraging.

## 2. Platform

* **Environment:** All notebooks will be developed for and hosted exclusively on **Google Colab**.
* **Colab Features:** Leverage Colab-specific features where beneficial (e.g., easy sharing, integration with Google Drive).
* **Compatibility:** Ensure all code and markdown renders correctly in Colab.

## 3. Notebook Structure & Content

* **Estimated Time:** Each notebook should be designed to be completed in approximately **30-60 minutes**.

  * Clearly state the estimated time at the beginning of the notebook.
* **Beginning of Notebook:**
  * **Title:** Clear and descriptive title.
  * **Summary/Introduction:** A brief overview of what the notebook covers and what the student will learn.
  * **Inspirational Quote:** Include a humorous or insightful quote from a scientist, mathematician, computer scientist, or historical figure that is relevant to the notebook's topic. This helps set the tone and provides context.
  * **Learning Objectives:** 2-3 bullet points outlining specific skills or knowledge students will gain.
  * **Prerequisites/Review:** A quick review of essential concepts from previous notebooks that will be used in the current one. Link back to relevant sections if possible.
    * When linking to another notebook in this series, use the full Google Colab GitHub link format, for example: `Notebook 3: Shapes and Calculations`.
* **End of Notebook:**
  * **Summary/Recap:** A concise summary of the key concepts covered in the notebook.
  * **Discussion Question (Meta-cognition):** Before the final summary, include an open-ended discussion question (`### 🤔 Discussion Question:`) to encourage students to reflect on their learning process. For example: "Think back on the challenges in this notebook. Which concepts 'clicked' for you right away? Which ones were a bit tricky? What strategies did you use when you got stuck?"
  * **Key Takeaways:** Bullet points highlighting the most important points.
  * **Next Steps/Preview:** Briefly mention what will be covered in the next notebook or suggest further exploration.
* **Interactivity & Engagement:**
  * **Minimum 1/3 Interactive Cells:** At least one-third of the cells in each notebook should be dedicated to interactive experimentation or mini-challenges.
  * **Code Cells:** Encourage students to run, modify, and experiment with code. Provide clear instructions and expected outputs.
  * **Markdown Cells:** Use markdown cells for explanations, instructions, and questions.

## 4. Section Icons and Decoration

Use consistent visual cues (e.g., emojis or icons) to denote different types of information. This helps students quickly identify the purpose of a section. **To ensure these sections appear in the notebook's table of contents, they should be formatted as markdown headers (e.g., `##` or `###`). As a general guideline, use `##` for major new topics and `###` for sub-topics, tips, and challenges.**

* `### 💡 Tip:` For helpful hints, shortcuts, or best practices.
  * _Example: "`### 💡 Tip:` You can use `Ctrl+Enter` (or `Cmd+Enter` on Mac) to run a code cell in Colab!"_
* `### 🎯 Mini-Challenge:` For small, focused coding exercises or tasks. Mini-challenges should follow a consistent structure to guide the student effectively, as seen in `03-basic-calculations.ipynb`.
  * To guide the student effectively, mini-challenges should follow a consistent **sequence of cells** without explicit numbering or labels like "Prompt" or "Solution".
    1. The challenge begins with a markdown cell containing the `### 🎯 Mini-Challenge:` heading and the problem description.
    2. This is followed by an optional markdown cell containing one or more collapsible `<details>` blocks for hints.
    3. Next is the student's code cell, pre-populated with starter code and a `# YOUR CODE HERE` placeholder.
    4. Finally, a markdown cell provides the solution within a collapsible `<details>` block (e.g., `<summary>Click to see a possible solution</summary>`).
* `### 🚀 Pro-Tip:` For more advanced tips or insights for curious students.
  * _Example: "`### 🚀 Pro-Tip:` Python also supports f-strings for even more flexible string formatting. We'll explore those later!"_
* `## 🐍 New Concept:` When introducing a new Python command, programming concept, or key vocabulary.
  * _Example: "`## 🐍 New Concept:` Variables - Variables are like containers that store information."_
* `### ⚠️ Heads Up!:` For important distinctions, common pitfalls, or things students need to be particularly careful about.
  * _Example: "`### ⚠️ Heads Up!:` Python is case-sensitive, meaning `myVariable` and `myvariable` are different."_
* `### 🤔 Discussion Question:` To prompt thought and reflection. These can be open-ended.
  * _Example: "`### 🤔 Discussion Question:` Can you think of other situations where using a loop would be helpful?"_
* `### 🔗 External Resources:` For links to relevant external websites, videos, or articles.
  * _Example: "`### 🔗 External Resources:` For more about Python lists, check out the official Python documentation [link]."_
* `### 📚 Learning More / Dig Deeper:` To suggest further exploration or optional advanced topics.
  * _Example: "`### 📚 Learning More:` If you're interested in game development with Python, you might want to explore the Pygame library."_
* `### ✅ Check Your Understanding:` For quick comprehension questions (e.g., multiple choice, fill-in-the-blank within a markdown cell).
  * _Example of a multiple-choice question:_

        ```markdown
        ### ✅ Check Your Understanding:
        Which of the following is a Python keyword used to define a variable that stores a whole number?
        a) `string`
        b) `float`
        c) `int`
        d) `define`

        <!-- Answer: c) int -->
        ```

  * _Example with a revealable answer (useful in Colab):_

        ```markdown
        ### ✅ Check Your Understanding:
        What would `print(5 + 3)` display?

        <details>
          <summary>Click to see the answer</summary>

          `8`
        </details>
        ```

* `## 🎉 Milestone / Well Done!:` To acknowledge progress and provide encouragement after completing a significant section or challenge.

**Usage:**

* Place the icon and bolded title at the beginning of the relevant markdown cell or section.
* Be consistent with the chosen icons.

## 5. Code Cells

* **Clarity:** Code should be well-commented, especially when introducing new concepts.
* **Simplicity:** Use the simplest effective code to demonstrate concepts. Avoid overly complex or obscure syntax.
* **Step-by-Step:** Break down complex operations into smaller, manageable code cells.
* **Output:** Ensure code cells produce clear and understandable output. If an error is expected as part of a lesson, explain it.
* **Placeholders:** Use clear placeholders like `# YOUR CODE HERE` or `# TODO: ...` for student exercises.
* **Code conventions and formatting** should follow guidelines set up in `./styleguide.md`

## 6. Markdown Cells

* **Formatting:** Use markdown formatting (headings, bold, italics, lists, etc.) to structure content and improve readability.
* **Images/GIFs:** Use relevant images or GIFs to illustrate concepts or make the notebook more engaging, but ensure they are optimized for web and do not significantly increase loading times.
* **Image Linking:** All images stored in the repository must be linked using the full GitHub raw content URL to ensure they render correctly on all platforms (e.g., nbviewer, GitHub).
  * The URL must point to the `refs/heads/main` branch and include the full path from the repository root (e.g., `notebooks/images/your-image.png`).
  * _Example:_ `![A diagram showing a single variable box labeled](https://raw.githubusercontent.com/sguy/programming-and-problem-solving/refs/heads/main/notebooks/images/variable_vs_list.svg)`
* **Mathematical Formulas:** Use LaTeX for all mathematical formulas to visually distinguish them from Python code. This ensures they are rendered clearly and professionally.
  * _Example:_ `$$Area = \frac{base \times height}{2}$$` instead of `Area = (base * height) / 2`.
* **Conciseness:** Keep explanations clear and to the point.

## 7. General Best Practices

* **Test Thoroughly:** Run through the entire notebook as a student would to catch errors, typos, or confusing instructions.
* **Save Regularly:** Encourage students to save their work (though Colab autosaves).
* **Iterative Improvement:** Be open to feedback and iterate on notebook content to improve the learning experience.

---
This style guide is a living document and may be updated as the project evolves.
      *The solution should print intermediate results where helpful.
      * Each `print()` statement in the solution should be followed by a comment showing the expected output. For `input()`, it should show a sample interaction.
      * _Example:_
      ```python
      # Solution code for a print statement
      print("The area is:", area)
      # Expected output: The area is: 50

      # Solution code for an input statement
      user_name = input("What is your name? ") # Sample interaction: What is your name? Ada
      ```

* 🚀 **Pro-Tip:** For more advanced tips or insights for curious students.
  * _Example: "🚀 **Pro-Tip:** Python also supports f-strings for even more flexible string formatting. We'll explore those later!"_
* 🐍 **Python / New Concept:** When introducing a new Python command, programming concept, or key vocabulary.
  * _Example: "🐍 **New Concept: Variables** - Variables are like containers that store information."_
* ⚠️ **Heads Up!:** For important distinctions, common pitfalls, or things students need to be particularly careful about.
  * _Example: "⚠️ **Heads Up!** Python is case-sensitive, meaning `myVariable` and `myvariable` are different."_
* 🤔 **Discussion Question:** To prompt thought and reflection. These can be open-ended.
  * _Example: "🤔 **Discussion Question:** Can you think of other situations where using a loop would be helpful?"_
* 🔗 **External Resources:** For links to relevant external websites, videos, or articles.
  * _Example: "🔗 **External Resource:** For more about Python lists, check out the official Python documentation [link]."_
* 📚 **Learning More / Dig Deeper:** To suggest further exploration or optional advanced topics.
  * _Example: "📚 **Learning More:** If you're interested in game development with Python, you might want to explore the Pygame library."_
* ✅ **Check Your Understanding:** For quick comprehension questions (e.g., multiple choice, fill-in-the-blank within a markdown cell).
  * _Example of a multiple-choice question:_

        ```markdown
        ✅ **Check Your Understanding:**
        Which of the following is a Python keyword used to define a variable that stores a whole number?
        a) `string`
        b) `float`
        c) `int`
        d) `define`

        <!-- Answer: c) int -->
        ```

  * _Example with a revealable answer (useful in Colab):_

        ```markdown
        ✅ **Check Your Understanding:**
        What would `print(5 + 3)` display?

        <details>
          <summary>Click to see the answer</summary>

          `8`
        </details>
        ```

* 🎉 **Milestone / Well Done!:** To acknowledge progress and provide encouragement after completing a significant section or challenge.

**Usage:**

* Place the icon and bolded title at the beginning of the relevant markdown cell or section.
* Be consistent with the chosen icons.

## 5. Code Cells

* **Clarity:** Code should be well-commented, especially when introducing new concepts.
* **Simplicity:** Use the simplest effective code to demonstrate concepts. Avoid overly complex or obscure syntax.
* **Step-by-Step:** Break down complex operations into smaller, manageable code cells.
* **Output:** Ensure code cells produce clear and understandable output. If an error is expected as part of a lesson, explain it.
* **Placeholders:** Use clear placeholders like `# YOUR CODE HERE` or `# TODO: ...` for student exercises.
* **Code conventions and formatting** should follow guidelines set up in `./styleguide.md`

## 6. Markdown Cells

* **Formatting:** Use markdown formatting (headings, bold, italics, lists, etc.) to structure content and improve readability.
* **Images/GIFs:** Use relevant images or GIFs to illustrate concepts or make the notebook more engaging, but ensure they are optimized for web and do not significantly increase loading times.
* **Image Linking:** All images stored in the repository must be linked using the full GitHub raw content URL to ensure they render correctly on all platforms (e.g., nbviewer, GitHub).
  * The URL must point to the `refs/heads/main` branch and include the full path from the repository root (e.g., `notebooks/images/your-image.png`).
  * _Example:_ `!A descriptive caption for the image`
* **Mathematical Formulas:** Use LaTeX for all mathematical formulas to visually distinguish them from Python code. This ensures they are rendered clearly and professionally.
  * _Example:_ `$$Area = \frac{base \times height}{2}$$` instead of `Area = (base * height) / 2`.
* **Conciseness:** Keep explanations clear and to the point.

## 7. General Best Practices

* **Test Thoroughly:** Run through the entire notebook as a student would to catch errors, typos, or confusing instructions.
* **Save Regularly:** Encourage students to save their work (though Colab autosaves).
* **Iterative Improvement:** Be open to feedback and iterate on notebook content to improve the learning experience.
* **Meaningful Cell IDs:** Assign meaningful, human-readable IDs to each cell in the notebook's JSON source (e.g., `id: "case-study-intro"`). This practice makes version control diffs more informative and the raw notebook file easier to navigate.

---
This style guide is a living document and may be updated as the project evolves.

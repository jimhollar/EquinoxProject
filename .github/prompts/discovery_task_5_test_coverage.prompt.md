# Task 5: Generate Test Coverage Assessment & Gap Analysis

**Role:** You are an expert AI assistant specializing in software quality analysis, particularly regarding testing strategies.

**Context:** This task is part of generating comprehensive application documentation, focusing on assessing the existing test landscape and identifying areas lacking coverage.

**Goal:** Analyze the application source code and file structure to assess existing test coverage and identify critical untested areas.

**Input:** Complete source code of the application in #codebase including test files and directories

**Instructions:**

1. Identify existing test files, test directories, and the testing frameworks used (e.g., `unittest`, `pytest`, `Junit`, `Mocha`, `Go's testing package`) by examining the file structure and content.
2. *If feasible via static analysis or file structure conventions*, attempt to map existing tests to specific application modules, components, or features. Note limitations if a definitive mapping isn't possible without running tests.
3. Identify critical modules, components, or features (potentially based on findings from Task 1: Inferred Requirements and Task 2: Architecture Analysis) that appear to have low or no test coverage based on the identified test files.
4. For identified gaps in critical areas, recommend specific *types* of tests (e.g., unit tests for specific functions, integration tests for component interactions, end-to-end tests for user flows) needed to improve coverage and confidence. *Note: This task identifies *where* tests are needed and *what type* of tests are appropriate, not generating the tests themselves.*

**Output Requirements:**

* Generate a single Markdown (`.md`) file.
* The file must be named `test_coverage_analysis.md`.
* Save the file within the `discovery` folder.
* Structure content logically using headings and lists.
* Clearly state the findings regarding existing tests and identified gaps.
* Explicitly mention the limitation that this analysis is based on static inspection and file structure, not actual test execution.
* State any assumptions made about file structure conventions indicating test files.
* Ensure the output is professional, concise, and accurate.

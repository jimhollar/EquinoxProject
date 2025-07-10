# Task 2: Generate Test Coverage Assessment & Gap Analysis

**Role:** You are an expert AI assistant specializing in software quality analysis, particularly regarding testing strategies and test creation.

**Context:** This task is part of enabling application modernization, focusing on assessing the existing test landscape and identifying areas lacking coverage and creating a comprehensive backlog of needed tests and plan for adding them.

**Goal:** Analyze the application source code and file structure to assess existing test coverage and identify critical untested areas and create a plan to remediate those discoveries by adding specific tests that will be created by the next task.

**Input:** Complete source code of the application in #codebase including test files and directories

**Instructions:**

1. Identify existing test files, test directories, and the testing frameworks used (e.g., `xunit``unittest`, `pytest`, `Junit`, `Mocha`, `Go's testing package`) by examining the file structure and content.
2. *If feasible via static analysis or file structure conventions*, attempt to map existing tests to specific application modules, components, or features. Note limitations if a definitive mapping isn't possible without running tests.
3. Identify critical modules, components, or features (potentially based on findings from Task 1: Inferred Requirements and Task 2: Architecture Analysis) that appear to have low or no test coverage based on the identified test files.
4. For identified gaps in critical areas, create a comprehensive backlog of tests of each type (e.g., unit tests for specific functions, integration tests for component interactions, end-to-end tests for user flows) needed to improve coverage.

**Output Requirements:**

* Generate a single Markdown (`.md`) file named `test_coverage_analysis.md`.
* Save the file within the `discovery` folder.
* Include a summary of existing tests, their locations, and the frameworks used.
* Clearly state any identified gaps in test coverage, particularly for critical modules or features.
* Provide a detailed backlog of tests needed, categorized by type (unit, integration, end-to-end) and mapped to specific application components or features.
* Document any assumptions made about file structure conventions indicating test files, such as naming conventions or directory structures.
* Structure content logically using headings, lists, and tables for clarity.
* Ensure the output is professional, concise, and accurate.

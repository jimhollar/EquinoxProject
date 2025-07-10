# Application Discovery Documentation Generation Process Status

This document outlines the steps required to generate comprehensive documentation for the application source code within the codebase.

The process is broken down into sequential tasks. To execute the full documentation generation, start from the first incomplete task below.

## Automatically perform the following actions

- *Create the `discovery` and `discovery/diagrams` folders before running `discoveryTracker.md`*
- *create `discoveryTracker.md` in the `discovery` folder using the template provided below.*
- *run the prompt in `discoveryTracker.md` and complete all the tasks specidifed in the prompt

## Template for `discoveryTracker.md`

**Instructions:**

1. Ensure you have access to the application source code at the specified path.
2. Do not change any existing application code, or run any tasks that may have been defined inthe applocation source code.
3. Run the prompt corresponding to the first task that is marked with `[ ]` (incomplete).
4. Once a task is successfully completed and its output file(s) are generated, update this `discoveryTracker.md` file by changing the `[ ]` to `[x]` for that task.
5. Save the updated `discoveryTracker.md`.
6. Proceed to the next task marked `[ ]`.
7. The process is complete when all tasks are marked `[x]`.

**Task List & Status:**

- [ ] **Task 1: Generate Inferred Product Requirements Document**
  - *Prompt File:* `#file:discovery_task_1_inferred_requirements.prompt.md`
  - *Output File:* [inferred_requirements.md](./inferred_requirements.md)

- [ ] **Task 2: Generate Architecture and Design Diagrams (Mermaid)**
  - *Prompt File:* `#file:discovery_task_2_diagrams.prompt.md`
  - *Output Files:*
    - [discoveryTracker.md](./diagrams/system_architecture.md)
    - [application_architecture.md](./diagrams/application_architecture.md)
    - [data_flow_diagram.md](./diagrams/data_flow_diagram.md)
    - [dependency_graph.md](./diagrams/dependency_graph.md)
    - [component_diagram.md](./diagrams/component_diagram.md) (Optional)
    - [relationship_diagram.md](./diagrams/relationship_diagram.md) (Optional)

- [ ] **Task 3: Generate Dependency Analysis Report**
  - *Prompt File:* `#file:discovery_task_3_dependencies.prompt.md`
  - *Output File:* [dependency_analysis.md](./dependency_analysis.md)

- [ ] **Task 4: Generate Code Quality and Idiom Analysis**
  - *Prompt File:* `#file:discovery_task_4_code_quality.prompt.md`
  - *Output File:* [code_quality_idiom_analysis.md](./code_quality_idiom_analysis.md)

- [ ] **Task 5: Generate Test Coverage Assessment & Gap Analysis**
  - *Prompt File:* `#file:discovery_task_5_test_coverage.prompt.md`
  - *Output File:* [test_coverage_analysis.md](./test_coverage_analysis.md)

- [ ] **Task 6: Generate Design Pattern Analysis**
  - *Prompt File:* `#file:discovery_task_6_design_patterns.prompt.md`
  - *Output File:* [design_patterns_analysis.md](./design_patterns_analysis.md)

- [ ] **Task 7: Generate Static Code Analysis Report**
  - *Prompt File:* `#file:discovery_task_7_static_analysis.md`
  - *Output File:* [static_analysis_report.md](./static_analysis_report.md)

- [ ] **Task 8: Generate Performance Enhancement Report**
  - *Prompt File:* `#file:discovery_task_8_performance_enhancement.prompt.md`
  - *Output File:* [performance_enhancement_report.md](./performance_enhancement_report.md)

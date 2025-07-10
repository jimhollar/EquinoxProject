# Task 2: Generate Architecture and Design Diagrams

**Role:** You are an expert AI assistant specializing in software architecture, code analysis, and visual documentation generation using tools like Mermaid.

**Context:** This task focuses on creating visual representations of the application's architecture and structure as part of the overall documentation process.

**Goal:** Analyze the provided application source code and generate key architecture and design diagrams using Mermaid syntax (version 10 or later).  The diagrams should be visually appealing concise, complete and accurate.

**Input:** Complete source code of the application in #codebase (Assume access includes code files, dependency configuration files).

**Instructions:**

1. Analyze the application's structure, components, dependencies, and data flow.
2. Generate the following diagrams using valid Mermaid syntax embedded within Markdown code blocks (```mermaid ...```):
    * **System Architecture Diagram:** High-level view showing application components, boundaries, external systems (databases, APIs, message queues, file storage), and interaction protocols.
    * **Application Architecture Diagram:** Internal structure showing main modules/layers/components and their primary interactions/dependencies *within* the application.
    * **Data Flow Diagram:** Illustrate the primary pathways and transformations of data through the system or key components.
    * **Dependency Graph:** Visualize the application's key internal modules/components and their direct dependencies on *external libraries* (from configuration files like `requirements.txt`, `package.json`, `pom.xml`, etc.).
    * **Component Diagram:** If the architecture is component-based, visualize the structure and relationships of key software components.
    * **Class/Module Relationship Diagram:** Visualize key relationships like inheritance, composition, or significant dependencies within critical parts of the codebase if they impact understanding.
    * **Sequence Diagrams:** Visualize key workflows and represent them as sequence diagrams.  The diagrams should be persisted in `discovery/diagrams/sequence` folder.  Each sequence should be represented a single set of related workflows.
3. Ensure all diagram descriptions within the Mermaid code blocks do *not* contain `(` character, as this can cause rendering issues. Use parentheses `()` sparingly and carefully escape them if necessary, though avoiding them in descriptions is preferred.

**Output Requirements:**

* Generate multiple Markdown (`.md`) files, one for each required diagram type.
* Each file should contain a single, correctly formatted Mermaid code block representing the diagram.
* The files must be saved within the `discovery/diagrams/` folder.
* File Names: `system_architecture.md`, `application_architecture.md`, `data_flow_diagram.md`, `dependency_graph.md`, `component_diagram.md` (if generated), `relationship_diagram.md` (if generated).
* Diagrams should be reasonably concise and clear.
* State any assumptions made about the architecture or external systems.
* Ensure the output is professional, concise, and accurate.
* Format the mermaid code blocks correctly for rendering and use Flowchart syntax if unable to use the other diagram types.

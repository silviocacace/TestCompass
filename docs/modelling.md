# Modelling

Modelling is the foundation of early Model-Based Testing (eMBT).  
In TestCompass, a model represents the intended behaviour of a system in a clear, structured, and explicit way.  
It serves as a shared thinking tool for business and technical stakeholders, enabling early discovery of ambiguities, risks, and misunderstandings.

This page explains the conceptual principles behind modelling in TestCompass and how models support systematic test generation, impact analysis, and collaborative understanding.

---

## Purpose of Modelling

A model makes behaviour explicit.  
Instead of relying on assumptions, implicit knowledge, or scattered requirements, the model provides a single, visual representation of:

- decisions  
- business rules  
- flows and outcomes  
- boundary conditions  
- exceptional behaviour  

By externalising behaviour, teams can reason more clearly, validate understanding earlier, and avoid costly rework later in the development process.

---

## Modelling Principles

TestCompass uses a lightweight, expressive modelling style based on flowchart principles.  
The goal is not to create a perfect diagram, but to create a **shared understanding** of behaviour.

Key principles:

- **High-level abstraction**  
  Models should be understandable by both business and IT.

- **Explicit decisions**  
  Every decision is represented visually, making happy and unhappy paths visible.

- **Clear outcomes**  
  Each path leads to a result that reflects the expected system behaviour.

- **No hidden assumptions**  
  If something is unclear, it becomes visible in the model.

- **Iterative refinement**  
  Models evolve as requirements become clearer.

---

## Node Types

TestCompass models use a small set of node types to keep diagrams simple and readable:

- **Start**  
  The entry point of the behaviour. A model always begins with exactly one Start node.

- **Action / State**  
  Represents an action or a state in the flow.  
  Has exactly one outgoing link.

- **Decision**  
  Represents a branching point with two explicit outcomes: Yes and No.  
  These branches are classified as test paths and are important for test generation.

- **Result**  
  Represents an expected outcome or observable effect.

- **End**  
  Represents the termination of the behaviour.  
  A model must contain at least one End node.

- **Comment**  
  Used to capture questions, ambiguities, contradictions, or open ends.  
  Comments are not connected to the flow and serve as prompts for review.

These elements are sufficient to express complex behaviour without overwhelming the reader.

---

## Model Validation

TestCompass automatically validates the structure of a model to ensure it is logically sound.  
Validation checks include:

- missing or incorrect links  
- nodes with invalid numbers of incoming or outgoing transitions  
- unreachable behaviour  
- missing end nodes  
- structural inconsistencies in decision logic  

These validations help teams detect structural issues early, before generating tests or exporting artefacts.  
Validation is not a replacement for review — it is a safeguard that supports clear, explicit modelling.

---

## Preconditions and Data

Nodes may optionally contain preconditions or data.  
When provided, these enrich the model and are automatically included in exported artefacts such as:

- Excel test designs  
- decision tables  
- Gherkin feature files  

Preconditions and data do not change the structure of the model, but they make the resulting test scenarios more concrete and executable.

---

## Modelling Workflow

Modelling typically follows an iterative workflow aligned with the eMBT phases:

1. **Exploratory**  
   Initial model creation based on available requirements.  
   Questions, ambiguities, and assumptions are captured using comment nodes.

2. **Review**  
   The team discusses the model, resolves uncertainties, and updates the behaviour accordingly.

3. **Coverage**  
   Once validated, the model becomes the basis for systematic test generation.

4. **Checking**  
   The model and generated tests are used to verify the system under test.

This workflow ensures that modelling is not a one‑time activity but a continuous source of clarity.

---

## Requirements Discovery Practices

TestCompass supports collaborative requirements discovery practices such as:

- Feature Mapping  
- Example Mapping  

These practices help teams explore behaviour, identify business rules, and clarify examples before modelling.  
Because the maps are created directly in the modelling environment, they can be transformed into a complete model with minimal effort, ensuring continuity from discovery to modelling to test generation.

---

## Modelling with Gherkin

TestCompass supports modelling using Gherkin concepts such as:

- Feature  
- Background  
- Rule  
- Given / When / Then  
- And / But  
- Examples  

This allows teams to generate Gherkin feature files directly from the model, ensuring that executable specifications remain aligned with the behavioural structure.

Gherkin modelling is flexible:  
the model expresses the behaviour, while the Gherkin labels provide semantic meaning for BDD workflows.

---

## Modelling with Mermaid

TestCompass supports open, text-based modelling through Mermaid:

- Import Mermaid diagrams and convert them into testable models  
- Export models back to Mermaid for documentation or version control  

This enables teams to collaborate using plain text, pull requests, and version-controlled workflows.

➡️ See examples in the repository’s Mermaid section.

---

## Relationship to Test Generation

A well‑structured model directly enables:

- path-based test generation  
- decision coverage  
- boundary-oriented coverage  
- minimal path sets  
- custom constraints  

The quality of the model determines the quality of the generated tests.

➡️ Learn more: **[Test Generation](ca://s?q=Open_test_generation_documentation)**

---

## Relationship to Impact Analysis

When requirements change, the model is updated — not the tests.  
TestCompass automatically identifies which generated scenarios are:

- added  
- removed  
- updated  
- unchanged  

This keeps test suites maintainable and aligned with evolving requirements.

➡️ Learn more: **[Impact Analysis](ca://s?q=Open_impact_analysis_documentation)**

---

Modelling is not about drawing diagrams — it is about creating clarity.  
TestCompass provides the structure, the notation, and the workflow to make that clarity possible.


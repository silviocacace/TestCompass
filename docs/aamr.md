[← Back to Documentation Index](index.md)

# AAMR – AI-Assisted Model Reflection

AAMR (AI-Assisted Model Reflection) is an AI-supported feature within TestCompass designed to help teams critically review, challenge, and strengthen existing test models.

Rather than generating models automatically, AAMR analyzes the model's context and structure to guide users through a structured brainstorming process—engaging them with targeted questions and alternative perspectives to uncover blind spots and hidden assumptions.

> **Purpose & Role of AAMR**  
> AAMR acts as a collaborative thinking partner and catalyst for critical thinking. It does not replace human judgment; instead, it challenges assumptions, highlights potential risks, and sparks creative test ideas while keeping all final modeling decisions strictly under user control.

---

## Behavioural Characteristics & How AAMR Works

AAMR analyzes the structural layout and underlying business semantics of a TestCompass model to trigger structured reflection.

### 1. Contextual 3-Question Brainstorming
Instead of providing generic feedback or direct answers, AAMR engages the user with **3 targeted, thought-provoking questions** derived directly from the model's specific context. These questions challenge boundary conditions, unhandled paths, and implicit business rules.

### 2. Interactive Reflection & Evaluation
AAMR guides the team through a reflective evaluation loop:
* **Uncovering Blind Spots:** Identifies unhandled exceptions, missing returns, or ambiguous decision outcomes.
* **Reviewing Implications:** Presents potential risk areas, missing test ideas, or structural improvements.
* **Refining Suggestions:** Users can review, modify, or reject generated suggestions before deciding what to integrate into their workspace.

### 3. Visual Canvas Integration via Balloon Nodes
When a user accepts one or more generated suggestions or implications at the end of the AAMR reflection process:
* The accepted items are **automatically added directly to the TestCompass model workspace**.
* They are visually represented as **grey balloon nodes** linked to the relevant parts of the flow.
* Modelers can then optionally adjust, integrate, or expand the model based on these visual reflection nodes.

---

## Supported Reflection Outcomes

During an AAMR session, the generated reflections generally focus on:

- **Clarification Questions:** Specific inquiries regarding decision logic, boundary conditions, or unhandled branches.
- **Structural & Flow Observations:** Identification of single-entry paths, dead ends, or missing termination states.
- **Potential Ambiguities:** Highlighting logic that business and technical stakeholders might interpret differently.
- **Missing Behaviour & Exception Paths:** Identifying missing error handling, fallback routines, or system timeouts.
- **Risk & Test Idea Generation:** Proposing edge cases and risk-oriented scenarios for test coverage.

<p align="center">
  <img src="AAMR_explanation.png" alt="TestCompass AAMR Reflection Canvas" width="600">
</p>

---

## Example Reflection Scenarios

When analyzing a model draft, AAMR presents questions such as:

- *What happens if this decision evaluates to "No" or times out?*
- *Is this outcome valid under all boundary conditions, or are there hidden prerequisites?*
- *Can a user navigate back to a previous state, or is this workflow strictly linear?*
- *Are all exception handling paths and error notifications explicitly modeled?*
- *Does this subprocess have a clearly defined termination point for all execution branches?*

These targeted prompts encourage deeper examination during peer reviews, refinement sessions, and three-amigos discussions.

---

## Model Reflection Workflow

1. **Analyze:** Run AAMR on an existing TestCompass model draft.
2. **Engage:** Review the 3 targeted contextual reflection questions and observations.
3. **Evaluate & Refine:** Discuss implications with the team and adjust suggestions as needed.
4. **Integrate:** Accept relevant suggestions to automatically project them onto the canvas as **grey balloon nodes**.
5. **Update Model:** Refine the core model structure based on the newly accepted nodes before test path generation.

---

## What AAMR Is Not

To maintain clarity around its design philosophy, AAMR is explicitly **not**:
- An automated model editor or auto-corrector
- A replacement for human testing domain expertise
- A system that enforces a single "correct" business interpretation
- A tool that modifies your model without explicit user approval

> **Human-in-the-Loop Philosophy**  
> The tester retains complete authority over the testing approach. AAMR suggests and highlights possibilities; the human expert decides what is valid and accepted into the model.

---

## Complementary Relationship: AAMC vs. AAMR

AAMC and AAMR support complementary stages within the early Model-Based Testing (eMBT) lifecycle:

### AAMC (AI-Assisted Model Creation)
- **Phase:** Model Creation
- **Primary Goal:** Transforms raw text, user stories, spreadsheets, or legacy diagrams into an initial, compliant TestCompass model draft.

### AAMR (AI-Assisted Model Reflection)
- **Phase:** Model Review
- **Primary Goal:** Challenges, refines, and validates an existing model draft by exposing gaps, risks, and assumptions through interactive reflection.

---

> **Summary**  
> Together, AAMC and AAMR accelerate the transition from vague requirements to robust, thoroughly reviewed TestCompass models, ensuring high test coverage and early risk identification before test execution begins.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**


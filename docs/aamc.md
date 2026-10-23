[← Back to Documentation Index](index.md)

# AAMC – AI-Assisted Model Creation

AAMC (AI-Assisted Model Creation) is an AI-supported feature within TestCompass that transforms behavioural descriptions into an initial TestCompass model draft.

It allows teams to start modelling directly from requirements, user stories, workshop notes or system specifications—rather than creating a model manually from scratch.

> 💡 **Purpose & Role of AAMC**  
> AAMC is designed to accelerate the creation of initial TestCompass models. It acts as a modelling assistant, not a replacement for human expertise. It provides a structured starting point so teams can spend less time building models manually and more time analyzing behaviour, detecting gaps, contradictions and open ends in the requirements and  identifying risks early.

---

## Behavioural Characteristics & Best Practices

AAMC interprets input text, identifies actions, decisions, outcomes and branching logic and converts them into a visual TestCompass model draft.

### Generative Nature & Iteration
Because generative AI is non-deterministic, the same input text may produce slightly different model interpretations. 
* **Model Regeneration:** If an initial draft contains structural inconsistencies or suboptimal flows, regenerating the model produces a fresh interpretation of the input.
* **User Control:** Users retain full control over whether to accept a generated draft, run another generation, or adjust the model manually in the workspace.

### Single Process Input Focus
For optimal results, input descriptions should focus on **one clear process from start to finish**.
* Providing requirements that contain multiple distinct processes, multiple primary actors, or unrelated parallel flows may result in disconnected model structures ("islands").
* Multi-process documentation should be provided to AAMC incrementally, one process at a time, to build focused and maintainable models.
* AAMC fully handles complex logic, decision trees, error paths, and system validations as long as they belong to the same core process.

---

## Supported Inputs

AAMC processes both unstructured natural language and structured, machine-readable formats:

### Natural Language
- Requirements & Acceptance Criteria
- User Stories & Scenarios
- Domain Descriptions & Business Process Rules
- Workshop Notes & Discussion Summaries

### Structured Formats
- **BPMN 2.0 XML**
- **JSON Workflow Definitions**
- **XML Behaviour Descriptions**
- **Mermaid Diagrams** & **Gherkin Scenarios**
- **OCR / External AI Outputs:** Text extracted from image files, whiteboard sketches, or external AI tools.

---

## Model Validation & Handling Issues

After generation, TestCompass automatically validates the model structure directly on the canvas:

* **Visual Indicators:** Structural anomalies—such as isolated nodes, action nodes with multiple outgoing links, or decision nodes without clear binary outcomes—are highlighted with visual markers.
* **Resolution Strategy:** When a generated draft contains multiple structural issues, regenerating is generally more efficient than manual correction. For minor issues (such as a single missing transition), accepting the draft and making quick adjustments directly in the editor or reviewing the Test tab is recommended.

<p align="center">
  <img src="AAMC_explanation.png" alt="TestCompass AAMC Explanation Canvas" width="600">
</p>

---

## Example: Generating an eMBT Model from Requirements

The example below demonstrates how AAMC converts a short natural language requirement into a structured, semantically consistent TestCompass model while exposing incomplete logic.

---

### 1. Input Requirement (English)

> After creating an account, the system asks the user to complete their profile.  
> The user provides the requested information.  
> The system checks whether all mandatory fields are filled in.  
> If all mandatory fields are provided, the system verifies the user’s email address.  
> If the email is verified, the system activates the user’s account.  
> If the email is not verified, the system informs the user that verification is required.

---

### 2. Generated Model Draft

AAMC generates an initial model draft directly inside TestCompass:

<p align="center">
  <img src="Model_AAMC.png" alt="AAMC Generated TestCompass Model Draft" width="600">
</p>

---

### 3. Key Takeaways from the Generated Model

- **Explicit Decisions:** Automatically identifies key branching logic (*"All mandatory fields filled in?"*, *"Email verified?"*).
- **No Unsafe Assumptions:** AAMC does not guess or invent logic for unspecified paths (e.g., what happens if mandatory fields are missing).
- **Exposing Incomplete Behaviour:** Unspecified outcomes are left open and marked with visual indicators so teams can clarify gaps early.

---

> **Key Takeaway**  
> AAMC bridges the gap between text requirements and visual modelling in seconds. It exposes ambiguity early, providing a clean baseline to refine, execute impact analysis on, and derive test scenarios from.

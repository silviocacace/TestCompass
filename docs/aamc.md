[← Back to Documentation Index](index.md)

# AAMC – AI-Assisted Model Creation

AAMC (AI-Assisted Model Creation) is an AI-supported feature within TestCompass that transforms behavioural descriptions into an initial TestCompass model draft.

It allows users to start modelling directly from requirements, user stories, workshop notes, business process descriptions, and other sources—rather than creating a model manually from scratch.

> ⚡ **Purpose of AAMC**  
> AAMC is designed to accelerate the creation of initial TestCompass models. By providing a structured starting point, it helps teams begin modelling earlier and spend more time reviewing, refining, and exploring behaviour rather than building models manually.

The generated draft can immediately be reviewed, refined, and used within TestCompass for extending, impact analysis, and generating test scenarios.

---

## Supported Inputs

AAMC can process both natural-language and structured inputs, including:

### 📄 Natural Language
- Requirements & Acceptance Criteria
- User Stories & Scenarios
- Domain Descriptions
- Workshop & Discussion Notes

### 🧩 Structured Inputs
- BPMN 2.0 XML
- JSON Workflow Definitions
- XML Behaviour Descriptions
- Mermaid Diagrams
- Gherkin Scenarios
- Other machine-readable behavioural formats

---

## Generated Output

AAMC generates an initial TestCompass model draft containing:

- **Model structure & flow**
- **Actions & States**
- **Decisions & Branching logic**
- **Transitions & Test paths**
- **Expected Results**

After generation, TestCompass automatically validates the model structure and highlights any detected modelling or semantic issues directly within the canvas.

<p align="center">
  <img src="AAMC_explanation.png" alt="TestCompass AAMC Explanation Canvas" width="600">
</p>

---

## Example: Generating an eMBT Model from Requirements

AAMC converts natural language requirements directly into a structured, semantically consistent TestCompass model.  
The example below demonstrates how AAMC interprets a short requirement, identifies decisions, and exposes incomplete behaviour without making assumptions.

---

### 1. Input Requirement (English)

> After creating an account, the system asks the user to complete their profile.  
> The user provides the requested information.  
> The system checks whether all mandatory fields are filled in.  
> If all mandatory fields are provided, the system verifies the user’s email address.  
> If the email is verified, the system activates the user’s account.  
> If the email is not verified, the system informs the user that verification is required.

---

### 2. Generated Model

AAMC generates an initial model draft directly inside TestCompass:

<p align="center">
  <img src="Model_AAMC.png" alt="AAMC Generated TestCompass Model Draft" width="600">
</p>

---

### 3. Explanation & Workflow

- 🔀 **Explicit Decisions:** AAMC automatically identifies key branching logic (*"All mandatory fields filled in?"*, *"Email verified?"*).
- 🚫 **No Assumptions:** AAMC does not guess or invent logic for missing requirements (e.g. what happens if mandatory fields are missing).
- ❓ **Exposing Incomplete Behaviour:** Paths that lack explicit specification are left open and marked with a visual indicator (such as an exclamation mark / question mark).
- 🔍 **Integrated Validation:** Once you accept the AAMC draft into your TestCompass workspace, these markers become part of the active model. TestCompass highlights them to show unverified or incomplete paths, enabling teams to clarify missing specifications early.

---

> 💡 **Key Takeaway**  
> This example illustrates how AAMC exposes ambiguity and missing paths instead of hiding them, allowing teams to address open ends before development or coding begins.

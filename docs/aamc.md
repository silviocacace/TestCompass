[← Back to Documentation Index](index.md)

# AAMC – AI-Assisted Model Creation

AAMC (AI-Assisted Model Creation) is an AI-supported feature within TestCompass that helps transform behavioural descriptions into an initial TestCompass model draft.

It allows users to start modelling from requirements, user stories, workshop notes, business process descriptions and other behavioural sources rather than creating a model manually from scratch.

The generated draft can then be reviewed, refined and used within TestCompass for e.g. extending, impact analysis, generating test scenarios, etc.

---

## Purpose

AAMC is designed to accelerate the creation of initial TestCompass models from behavioural descriptions.

It provides a structured starting point that helps teams begin modelling earlier and spend more time reviewing, refining and exploring behaviour rather than creating a model from scratch.

---

## Supported Inputs

AAMC can process both natural-language and structured inputs, including:

### Natural Language
- requirements
- user stories
- acceptance criteria
- scenarios
- domain descriptions
- workshop or discussion notes

### Structured Inputs
- BPMN 2.0 XML
- JSON workflow definitions
- XML behaviour descriptions
- Mermaid diagrams
- Gherkin scenarios
- other machine-readable behavioural formats

---

## Generated Output

AAMC generates an initial TestCompass model draft containing:

- model structure
- actions
- decisions
- transitions
- behavioural flows

The generated model can immediately be reviewed, refined and further developed inside TestCompass.

After generation, TestCompass automatically validates the model and highlights any detected modelling or semantic issues directly within the model.

---

## Example: Generating an eMBT Model from Natural Language Requirements

AAMC converts natural language requirements directly into a structured, semantically consistent TestCompass model.  
The example below demonstrates how AAMC interprets a short requirement, identifies decisions, and exposes incomplete behaviour without making assumptions.

---

### Input Requirement (English)

> After creating an account, the system asks the user to complete their profile.  
> The user provides the requested information.  
> The system checks whether all mandatory fields are filled in.  
> If all mandatory fields are provided, the system verifies the user’s email address.  
> If the email is verified, the system activates the user’s account.  
> If the email is not verified, the system informs the user that verification is required.

---

### Generated Model

AAMC generates an initial model draft directly inside TestCompass:

![Generated TestCompass Model for Account Creation](images/Model_AAMC.png)

*(Replace `images/aamc-generated-model.png` with the actual filename of your uploaded image)*

---

### Explanation & Workflow

- **Explicit Decisions:** AAMC identifies the key branching logic ("All mandatory fields filled in?", "Email verified?").
- **No Assumptions:** AAMC does not guess or invent logic for missing requirements.
- **Exposing Incomplete Behaviour:** Paths that lack description are left open and marked with an indicator (such as an exclamation mark). 
- **Integrated Validation:** Once you accept the AAMC draft into the TestCompass workflow, these markers become part of the model. TestCompass then highlights them to show that the path is unverified or incomplete, enabling teams to address missing specifications early.

This example illustrates how AAMC exposes ambiguity and missing paths instead of hiding them, allowing teams to clarify requirements before development begins.

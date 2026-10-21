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

AAMC converts natural language requirements into a structured, semantically consistent eMBT model.  
The example below demonstrates how AAMC interprets a short requirement, identifies decisions, and exposes incomplete behaviour without making assumptions.

---

### Input Requirement (English)

After creating an account, the system asks the user to complete their profile.
The user provides the requested information.
The system checks whether all mandatory fields are filled in.
If all mandatory fields are provided, the system verifies the user’s email address.
If the email is verified, the system activates the user’s account.
If the email is not verified, the system informs the user that verification is required.
*(The requirement does not describe what happens if mandatory fields are missing.)*
*(The requirement does not describe what happens after informing the user about email verification.)*

---

### Generated Model (Mermaid)

AAMC generates an initial TestCompass model draft.
The Mermaid diagram shown below is only a documentation-friendly visualization of that model, not the model itself.

```mermaid
flowchart TD
    Start([Start]) --> A[Ask user to complete profile]
    A --> B[User provides requested information]
    B --> C{All mandatory fields filled?}

    C -->|Yes| D{Email verified?}
    C -->|No| E[Missing behaviour]

    D -->|Yes| F[Activate user's account]
    D -->|No| G[Inform user that verification is required]

    F --> End([End])
    G --> H[Missing behaviour]
    H --> End([End])

[← Back to Documentation Index](index.md)

# AAMC – AI-Assisted Model Creation

AAMC (AI-Assisted Model Creation) is a feature in TestCompass that converts flexible text-based input (plain text) into an initial model draft. The input can range from free-form text and user stories to structured formats like Mermaid diagrams, JSON, XML, decision tables, etc.

It allows teams to start modelling directly from requirements, user stories, workshop notes, or system specifications, without having to build the model manually node by node.

> **Purpose & Role of AAMC**  
> AAMC speeds up the creation of initial TestCompass models. It acts as an assistant, not a replacement for human testing experience. It provides a solid starting point so teams can spend less time drawing models and more time reviewing business logic, finding missing requirements, and identifying risks early.

---

## How AAMC Works & Best Practices

AAMC reads the input text, identifies actions, decisions, outcomes, and branches, and turns them into a visual model draft based on TestCompass modelling rules.

### Working with Draft Iterations
Because AI generation can vary slightly each time, the same text might yield slightly different model layouts. 
- **Regenerating Models:** If a generated draft looks messy or misses a logical step, regenerating it creates a fresh interpretation of the input.
- **Full User Control:** You decide whether to accept a generated draft, run another generation, or adjust the model yourself in the editor.

### Focus on One Process at a Time
For the best results, input text should cover **one clear process from start to finish**.
- Combining multiple unrelated processes or different user roles in one text can result in loose, disconnected model parts.
- Large specifications are best fed to AAMC step by step, one process at a time, to keep models clear and maintainable.
- AAMC easily handles complex logic, decision flows, and error paths, as long as they belong to the same core process.

---

## Supported Input Formats

AAMC can process plain text, spreadsheets, legacy diagram exports, and structured files:

### Plain Text & Notes
- Requirements & Acceptance Criteria
- User Stories & Scenarios
- Business Process Rules
- Workshop Notes & Discussion Summaries

### Spreadsheets & Tables
- **Excel Decision Tables:** Tables with conditions, rules, and outcomes are automatically turned into decision logic.
- **CSV & Decision Grids:** Rule matrices and tabular logic.
- **Other Tables** (e.g., Markdown, Word, or Confluence tables).

### Structured & Diagram Formats
- **BPMN 2.0 XML**
- **JSON & XML Workflow Files**
- **Mermaid Diagrams & Gherkin Scenarios**
- **Diagram Migrations:** Text, JSON, or Mermaid exported from tools like Visio, Lucidchart, or Draw.io, or extracted from whiteboard photos.

> **Migrating Existing Models**  
> If you are moving existing process diagrams (like Visio or Lucidchart flows) into TestCompass, you for e.g. can export them as JSON, XML, or Mermaid and load them into AAMC. As long as a process or business rule can be written as text, whether in plain prose, spreadsheets, or code, AAMC can read it and generate a initial model draft.

---

## Model Checks & Fixing Issues

After generating a draft, TestCompass automatically checks it against official modelling rules:

- **Red Exclamation Marks:** If a model breaks a rule, for example, a decision node with only 1 outgoing path, or an action node with no output, TestCompass flags it directly on the canvas with a red exclamation mark.
- **Fixing Issues:** If a draft has multiple structural errors, clicking **Regenerate** is usually faster than fixing it manually. For small issues (like a single missing connection), simply accept the draft and edit it directly in the workspace.

<p align="center">
  <img src="AAMC_explanation.png" alt="TestCompass AAMC Explanation Canvas" width="600">
</p>

---

## Example: Creating a Model from Requirements

Here is a simple example showing how AAMC turns a short requirement into a structured model while highlighting missing logic.

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

AAMC generates this initial model draft in TestCompass:

<p align="center">
  <img src="Model_AAMC.png" alt="AAMC Generated TestCompass Model Draft" width="600">
</p>

---

### 3. Model Analysis & Observations

- **Explicit Decisions:** Automatically identifies decision points (*"All mandatory fields filled in?"*, *"Email verified?"*).
- **No Unsafe Guesses:** AAMC does not invent rules for paths that are not described (e.g., what happens if mandatory fields are missing).
- **Highlighting Requirement Gaps:** Unspecified outcomes are left open on purpose. Because an open path violates TestCompass model rules, the app flags it with a red exclamation mark. This makes missing business logic visible before development starts.

---

> **Summary**  
> AAMC turns text requirements into visual models in seconds. By running instant rule checks, it highlights missing logic and gaps early, giving teams a clean starting point for test generation and impact analysis.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

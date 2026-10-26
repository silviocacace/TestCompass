[← Back to Documentation Index](index.md)

# early Model-Based Testing (eMBT)

Early Model-Based Testing (eMBT) is a collaborative testing approach that helps teams build a shared understanding of requirements early in the development lifecycle. It does much more than just speed up test design. eMBT stimulates critical thinking and communication between business and technical stakeholders. Discovering misunderstandings, ambiguities, or missing details early helps prevent costly defects later.

---

> 💡 **Why Intent-Driven eMBT Matters**  
> Traditional testing often checks *what is written* in specifications, even if those requirements miss important details. Intent-Driven eMBT supported by TestCompass ensures teams uncover and validate *what business stakeholders actually meant*. By visually modelling system behaviour during early design, you do not just capture specifications, you actively explore them. This exposes risks, missing logic, wrong assumptions, and contradictions early, ensuring everyone shares the same understanding before a single line of code is written.  
>   
> *This is how you shift from a late quality stamp of approval to building correct specifications from day one.*

---

## The Philosophy of early Model-Based Testing (eMBT)

When people hear model-based testing, they often think of technical test generation at the end of a sprint. eMBT takes a practical, collaborative approach. 

Instead of treating models purely as technical inputs for automated scripts, eMBT positions explicit models as shared thinking tools for the entire team:

- **Collaboration First:** The model acts as a bridge during refinement and Three Amigos sessions, helping business analysts, developers, and testers speak the same language.
- **Clarity Before Code:** By visualizing workflows and intent before development starts, teams uncover misunderstandings when they are still fast and cheap to fix.
- **Intent Over Output:** Test generation is a natural outcome of a validated model, but the true value lies in revealing stakeholder intent and capturing shared insights while building the model.

> **Key Takeaway**  
> eMBT is not just a test design technique. It is an intentional, collaborative mindset that makes thinking visible early, ensuring teams build the right thing from day one.

---

## The Four Iterative Phases of eMBT

eMBT structures the testing workflow into four iterative phases:

<p align="center">
  <img src="eMBT_phases.jpg" alt="The 4 Iterative Phases of eMBT" width="550">
</p>

---

### 1. Exploratory Phase
In this phase, the team explores and visualizes the requirements and underlying intent. The goal is to make behaviour explicit and identify:

- ambiguities and missing specifications
- inconsistencies in business rules
- open ends and unhandled scenarios
- hidden assumptions between business and IT
- potential risks and test ideas

A graphical test model is created directly in TestCompass as a shared thinking tool. Teams can also conduct collaborative discovery directly on the canvas using interactive Sticky Note nodes for Feature and Example Mapping, or use AI-Assisted Model Creation (AAMC) to draft test models in seconds.

*(See: [BDD Requirements Discovery](bdd-discovery.md))*

---

### 2. Review Phase
All questions, open ends, and uncertainties raised during the exploratory phase are reviewed with the full team. Business and IT validate:

- the true meaning and intent of requirements
- business rules and decision logic
- boundary conditions and edge cases
- exception paths and risk scenarios

TestCompass enhances this phase with AAMR (AI-Assisted Model Reflection), acting as an interactive reflection partner to challenge assumptions and surface hidden gaps. Every requirement change or newly discovered risk leads to an updated model and a brief review cycle.

---

### 3. Coverage Phase
Once the model is validated, test scenarios and specifications are automatically derived based on the selected mathematical coverage strategy.

The following coverage levels are available:

- **Node coverage (NC):** covers all actions, decisions, and results at least once.
- **Edge coverage (EC):** covers all transitions and yes/no branches.
- **Path Pair coverage (PPC):** covers combinations of two consecutive decision branches.
- **Path Triple coverage (PTC):** covers combinations of three consecutive decision branches.
- **Full Path coverage (FPC):** covers all possible end-to-end paths.

By defining test data and preconditions within node details, TestCompass automatically derives Data-Driven Gherkin Scenario Outlines for BDD and physical test scenarios complete with data matrices for Excel test design.

---

### 4. Checking Phase
The generated coverage-based test scenarios serve as the design blueprint for test execution, whether executed manually, via automated scripts, or a combination of both. 

While TestCompass focuses entirely on modelling, coverage, and systematic test design, it feeds your execution workflow by exporting ready-to-use artifacts:
- **Test Management:** export detailed test cases and decision matrices directly into Excel, CSV, Azure DevOps, Jira, Zephyr, or Xray.
- **Test Automation:** export coverage-derived Gherkin `.feature` files directly into automation frameworks like Cucumber, Reqnroll, SpecFlow, Playwright, or Cypress.

The goal is to verify that the actual implementation reflects stakeholder intent and to gain insight into release readiness.

---

## Impact Analysis

Because requirements change continuously, eMBT includes a structured way to manage change without manual scenario upkeep. When the model is updated, an automated impact analysis shows which test scenarios are:

- **Added:** new behaviour introduced.
- **Removed:** obsolete behaviour.
- **Updated:** existing paths modified.
- **Unchanged:** remains fully valid.

This eliminates manual scenario maintenance, prevents drift between specifications and test suites, and keeps quality artifacts synchronized.

---

## Key Benefits of eMBT

eMBT helps teams:

- capture true business intent early and remove ambiguities before development begins
- foster shared understanding and improve collaboration between business and IT
- identify risks and missing behaviour sooner, avoiding hidden assumptions
- design coverage-based tests automatically directly from visual behavioural models
- manage change effortlessly through single-click model updates and automated impact analysis
- reduce rework and defects in production, protecting true business value

---

## Relation to TestCompass

TestCompass supports the complete eMBT lifecycle:

- In-Tool Discovery & Modelling (Exploratory Phase)
- Collaborative Reviewing & AI Reflection (Review Phase)
- Automated Test Scenario & Gherkin Generation (Coverage Phase)
- Impact Analysis & Test Management Export (Checking Phase)

In addition, TestCompass provides built-in AI capabilities to enhance reasoning:

- **AAMC (AI-Assisted Model Creation):** jumpstart modelling from natural language requirements or Mermaid diagrams.  
  ➡️ **Learn more:** [AAMC Documentation](aamc.md)

- **AAMR (AI-Assisted Model Reflection):** acts as a critical partner to uncover hidden risks, missing logic, and open ends.  
  ➡️ **Learn more:** [AAMR Documentation](aamr.md)

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

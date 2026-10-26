[← Back to Documentation Index](index.md)

# Overview

TestCompass is an **Intent-Driven early Model-Based Testing (eMBT)** platform designed to help teams reason clearly, uncover risks early, and build shared understanding before development begins. 

It brings together in-tool discovery, explicit behavioural modelling, AI-assisted model creation and reflection, and automated coverage-driven test design.

> **Purpose & Role of TestCompass**  
> TestCompass replaces hidden assumptions with explicit behavioural models, capturing true stakeholder intent, enabling early risk discovery, and deriving systematic, coverage-driven test suites before code is written.

This overview explains the fundamental value of TestCompass, the principles behind early Model-Based Testing (eMBT), and how the platform supports a structured, collaborative testing workflow.

---

## About the Creator

**TestCompass was created by Silvio Cacace**, drawing on over **30 years of practical domain expertise** in software testing, quality engineering, and Model-Based Testing.

Throughout his career leading test transformations across enterprise environments, Silvio recognized that most software defects originate from incomplete specifications and implicit assumptions long before code is written. 

<p align="center" style="margin-top: 20px;">
  <img src="Silvio1.PNG" alt="Silvio Cacace - Creator of TestCompass" width="300" style="border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
</p>

To address this, he originally pioneered the **ATS & DTM methodology and DTM tool**, which served as the foundation for modern test design automation. Building on years of practical application, Silvio evolved ATS & DTM into the **early Model-Based Testing (eMBT)** approach and created **TestCompass** as its next-generation platform. Today, eMBT and TestCompass are applied in corporate environments, embedded in professional testing frameworks, and taught within software engineering programs across multiple Universities.

---

## Why early Model-Based Testing (eMBT)?

Many defects in software projects originate from unclear, implicit, or incomplete requirements. Traditional test case generation, even when driven by fast AI prompts, often simply multiplies these requirement gaps by producing test cases based on incomplete logic.

eMBT addresses this by making system behaviour and true business intent explicit early in the lifecycle, enabling teams to:

- **Capture true stakeholder intent** rather than validating incomplete text specifications
- **Surface implicit requirements** and clarify edge cases before implementation
- **Eliminate hidden assumptions** between business analysts, developers, and testers
- **Prevent defects early** rather than managing bugs late in production
- **Establish clear shared understanding** across all stakeholders
- **Generate systematic, reproducible test suites** directly from validated behavioural models

TestCompass supports this approach by providing a modelling environment that is simple enough for business stakeholders to review, while remaining precise enough for automated test derivation.

➡️ **Learn more:** [The eMBT Approach](eMBT-approach.md)

---

## The Philosophy of early Model-Based Testing (eMBT)

When people hear "Model-Based Testing," they often think of technical test generation at the end of a sprint. eMBT takes a practical, collaborative perspective. 

Rather than treating models purely as technical inputs for automated scripts, eMBT positions explicit models as **shared thinking tools** for the team. 

- **Collaboration First:** The model acts as a bridge during refinement and "Three Amigos" sessions, helping business analysts, developers, and testers align on requirements.
- **Clarity Before Code:** By visualizing workflows before development starts, teams uncover misunderstandings while they are still fast and cheap to fix.
- **Intent Over Output:** Test generation is a natural outcome of a validated model, but the primary value lies in clarifying stakeholder intent while building the model.

> **Key Takeaway**  
> eMBT is not just a test design technique; it is an Intent-Driven collaborative mindset that makes thinking visible early, ensuring teams build the right thing from day one.

---

## What TestCompass Provides

TestCompass offers a complete workflow for early Model-Based Testing, focusing on **modelling, systematic test design, and specification generation**:

- **In-Tool Collaborative Discovery:** Run Feature and Example Mapping sessions directly within TestCompass using dedicated **Sticky Note nodes**, without needing external whiteboards.
- **Explicit Behavioural Modelling:** Create visual models that represent system logic, decisions, and state transitions using formal TestCompass model rules.
- **AI-Assisted Capabilities:** 
  - **AAMC (AI-Assisted Model Creation):** Generate initial models directly from raw text like user stories, Example Maps, or legacy diagrams (Visio, Lucidchart, Mermaid) and structured formats like Mermaid diagrams, JSON, XML, decision tables, etc.
  - **AAMR (AI-Assisted Model Reflection):** Use a structured 3-question reflection loop to uncover blind spots and project accepted changes onto the canvas.
- **Coverage-Based Test Design & Living Specifications:** Automatically derive test scenarios using graph coverage algorithms (Node, Edge, Path Pair, Path Triple, Full Path Coverage).
  - **Data-Driven BDD:** Generate structured Gherkin `.feature` files with `Scenario Outlines` and populated `Examples:` tables.
  - **Physical Test Scenarios:** Generate complete Excel Test Design matrices and Decision Tables when defining concrete test data, preconditions, and expected outcomes in node details.
- **Automated Impact Analysis:** Automatically detect added, removed, updated, and unchanged test scenarios whenever requirements or models evolve—eliminating manual scenario maintenance.
- **Export & Tooling Integration:** Feed execution frameworks and test management suites by exporting directly to Azure DevOps, Jira, Zephyr, Xray, Excel, CSV, or Gherkin `.feature` files.

---

## How TestCompass Fits into the Delivery Workflow

TestCompass is designed to integrate into modern, iterative agile workflows:

- Fits into version-controlled repositories and continuous documentation setups
- Supports early collaboration during refinement, "Three Amigos" sessions, and BDD discovery
- Promotes a Shift-Left quality approach by validating intent and specifications before coding begins
- Produces maintainable artifacts (living specifications) with full traceability to requirements
- Serves as the dedicated **test design engine**, passing structured artifacts to manual execution or automation frameworks (Cucumber, SpecFlow, Playwright, Cypress)

The result is a clear, shared understanding of system behaviour, reducing costly rework and protecting business value.

---

## What This Documentation Covers

This documentation provides conceptual guidance, architecture rules, and workflow explanations for:

- [The eMBT Approach](eMBT-approach.md)
- [Behavioural Modelling](modelling.md)  
- [AAMC – AI-Assisted Model Creation](aamc.md)
- [AAMR – AI-Assisted Model Reflection](aamr.md)
- [Test Generation and Coverage](test-generation.md)  
- [Impact Analysis](impact-analysis.md)  
- [Mermaid Import and Export](mermaid-import-export.md)
- [Export Formats](export-formats.md)
- [Integrations](integrations.md)
- [BDD Discovery & Formulation](bdd-discovery.md)
- [Security & Architecture](security-architecture.md)

*(Note: This documentation focuses on methodologies, architecture, and concepts. It is designed to complement the in-product Quick Start Guide and guided UI tours.)*

---

> **Summary**  
> By bridging the gap between stakeholder intent, explicit visual models, and automated test derivation, TestCompass ensures teams focus on shared understanding, early risk visibility, and reliable delivery decisions.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

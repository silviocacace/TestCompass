[← Back to Documentation Index](index.md)

# Overview

TestCompass is an **Intent-Driven early Model-Based Testing (eMBT)** platform designed to help teams reason clearly, uncover risks early, and build shared understanding before development begins. 

It brings together in-tool discovery, explicit behavioural modelling, AI-assisted model creation and reflection, and automated coverage-driven test design.

> **Purpose & Role of TestCompass**  
> TestCompass empowers teams to replace hidden assumptions with explicit behavioural models—capturing true stakeholder intent, enabling early risk discovery, and deriving systematic, mathematically sound test coverage before code is written.

This overview explains the fundamental value of TestCompass, the principles behind early Model-Based Testing (eMBT), and how the platform supports a structured, collaborative testing workflow.

---

## About the Creator

**TestCompass was created by Silvio Cacace**, drawing on over **30 years of practical domain expertise** in software testing, quality engineering, and Model-Based Testing.

Throughout his career leading test transformations across enterprise environments, Silvio recognized that most software defects originate from incomplete specifications and implicit assumptions long before code is written. 

<p align="center" style="margin-top: 20px;">
  <img src="Silvio1.PNG" alt="Silvio Cacace - Creator of TestCompass" width="300" style="border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
</p>

To bridge this gap, Silvio established the **early Model-Based Testing (eMBT)** methodology and created **TestCompass**, a collaborative, risk-driven platform designed to build shared understanding first. Today, eMBT and TestCompass are widely applied in mission-critical corporate environments, embedded in professional testing frameworks and taught within software engineering programs across multiple universities.

---

## Why early Model-Based Testing (eMBT)?

Many defects in software projects originate from unclear, implicit, or incomplete requirements. Traditional test case generation, even when driven by fast generative AI prompts, often simply scales these requirement gaps by producing plausible-looking test cases derived from incomplete logic.

eMBT addresses this by making system behaviour and true business intent explicit early in the lifecycle, enabling teams to:

- **Capture true stakeholder intent** rather than blindly validating incomplete text specifications
- **Surface implicit requirements** and clarify edge cases before implementation
- **Eliminate hidden assumptions** between business analysts, developers, and testers
- **Prevent defects early** rather than managing bugs late in production
- **Establish true shared understanding** across all stakeholders
- **Generate systematic, reproducible test suites** directly from validated behavioural models

TestCompass supports this approach by providing a modelling environment that is simple and intuitive enough for business stakeholders to review, while remaining formal and precise enough for automated test derivation.

➡️ **Learn more:** [The eMBT Approach](eMBT-approach.md)

---

## The Philosophy of early Model-Based Testing (eMBT)

When people hear "Model-Based Testing," they often think of technical test generation at the end of a sprint. eMBT takes a fundamentally different, collaborative perspective. 

Rather than treating models as technical input for automated scripts alone, eMBT positions explicit models as **shared thinking tools** for the entire team. 

- **Collaboration First:** The model acts as a bridge during refinement and "Three Amigos" sessions, helping business analysts, developers and testers speak the exact same language.
- **Clarity Before Code:** By visualizing workflows before development starts, teams uncover misunderstandings when they are still cheap and easy to fix.
- **Intent Over Output:** Test generation is a natural consequence of a validated model, but the true value lies in revealing true stakeholder intent and capturing shared insights *while building the model*.

> **Key Takeaway**  
> eMBT is not just a test design technique; it is an Intent-Driven collaborative mindset that makes thinking visible early, ensuring teams build the right thing from day one.

---

## What TestCompass Provides

TestCompass offers a complete end-to-end workflow for early Model-Based Testing, focusing entirely on **modelling, systematic test design, and specification generation**:

- **In-Tool Collaborative Discovery:** Run Feature and Example Mapping sessions directly within TestCompass using dedicated **Sticky Note nodes**, eliminating the need for external whiteboards.
- **Explicit Behavioural Modelling:** Create clear, structured visual models that represent system logic, decisions, and state transitions using formal TestCompass model rules.
- **AI-Assisted Capabilities:** 
  - **AAMC (AI-Assisted Model Creation):** Jumpstart models directly from raw text, user stories, Example Maps, or legacy diagrams (Visio, Lucidchart, Mermaid).
  - **AAMR (AI-Assisted Model Reflection):** Engage in a structured 3-question reflection loop to uncover blind spots and project accepted ideas directly onto the canvas.
- **Coverage-Based Test Design & Living Specifications:** Automatically derive test scenarios using graph coverage algorithms (Node, Edge, Path Pair, Path Triple, Full Path Coverage).
  - **Data-Driven BDD:** Generate structured Gherkin `.feature` files with `Scenario Outlines` and populated `Examples:` tables.
  - **Physical Test Scenarios:** Generate complete Excel Test Design matrices and Decision Tables when defining concrete test data, preconditions, and predictions in node details.
- **Automated Impact Analysis:** Instantly detect added, removed, updated, and unchanged test scenarios whenever requirements or models evolve—eliminating manual scenario maintenance.
- **Seamless Export & Tooling Integration:** Feed execution frameworks and test management suites by exporting directly to Azure DevOps, Jira, Zephyr, Xray, Excel, CSV, or Gherkin `.feature` files.

---

## How TestCompass Fits into the Delivery Workflow

TestCompass is designed to integrate naturally into modern, iterative agile workflows:

- Fits seamlessly into version-controlled repositories and continuous documentation setups
- Encourages early collaboration during refinement, "Three Amigos" sessions, and BDD discovery
- Supports a genuine "Shift-Left" quality culture by validating intent and specifications before coding begins
- Produces maintainable, reviewable artifacts (living specifications) that maintain full traceability to requirements
- Serves as the dedicated **test design engine**, passing ready-to-use artifacts to manual testing setups or automation runners (Cucumber, SpecFlow, Playwright, Cypress)

The result is a unified understanding of system behaviour, reducing costly rework, eliminating false confidence, and protecting true business value.

---

## What This Documentation Covers

This documentation provides conceptual guidance, architecture rules and workflow explanations for:

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

*(Note: This documentation focuses on methodologies, architecture, and concepts. It is designed to complement the in-product Quick Start Guide and guided UI tours.)*

---

> **Summary**  
> By bridging the gap between stakeholder intent, explicit visual models, and automated test derivation, TestCompass ensures teams focus on what truly matters: shared understanding, early risk visibility, and complete confidence in every delivery decision.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

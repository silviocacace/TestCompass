[← Back to Documentation Index](index.md)

# Overview

TestCompass is an early Model-Based Testing (eMBT) platform designed to help teams reason clearly, uncover risks early, and build shared understanding before development begins. 

It brings together explicit behavioural modelling, AI-assisted model creation and reflection, and open, text-based modelling.

> **Purpose & Role of TestCompass**  
> TestCompass empowers teams to replace hidden assumptions with explicit behavioural models, enabling early risk discovery, true shared understanding between business and IT, and systematic test generation before code is written.

This overview explains the fundamental value of TestCompass, the principles behind early Model-Based Testing (eMBT), and how the platform supports a structured, collaborative testing workflow.

<p align="left">
  <img src="Silvio1.PNG" alt="TestCompass Platform" width="350">
</p>

---

### About the Creator & The Origin of eMBT

**TestCompass was created by Silvio Cacace**, bringing over **30 years of practical domain expertise** in software testing, quality engineering, and Model-Based Testing. 

Throughout three decades of leading test transformations across enterprise environments, Silvio recognized a persistent pattern: most software defects can be traced back to the requirements phase, from incomplete specifications and implicit assumptions long before code is written. Traditional Model-Based Testing (MBT) tools were often too complex or technical for daily agile refinement, while modern generative AI tools often simply generate test cases from incomplete text without validating the underlying logic.

To bridge this gap, Silvio established the **early Model-Based Testing (eMBT)** methodology, a collaborative, risk-driven approach designed to build shared understanding first. Today, eMBT is widely applied in mission critical corporate environments, embedded in professional testing frameworks and taught within software engineering programs across multiple Universities.

---

## Why early Model-Based Testing (eMBT)?

Many defects in software projects originate from unclear, implicit, or incomplete requirements. Traditional test case generation, even when driven by fast generative AI prompts, often simply scales these requirement gaps by producing plausible-looking test cases derived from incomplete logic.

eMBT addresses this by making system behaviour explicit early in the lifecycle, enabling teams to:

- **Surface implicit requirements** and clarify edge cases before implementation
- **Eliminate hidden assumptions** between business analysts, developers, and testers
- **Prevent defects early** rather than managing bugs late in production
- **Establish true shared understanding** across all stakeholders
- **Generate systematic, reproducible tests** directly from validated behavioural logic

TestCompass supports this approach by providing a modelling environment that is simple and intuitive enough for business stakeholders to review, while remaining formal and precise enough for automated test derivation.

➡️ **Learn more:** [The eMBT Approach](eMBT-approach.md)

---

## The Philosophy of early Model-Based Testing (eMBT)

When people hear "Model-Based Testing," they often think of technical test generation at the end of a sprint. eMBT takes a fundamentally different, collaborative perspective. 

Rather than treating models as technical input for automated scripts alone, eMBT positions explicit models as **shared thinking tools** for the entire team. 

- **Collaboration First:** The model acts as a bridge during refinement and "Three Amigos" sessions, helping business analysts, developers and testers speak the exact same language.
- **Clarity Before Code:** By visualizing workflows before development starts, teams uncover misunderstandings when they are still cheap and easy to fix.
- **Understanding Over Output:** Test generation is a natural consequence of a validated model, but the true value lies in the conversations and shared insights that happen *while building the model*.

> **Key Takeaway**  
> eMBT is not just a test design technique; it is a collaborative mindset that makes thinking visible early, ensuring teams build the right thing from day one.

---

## What TestCompass Provides

TestCompass offers a complete end-to-end workflow for early Model-Based Testing:

- **Explicit Behavioural Modelling:** Create clear, structured models that represent system logic, decisions, and state transitions using formal TestCompass model rules.
- **AI-Assisted Capabilities:** 
  - **AAMC (AI-Assisted Model Creation):** Jumpstart models directly from raw text, user stories, Excel decision tables, or legacy diagrams (Visio, Lucidchart).
  - **AAMR (AI-Assisted Model Reflection):** Engage in a structured 3-question reflection loop to uncover blind spots and project accepted ideas directly onto the canvas as grey balloon nodes.
- **Automated Test Generation:** Derive test scenarios automatically based on formal coverage strategies, from basic node coverage up to full path coverage.
- **Impact Analysis:** Automatically detect added, removed, updated, and unchanged test scenarios whenever requirements or models evolve.
- **Open Standards & Interoperability:** Import and export Mermaid diagrams, JSON, and Gherkin scenarios for version control, documentation, and seamless pipeline integration.
- **Tooling Integration:** Connect directly with Azure DevOps, Jira, Zephyr, Xray, and other test management environments.

---

## How TestCompass Fits into the Delivery Workflow

TestCompass is designed to integrate naturally into modern, iterative agile workflows:

- Fits seamlessly into version-controlled repositories and continuous documentation setup
- Encourages early collaboration during refinement, "Three Amigos" sessions, and BDD discussions
- Supports a genuine "Shift-Left" quality culture by validating specifications before coding begins
- Produces maintainable, reviewable artefacts that maintain full traceability to requirements

The result is a unified understanding of system behaviour, reducing costly rework, eliminating false confidence and protecting business value.

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

*(Note: This documentation focuses on methodologies, architecture, and concepts. It is designed to complement the in-product Quick Start Guide and guided UI tours.)*

---

> **Summary**  
> By bridging the gap between requirements, explicit models, and automated test derivation, TestCompass ensures teams focus on what truly matters: shared understanding, early risk visibility, and confidence in every delivery decision.

---

[← Back to Documentation Index](index.md)

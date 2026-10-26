# TestCompass Documentation

Welcome to the official documentation for **TestCompass**, an early Model-Based Testing (eMBT) platform designed to help teams reason clearly, uncover risks early, and build shared understanding before code is written.

Testing tools are everywhere, but most focus purely on automation or test execution. Few tools help teams think deeply about test design itself: exploring assumptions, uncovering edge cases, and understanding how a system behaves *before* test cases are created. **That is exactly what TestCompass does.**

<p align="center">
  <img src="TestCompass.jpg" alt="TestCompass Platform" width="550" style="border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
</p>

---

> **Core Purpose & Philosophy**  
> Requirements often describe only the happy path. While AI can generate test cases from text in seconds, speed alone cannot replace understanding. If initial requirements miss key business logic, fast test generation simply multiplies those gaps. TestCompass combines practical testing experience with modern AI assistance, focusing on **Intent-Driven early Model-Based Testing**. By capturing true stakeholder intent early, TestCompass turns implicit assumptions into explicit, coverage-driven test suites.

---

## Getting Started

If you are new to TestCompass or early Model-Based Testing, start here:

- **[Overview](overview.md)** — Learn what TestCompass is, why early MBT matters, and how it fits into delivery workflows.
- **[The eMBT Approach](eMBT-approach.md)** — Understand the 4-phase eMBT workflow: Exploratory, Review, Coverage, and Checking.
- **[Quick Start Guide](quick-start-guide.md)** — Step-by-step guidance to get you up and running quickly.

---

## Core Workflow & Modelling

Learn how to build, validate, and reason about explicit behavioural models:

- **[Behavioural Modelling](modelling.md)** — Foundations of flowchart-based modelling, node types, and requirements discovery.
- **[Mermaid Import & Export](mermaid-import-export.md)** — Bi-directional sync between text-based Mermaid diagrams and testable eMBT models.
- **[BDD Discovery & Formulation](bdd-discovery.md)** — BDD requirements discovery and formulation supported by TestCompass.

---

## AI-Assisted Testing

Explore how AI acts as an accelerator and a thinking partner in TestCompass:

- **[AAMC – AI-Assisted Model Creation](aamc.md)** — Draft initial, semantically correct models from plain text, like user stories, spreadsheets, legacy diagrams and structured formats like Mermaid diagrams, JSON, XML, decision tables, etc. in seconds.
- **[AAMR – AI-Assisted Model Reflection](aamr.md)** — Uncover hidden assumptions, missing paths, and risks through interactive, 3-question AI reflection loops.

---

## Test Generation & Impact Analysis

Turn models into systematic test suites and maintain them effortlessly over time:

- **[Test Generation and Coverage](test-generation.md)** — Derive test scenarios automatically based on Node, Edge, Path Pair, Path Triple, and Full Path Coverage.
- **[Impact Analysis](impact-analysis.md)** — Automatically detect Added, Removed, Updated, and Unchanged scenarios as requirements evolve.

---

## Integrations, Export & Security

Connect TestCompass into your daily tools, pipelines, and enterprise compliance requirements:

- **[Export Formats](export-formats.md)** — Overview of Excel (Test Design & Decision Tables), Gherkin (`.feature`), CSV, PNG, and native `.tcmodel` formats.
- **[Integrations](integrations.md)** — How TestCompass works alongside Azure DevOps, Jira, Zephyr, Xray, and other test management tools.
- **[Security & Architecture](security-architecture.md)** — Overview of AWS EU hosting, AES-256 encryption, TLS traffic security, BCP/DRP, and GDPR data disposal procedures.

---

## Example: Beyond the "Happy Path"

Consider a typical workflow: *a user submits an order, payment is authorized, the order is confirmed, and eventually canceled.* 

Written requirements rarely cover all edge cases. Visualizing this workflow in TestCompass immediately surfaces critical edge cases and missing business logic, such as:
- *Can cancellation occur before payment authorization?*
- *What happens if payment authorization is delayed or times out?*
- *What is the exact system state if cancellation fails mid-process?*
- *Is reserved inventory released immediately upon cancellation?*

Addressing these types of questions during refinement turns implicit assumptions into shared knowledge and leads to complete, coverage-based test suites.

---

## Video Tutorials & Visual Guides

Prefer learning by watching? Explore our library of step-by-step video tutorials covering everything from basic model creation to advanced AI reflection and test generation.

- **Watch tutorials on our website:** [Compass Test Services Tutorials](https://www.compass-testservices.com/tutorials/)
- **Watch on YouTube:** [TestCompass YouTube Channel](https://www.youtube.com/@testcompass9513)

*(Tip: You can easily access the Quick Start Guide, these GitHub docs, and tutorials directly inside the TestCompass platform via the **Help menu (?)** in the top navigation bar).*

---

## About the Creator

<img src="Silvio1.PNG" alt="Silvio Cacace - Creator of TestCompass" width="260" align="right" style="margin-left: 20px; margin-bottom: 15px; border-radius: 8px;">

**TestCompass was created by Silvio Cacace**, drawing on over **30 years of practical domain expertise** in software testing, quality engineering, and Model-Based Testing. 

Throughout his career leading test transformations across enterprise environments, Silvio recognized that most defects originate from incomplete specifications and implicit assumptions long before code is written. To address this, he originally pioneered the **DTM methodology and DTM tool**, which served as the foundation for modern test design automation. 

Building on years of practical application and feedback, Silvio evolved DTM into the **early Model-Based Testing (eMBT)** approach and created **TestCompass** as its next-generation platform, making collaborative, risk-driven testing practical for daily agile delivery. 

Today, eMBT is applied in professional corporate environments and incorporated into software engineering programs across various universities.

<br clear="all">

---

> **Summary**  
> Explore the topics above to master **Intent-Driven early Model-Based Testing**, from capturing true stakeholder intent in your first model draft to generating complete, coverage-based test suites.

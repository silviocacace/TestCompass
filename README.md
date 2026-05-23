# TestCompass  
**early Model Based Testing with explicit models, AI assistance and open standards**

TestCompass is a practical early Model Based Testing (eMBT) platform that helps teams reason clearly, uncover risks early and build shared understanding before development begins.
It brings explicit behavioural modelling and AI‑assisted model creation into the earliest stages of development, enabling deep, traceable testing from the start.

---

## Overview

TestCompass provides a complete workflow for early Model‑Based Testing (eMBT) and BDD, enabling teams to explore behaviour collaboratively, identify risks early and generate reproducible tests from well‑structured models.
It supports open, text‑based modelling formats — including Mermaid, JSON, XML, UML and other industry‑standard formats — and integrates naturally with version‑controlled development workflows.

TestCompass connects seamlessly with tools such as Azure DevOps and Jira, making early modelling and traceable testing part of the everyday delivery process.

---

## early Model-Based Testing (eMBT)

early Model-Based Testing (eMBT) is a collaborative, model‑driven approach that helps teams clarify behaviour early, reduce ambiguity, and design tests systematically.  
It structures the modelling and testing workflow into four iterative phases — Exploratory, Review, Coverage, and Checking — each focused on making behaviour explicit and improving shared understanding.

➡️ Full explanation: [eMBT Overview](eMBT/README.md)

---

## Core Capabilities

- **Explicit behavioural modelling**  
- **AI-Assisted Model Creation (AAMC)**  
- **AI-Assisted Model Reflection (AAMR)**  
- **Automatic test scenario generation**  
- **Multiple test coverage strategies**  
- **Impact analysis on model changes**  
- **Mermaid import and export**  
- **Extensive export and integration options**

---

## AI Features

### AI‑Assisted Model Creation (AAMC)
AAMC generates an initial, semantically consistent model draft from requirements, user stories, or scenarios.  
It accelerates modelling while keeping the tester fully in control.

➡️ Full documentation: [AAMC](AAMC/README.md)

### AI‑Assisted Model Reflection (AAMR)
AAMR analyses a model and asks targeted, context‑aware questions that uncover assumptions, highlight risks, and strengthen the clarity of the behaviour.  
It acts as a thinking partner that supports critical reasoning and early discovery.

➡️ Full documentation: [AAMR](AAMR/README.md)

---

## Test Generation & Coverage

TestCompass generates test scenarios directly from the model using multiple coverage strategies:

- Node Coverage (NC)  
- Edge Coverage (EC) 
- Path Pair Coverage (PPC)  
- Path Triple Coverage (PTC)  
- Full Path Coverage (FPC) 

Export options include:

- Excel test design  
- Excel decision tables  
- Gherkin feature files  
- .CSV for TMS's, like Jira, Azure DevOps, etc

---

## Impact Analysis

When requirements or behaviour change, TestCompass identifies:

- which parts of the model are affected  
- which test scenarios become obsolete  
- which scenarios remain valid  
- what needs to be updated  

This reduces maintenance effort and supports continuous testing.

---

## Import / Export & Integrations

### Mermaid Import & Export
- Import Mermaid diagrams and convert them into testable models  
- Export any model back to Mermaid for documentation, version control, or collaboration  

### Integrations
TestCompass integrates with:

- Azure DevOps  
- Jira  
- Zephyr  
- Xray
- QMetry
- Other test management platforms  

---

## Example Mermaid Model

(Example model omitted here for readability — see repository for full version.)

---

## Repository Contents

- Documentation for AAMC and AAMR  
- Mermaid examples  
- Import/export explanation  
- Background on the eMBT approach  
- Example generated test scenarios  

---

## Purpose of this Repository
This repository contains public documentation, examples, and conceptual material related to TestCompass, AAMC, AAMR, and the eMBT approach.  
It does not contain the TestCompass source code.

---

## Contact

For more information about TestCompass or AI-assisted modelling:

- Website: https://www.testcompass.com  
- LinkedIn: https://www.linkedin.com/in/silviocacace/

---

## Documentation

- [Overview](docs/overview.md)  
- [Modelling](docs/modelling.md)  
- [Test Generation](docs/test-generation.md)  
- [Impact Analysis](docs/impact-analysis.md)  
- [Integrations](docs/integrations.md)  
- [Export Formats](docs/export-formats.md)

---

**Happy Testing!** 🧪

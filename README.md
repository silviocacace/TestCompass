# TestCompass  
**Early Model-Based Testing with explicit models, AI assistance, and open standards**

TestCompass is a practical early Model-Based Testing (eMBT) platform that helps teams reason clearly, uncover risks early, and build shared understanding before development begins.  
It combines explicit behavioural modelling, AI-assisted model creation and reflection, and open, text-based modelling through Mermaid to support deep, traceable testing from the very start.

---

## Overview

TestCompass supports teams that want to move beyond assumptions and make behaviour explicit.  
It provides a complete workflow for early Model-Based Testing (eMBT) and BDD, enabling teams to explore behaviour, identify risks early, and generate reproducible tests based on well‑structured models.

The platform fits naturally into modern, version-controlled development practices and integrates with widely used tools such as Azure DevOps and Jira.

---

## early Model-Based Testing (eMBT)

early Model-Based Testing (eMBT) is a collaborative, model‑driven approach that helps teams clarify behaviour early, reduce ambiguity, and design tests systematically.  
It structures the modelling and testing workflow into four iterative phases — Exploratory, Review, Coverage, and Checking — each focused on making behaviour explicit and improving shared understanding before development begins.

eMBT is the foundation of the TestCompass workflow and is fully supported by the platform’s modelling, AI‑assistance, test generation, and impact analysis capabilities.

➡️ Full explanation: [eMBT Overview](eMBT/README.md)

---

## Core Capabilities

TestCompass offers a comprehensive set of capabilities for early MBT:

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

### AI-Assisted Model Reflection (AAMR)
AAMR analyses your model and asks targeted, context-aware questions to uncover assumptions, identify risks, and strengthen the model.  
It acts as a thinking partner that supports critical reasoning and early discovery.

### AI-Assisted Model Creation (AAMC)
AAMC generates a first, semantically consistent model draft based on requirements, user stories, or scenarios.  
It accelerates modelling while keeping the tester fully in control.

---

### AI‑Assisted Model Reflection (AAMR)

AAMR analyses a model and asks targeted, context‑aware questions that uncover assumptions, highlight risks, and strengthen the clarity of the behaviour.  
It acts as a thinking partner that supports critical reasoning and early discovery without taking over the modelling process.

➡️ Full documentation: [AAMR](AAMR/README.md)

---

### AI‑Assisted Model Creation (AAMC)

AAMC generates an initial, semantically consistent model draft from requirements, user stories, or scenarios.  
It accelerates the modelling process while keeping the tester fully in control, ensuring that behaviour remains explicit and aligned with the team’s understanding.

➡️ Full documentation: [AAMC](AAMC/README.md)


## Test Generation & Coverage

TestCompass generates test scenarios directly from the model using multiple coverage strategies:

- All paths  
- Unique paths  
- Minimal path set  
- Decision coverage  
- Boundary-oriented coverage  
- Custom coverage constraints  

Generated scenarios can be exported to:

- Excel test design  
- Excel decision tables  
- Gherkin feature files  
- CSV  

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
- Other test management platforms  

---

## Example Mermaid Model

---
title: "3.5 Hardware store (Phase Cover-physical)"
---
flowchart TB
    node_1@{shape: circle, label: "Start"}
    node_2@{shape: event, label: "Buy at Hardware Store"}
    node_4@{shape: decision, label: "Total #gt; 200 euro?"}
    node_5@{shape: decision, label: "Total #gt; 1000 euro?"}
    node_6@{shape: decision, label: "Total = 200 euro?"}
    node_7@{shape: decision, label: "Total = 1000 euro?"}
    node_8@{shape: decision, label: "In buy #gt; 30 screwdrivers?"}
    node_9@{shape: document, label: "Discount = 30%"}
    node_12@{shape: decision, label: "In buy 30 screwdrivers?"}
    node_13@{shape: document, label: "Discount 24%"}
    node_14@{shape: decision, label: "In buy #gt; 30 screwdrivers?"}
    node_15@{shape: document, label: "Discount = 14%"}
    node_18@{shape: decision, label: "In buy 30 screwdrivers?"}
    node_19@{shape: document, label: "Discount 4%"}
    node_20@{shape: event, label: "In buy #lt; 30 screwdrivers"}
    node_21@{shape: event, label: "In buy #lt; 30 screwdrivers"}
    node_22@{shape: event, label: "Total #gt; 200 and #lt;1000."}
    node_25@{shape: document, label: "Discount = 0%"}
    node_37@{shape: event, label: "Total #lt; 200 euro"}
    node_38@{shape: document, label: "Not possible to include #gt; 30 screwdrivers"}
    node_39@{shape: double-circle, label: "End"}
    node_41@{shape: decision, label: "In buy 30 screwdrivers?"}
    node_42@{shape: event, label: "In buy #lt; 30 screwdrivers."}
    node_43@{shape: document, label: "Discount 4%"}
    node_44@{shape: decision, label: "In buy #gt; 30 screwdrivers?"}
    node_45@{shape: document, label: "Discount = 14%"}
    node_4-- No --> node_6
    node_5 -- Yes --> node_8
    node_8 -- Yes --> node_9
    node_5-- No --> node_7
    node_8-- No --> node_12
    node_12 -- Yes --> node_13
    node_14 -- Yes --> node_15
    node_14-- No --> node_18
    node_18 -- Yes --> node_19
    node_7 -- Yes --> node_14
    node_12-- No --> node_20
    node_18-- No --> node_21
    node_21 --> node_19
    node_7-- No --> node_22
    node_6-- No --> node_37
    node_6 -- Yes --> node_38
    node_19 --> node_39
    node_15 --> node_39
    node_13 --> node_39
    node_41-- No --> node_42
    node_42 --> node_43
    node_22 --> node_44
    node_44-- No --> node_41
    node_45 --> node_39
    node_41 -- Yes --> node_43
    node_44 -- Yes --> node_45
    node_43 --> node_39
    node_25 --> node_39
    node_38 --> node_25
    node_37 --> node_38
    node_2 --> node_4
    node_4 -- Yes --> node_5
    node_9 --> node_39
    node_20 --> node_13
    node_1 --> node_2

---

## Repository Contents

This repository contains:

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

## 💬 Contact

For more information about TestCompass or AI-assisted modelling, please reach out via the website or LinkedIn.
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

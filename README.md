# TestCompass

**Intent-driven early Model-Based Testing with explicit models, AI assistance and tool integration**

TestCompass is a practical early Model-Based Testing (eMBT) platform that helps teams make intent explicit, clarify expected behaviour, uncover risks early and build shared understanding before development begins.

It brings explicit behavioural modelling and AI-assisted model creation into the earliest stages of development, enabling deep, traceable testing from the start.

<p align="center">
  <img src="docs/TestCompass.jpg" alt="TestCompass Platform" width="550">
</p>

> **Core Purpose**  
> TestCompass bridges the gap between requirements, explicit behavioural models, AI-assisted reasoning, and automated test generation—helping teams build the right thing and build it right from day one.

---

## Documentation

**Full Documentation Site:**  
[https://silviocacace.github.io/TestCompass/](https://silviocacace.github.io/TestCompass/)

**Quick Start Guide:**  
Available directly inside TestCompass via the Help menu and the Book icon.

---

## Overview

TestCompass provides a complete workflow for early Model-Based Testing (eMBT) and BDD, enabling teams to explore behaviour collaboratively, identify risks early, and generate reproducible tests from well-structured models.

Built upon **more than 30 years of practical domain expertise** in software testing and quality engineering, eMBT is a proven methodology widely applied in enterprise practice, embedded in professional testing frameworks, and taught across software engineering curricula at various universities.

It supports open, text-based modelling formats—including Mermaid, JSON, XML, UML, and other industry-standard formats—and integrates naturally with version-controlled development workflows and platforms such as Azure DevOps and Jira, making early modelling and traceable testing part of the everyday delivery process.

---

## Intent-Driven Testing

Effective testing starts with understanding intent: what a system is supposed to achieve and how it is expected to behave.

TestCompass helps teams translate requirements, user stories, and scenarios into explicit behavioural models. These models make assumptions, alternative behaviours, and potential risks visible, providing a shared foundation for systematic test generation and review.

By connecting intent to models and tests, TestCompass helps teams move from ambiguous requirements to behaviour that can be systematically explored and verified.

---

## Early Model-Based Testing (eMBT)

Early Model-Based Testing (eMBT) is a collaborative, model-driven approach that helps teams clarify behaviour early, reduce ambiguity, and design tests systematically.  
It structures the modelling and testing workflow into four iterative phases—Exploratory, Review, Coverage, and Checking—each focused on making behaviour explicit and improving shared understanding.

➡️ **Learn more:** [The eMBT Approach](docs/eMBT-approach.md)

---

## Core Capabilities

- **Explicit behavioural modelling** — Clear, structured flowcharts defining decisions and system paths.  
- **AI-Assisted Model Creation (AAMC)** — Rapid drafting of initial models from stories and requirements.  
- **AI-Assisted Model Reflection (AAMR)** — Context-aware questioning to uncover implicit assumptions and risks.  
- **Automatic test scenario generation** — Systematic derivation of test paths based on formal coverage goals.  
- **Multiple test coverage strategies** — From lightweight Node Coverage (NC) to Full Path Coverage (FPC).  
- **Impact analysis on model changes** — Automatic status tagging for Added, Removed, Updated, and Unchanged tests.  
- **Mermaid import and export** — Bi-directional sync with Git-friendly Markdown diagrams.  
- **Extensive export and integration options** — Seamless connection to Excel, Gherkin, CSV, Jira, Azure DevOps, and Zephyr.  

---

## AI Features

### AI-Assisted Model Creation (AAMC)
AAMC generates an initial, semantically consistent model draft from requirements, user stories, or scenarios.  
It accelerates modelling while keeping the tester fully in control.

➡️ **Full documentation:** [AAMC – AI-Assisted Model Creation](docs/aamc.md)

### AI-Assisted Model Reflection (AAMR)
AAMR analyses a model and asks targeted, context-aware questions that uncover assumptions, highlight risks, and strengthen the clarity of the behaviour.  
It acts as a thinking partner that supports critical reasoning and early discovery.

➡️ **Full documentation:** [AAMR – AI-Assisted Model Reflection](docs/aamr.md)

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
- Gherkin feature files (`.feature`)  
- CSV for Test Management Systems (Jira, Azure DevOps, Zephyr, Xray, etc.)  

➡️ **Full documentation:** [Test Generation and Coverage](docs/test-generation.md)

---

## Impact Analysis

When requirements or behaviour change, TestCompass identifies:

- which parts of the model are affected  
- which test scenarios become obsolete  
- which scenarios remain valid  
- what needs to be updated  

This reduces maintenance effort and supports continuous testing.

➡️ **Full documentation:** [Impact Analysis](docs/impact-analysis.md)

---

## Import / Export & Integrations

### Mermaid Import & Export
- Import Mermaid diagrams and convert them into testable models  
- Export any model back to Mermaid for documentation, version control, or collaboration  

➡️ **Full documentation:** [Mermaid Import and Export](docs/mermaid-import-export.md)

### Integrations
TestCompass integrates conceptually and practically with:
- Azure DevOps  
- Jira (including Zephyr & Xray)  
- QMetry  
- Other test management platforms supporting CSV or Gherkin  

➡️ **Full documentation:** [Integrations](docs/integrations.md) | [Export Formats](docs/export-formats.md)

---

## Repository Contents

- Documentation for AAMC and AAMR  
- Mermaid examples and guides  
- Import/export explanations  
- Background on the eMBT approach  
- Example models and generated test scenarios  

---

## Purpose of this Repository
This repository contains public documentation, examples, and conceptual material related to TestCompass, AAMC, AAMR, and the eMBT approach.  
It does not contain the TestCompass source code.

---

## Documentation Index

- [Overview](docs/overview.md)  
- [The eMBT Approach](docs/eMBT-approach.md)  
- [Behavioural Modelling](docs/modelling.md)  
- [Test Generation and Coverage](docs/test-generation.md)  
- [Impact Analysis](docs/impact-analysis.md)  
- [Integrations](docs/integrations.md)  
- [Export Formats](docs/export-formats.md)  
- [AAMC – AI-Assisted Model Creation](docs/aamc.md)  
- [AAMR – AI-Assisted Model Reflection](docs/aamr.md)  
- [Mermaid Import and Export](docs/mermaid-import-export.md)  

---

## About the Creator & The Origin of eMBT

<img src="docs/Silvio1.PNG" alt="Silvio Cacace - Creator of TestCompass" width="180" align="right" style="margin-left: 20px; margin-bottom: 15px; border-radius: 8px;">

**TestCompass was created by Silvio Cacace**, bringing over **30 years of practical domain expertise** in software testing, quality engineering, and Model-Based Testing. 

Throughout three decades of leading test transformations across enterprise environments, Silvio recognized that most software defects stem from incomplete specifications and implicit assumptions long before code is written. To bridge the gap between complex requirements and clear test coverage, he established the **early Model-Based Testing (eMBT)** methodology and created **TestCompass** to bring this collaborative approach into daily agile delivery.

<br clear="all">

---

## Contact

For more information about TestCompass or AI-assisted modelling:

- **Website:** [www.compass-testservices.com](https://www.compass-testservices.com)  
- **LinkedIn:** [Silvio Cacace](https://www.linkedin.com/in/silviocacace/)  

---

> **Key Takeaway**  
> TestCompass turns early behavioural models into actionable test intelligence—keeping your models, tests, and team fully aligned as software evolves.

**Happy Testing!** 🧪

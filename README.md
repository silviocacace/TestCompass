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

### AI-Assisted Model Creation (AAMC)
AAMC generates a first, semantically consistent model draft based on requirements, user stories, or scenarios.  
It accelerates modelling while keeping the tester fully in control.

### AI-Assisted Model Reflection (AAMR)
AAMR analyses your model and asks targeted, context-aware questions to uncover assumptions, identify risks, and strengthen the model.  
It acts as a thinking partner that supports critical reasoning and early discovery.

---

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

```mermaid
flowchart TD
    Start --> Login
    Login --> Dashboard
    Dashboard --> Logout

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

**Happy Testing!** 🧪

[← Back to Documentation Index](index.md)

# early Model-Based Testing (eMBT)

'early Model-Based Testing' (eMBT) is a collaborative, model-driven testing approach that helps teams achieve a shared understanding of requirements early in the software development lifecycle. It does much more than simply optimize or accelerate test design: eMBT actively stimulates critical thinking and communication between business and technical stakeholders. The earlier misunderstandings, ambiguities, or missing details are discovered, the more effectively teams can prevent costly defects later.

---

> 💡 **Why Intent-Driven eMBT Matters**  
> Traditional testing often validates *what is written* in specifications, regardless of whether those requirements miss the mark. **Intent-Driven eMBT** supported by TestCompass ensures teams uncover and validate *what was actually intended* by business stakeholders. By visually modelling system behaviour during early design, you don't just capture specifications, you actively explore them. In doing so, you uncover risks, open ends, wrong assumptions, contradictions and test ideas at an early stage, forcing a true shared understanding before a single line of code is written.  
>   
> *That’s how you shift from a late 'QA' stamp of approval to driving real customer value right from the start.*

---

## The Philosophy of early Model-Based Testing (eMBT)

When people hear "Model-Based Testing," they often think of technical test generation at the end of a sprint. eMBT takes a fundamentally different, collaborative perspective. 

Rather than treating models as technical input for automated scripts alone, eMBT positions explicit models as **shared thinking tools** for the entire team. 

- **Collaboration First:** The model acts as a bridge during refinement and "Three Amigos" sessions, helping business analysts, developers and testers speak the exact same language.
- **Clarity Before Code:** By visualizing workflows and intent before development starts, teams uncover misunderstandings when they are still cheap and easy to fix.
- **Intent Over Output:** Test generation is a natural consequence of a validated model, but the true value lies in revealing true stakeholder intent and capturing shared insights *while building the model*.

> **Key Takeaway**  
> eMBT is not just a test design technique; it is an Intent-Driven collaborative mindset that makes thinking visible early, ensuring teams build the right thing from day one.

---

## The Four Iterative Phases of eMBT

eMBT structures the testing workflow into four iterative phases:

<p align="center">
  <img src="eMBT_phases.jpg" alt="The 4 Iterative Phases of eMBT" width="550">
</p>

---

### 1. Exploratory Phase
In this phase, the team explores and visualizes the requirements and underlying intent.  
The goal is to make behaviour explicit and identify:

- ambiguities and missing specifications  
- inconsistencies in business rules  
- open ends and unhandled scenarios  
- hidden assumptions between business and IT  
- potential risks and test ideas  

A graphical test model is created directly in TestCompass as a shared thinking tool. Teams can also conduct collaborative discovery directly on the canvas using interactive **Sticky Note nodes** for Feature and Example Mapping, or leverage **AI-Assisted Model Creation (AAMC)** to draft test models in seconds.

*(See: [BDD Requirements Discovery](bdd-discovery.md))*

---

### 2. Review Phase
All questions, open ends, uncertainties, etc raised during the exploratory phase are reviewed with the full team.  
Business and IT validate:

- the true meaning and **intent** of requirements  
- business rules and decision logic  
- boundary conditions and edge cases  
- exception paths and risk scenarios  

TestCompass enhances this phase with **AAMR (AI-Assisted Model Reflection)**, acting as an interactive thinking partner to challenge assumptions and surface hidden gaps. Every requirement change or newly discovered risk leads to an updated model and a brief review cycle.

---

### 3. Coverage Phase
Once the model is validated, test scenarios and specifications are automatically derived based on the selected mathematical coverage strategy.

The following coverage levels are available:

- **Node coverage (NC)** — Covers all actions, decisions and results at least once  
- **Edge coverage (EC)** — Covers all transitions (Yes/No branches)  
- **Path Pair coverage (PPC)** — Covers combinations of two consecutive decision branches  
- **Path Triple coverage (PTC)** — Covers combinations of three consecutive decision branches  
- **Full Path coverage (FPC)** — Covers all possible end-to-end paths  

By defining test data, preconditions, and expected predictions within node details, TestCompass automatically derives both **Data-Driven Gherkin Scenario Outlines** (when modelling for BDD) and concrete, **Physical Test Scenarios** complete with test data matrices for Excel Test Design and Decision Tables.

---

### 4. Checking Phase
The generated coverage-based test scenarios are passed to execution frameworks and test management environments (executed manually, via automated scripts, or a combination of both). 

While TestCompass focuses on **modelling and systematic test design**, it seamlessly aligns with execution by exporting artifacts into tools like Azure DevOps, Jira, Zephyr, Xray, or Gherkin `.feature` files. The goal is to verify that actual system implementation strictly reflects stakeholder intent and to give real-time insight into release readiness.

---

## Impact Analysis

Because requirements change continuously, eMBT includes a structured way to manage change without manual scenario upkeep.  
When the model is updated, an automated impact analysis shows which test scenarios are:

- **Added** (new behaviour introduced)  
- **Removed** (obsolete behaviour)  
- **Updated** (existing path modified)  
- **Unchanged** (remains fully valid)  

This eliminates tedious manual scenario maintenance, prevents drift between specifications and test suites, and keeps quality artifacts 100% synchronized.

---

## Key Benefits of eMBT

eMBT helps teams:

- **Capture true business intent early** and remove ambiguities before development begins
- **Foster shared understanding** and improve collaboration between business and IT
- **Identify risks and missing behaviour sooner**, avoiding hidden assumptions
- **Design coverage-based tests automatically** directly from visual behavioural models
- **Manage change effortlessly** through single-click model updates and automated impact analysis
- **Reduce rework and defects** in production, protecting true business value

---

## Relation to TestCompass

TestCompass supports the complete eMBT lifecycle:

- **In-Tool Discovery & Modelling** *(Exploratory Phase)*  
- **Collaborative Reviewing & AI Reflection** *(Review Phase)*  
- **Automated Test Scenario & Gherkin Generation** *(Coverage Phase)*  
- **Impact Analysis & Test Management Export** *(Checking Phase)*  

In addition, TestCompass provides built-in AI capabilities to enhance reasoning:

- **AAMC (AI-Assisted Model Creation):** Jumpstart modelling from natural language requirements or Mermaid diagrams.  
  ➡️ **Learn more:** [AAMC Documentation](aamc.md)

- **AAMR (AI-Assisted Model Reflection):** Acts as a critical partner to uncover hidden risks, missing logic, and open ends.  
  ➡️ **Learn more:** [AAMR Documentation](aamr.md)

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

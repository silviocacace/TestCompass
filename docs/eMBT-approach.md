[← Back to Documentation Index](index.md)

# 'early Model-Based Testing' (eMBT)

'early Model-Based Testing' (eMBT) is a collaborative, model-driven testing approach that helps teams achieve a shared understanding of requirements early in the software development lifecycle. It does much more than simply optimize or accelerate test design: eMBT actively stimulates critical thinking and communication between business and technical stakeholders. The earlier misunderstandings, ambiguities or missing details are discovered, the more effectively teams can prevent costly defects later.

---

## Why eMBT Matters

This is precisely why 'early Model-Based Testing' (eMBT) supported by TestCompass is so powerful. By visually modelling the intended system behaviour during the initial design phase, you don't just capture specifications. You actively explore them. In doing so, you uncover risks, open ends, wrong assumptions and test ideas in an early stage. It forces a true shared understanding between business and IT before a single line of code is written.

That’s how you shift from a late 'QA' stamp of approval to driving real customer value right from the start.

---

## The Four Iterative Phases of eMBT

eMBT consists of four iterative phases:

---

<img src="eMBT_phases.jpg" alt="Generated TestCompass Model" width="500">

---

## 1. Exploratory Phase
In this phase, the team explores and visualizes the requirements.  
The goal is to identify:

- ambiguities  
- inconsistencies  
- open ends  
- hidden assumptions
- risks
- test ideas
- ... 

A graphical test model is created to make behaviour explicit.  
The model acts as a shared thinking tool that immediately triggers discussion and reveals misunderstandings. The model in TestCompass is readable for all stakeholders.

---

## 2. Review Phase
All questions and uncertainties raised during the exploratory phase are reviewed with the full team.  
Business and IT validate:

- the meaning of the requirements (intent) 
- business rules and decisions  
- boundary conditions  
- exceptions
- risks  

This phase is iterative.  
Every change in the requirements leads to an updated model and a new review cycle.

---

## 3. Coverage Phase
Once the model is complete and validated, test scenarios are automatically generated based on the selected coverage level.

The following coverage forms are available:

- **Node coverage (NC)**  
- **Edge coverage (EC)**  
- **Path Pair coverage (PPC)**  
- **Path Triple coverage (PTC)**  
- **Full Path coverage (FPC)**  

The chosen coverage level depends on risk, priority and desired thoroughness.

---

## 4. Checking Phase
The generated test scenarios are executed against the system under test.  
Depending on the nature of the test, execution may be:

- manual  
- automated  
- or a combination of both  

The goal is to check whether the system-behavior is conform the intent and to gain insight in the quality of the product. With this insight stakeholders can make informed discussions.

---

## Impact Analysis
Because requirements change continuously, eMBT includes a structured way to manage change.  
When the model is updated, an impact analysis can be performed and shows which test scenarios are:

- added  
- removed  
- updated  
- unchanged  

This prevents unnecessary test analysis work and reduces false positives and false negatives.

---

## Key Benefits of eMBT

eMBT helps teams:

- **Clarify requirements early** and remove ambiguities before development begins
- **Foster shared understanding** and improve collaboration between business and IT
- **Identify risks and missing behaviour sooner**, avoiding hidden assumptions
- **Design tests automatically and systematically** directly from behavioural models
- **Manage change effectively** through automated impact analysis
- **Reduce rework and defects** in production, protecting true business value 

---

## Relation to TestCompass

TestCompass supports the full eMBT workflow:

- modelling (Exploratory)  
- reviewing and iteration (Review)  
- automated test generation (Coverage)  
- impact analysis and execution support (Checking)  

In addition, TestCompass provides AI-assistance through:

- **AAMC** – AI-Assisted Model Creation
➡️ **Learn more:**  [AAMC](aamc.md)

- **AAMR** – AI-Assisted Model Reflection
➡️ **Learn more:**  [AAMR](aamr.md)

These capabilities accelerate modelling and improve the quality of reasoning.




[← Back to Documentation Index](index.md)

# Early Model-Based Testing (eMBT)

'Early Model-Based Testing' (eMBT) is a collaborative, model-driven testing approach that helps teams achieve a shared understanding of requirements early in the software development lifecycle. It does much more than simply optimize or accelerate test design: eMBT actively stimulates critical thinking and communication between business and technical stakeholders. The earlier misunderstandings, ambiguities, or missing details are discovered, the more effectively teams can prevent costly defects later.

---

> 💡 **Why eMBT Matters**  
> This is precisely why Early Model-Based Testing (eMBT) supported by TestCompass is so powerful. By visually modelling the intended system behaviour during the initial design phase, you don't just capture specifications—you actively explore them. In doing so, you uncover risks, open ends, wrong assumptions, and test ideas at an early stage. It forces a true shared understanding between business and IT before a single line of code is written.  
>  
> *That’s how you shift from a late 'QA' stamp of approval to driving real customer value right from the start.*

---

## The Four Iterative Phases of eMBT

eMBT structures the testing workflow into four iterative phases:

<p align="center">
  <img src="eMBT_phases.jpg" alt="The 4 Iterative Phases of eMBT" width="550">
</p>

---

### 1. Exploratory Phase
In this phase, the team explores and visualizes the requirements.  
The goal is to make behaviour explicit and identify:

- ambiguities and missing specifications  
- inconsistencies in business rules  
- open ends and unhandled scenarios  
- hidden assumptions between business and IT  
- potential risks and test ideas  

A graphical test model is created directly in TestCompass as a shared thinking tool. Because the model is easy to read for all stakeholders, it immediately triggers valuable discussions and reveals misunderstandings before implementation begins.

---

### 2. Review Phase
All questions, open ends, and uncertainties raised during the exploratory phase are reviewed with the full team.  
Business and IT validate:

- the true meaning and intent of requirements  
- business rules and decision logic  
- boundary conditions and edge cases  
- exception paths and risk scenarios  

This phase is continuous and iterative: every requirement change or newly discovered risk leads to an updated model and a brief review cycle.

---

### 3. Coverage Phase
Once the model is complete and validated, test scenarios are automatically generated based on the selected coverage strategy.

The following coverage forms are available:

- **Node coverage (NC)** — Covers all actions, decisions, and results at least once  
- **Edge coverage (EC)** — Covers all transitions (Yes/No branches)  
- **Path Pair coverage (PPC)** — Covers combinations of two consecutive decision branches  
- **Path Triple coverage (PTC)** — Covers combinations of three consecutive decision branches  
- **Full Path coverage (FPC)** — Covers all possible end-to-end paths  

The chosen coverage level depends on product risk, priority, and desired thoroughness.

---

### 4. Checking Phase
The generated test scenarios are executed against the system under test (manually, automated, or a combination of both).  

The goal is to verify that system behaviour is strictly in line with intent and to gain real-time insight into product quality. With this insight, stakeholders can make confident, informed decisions about release readiness.

---

## Impact Analysis

Because requirements change continuously, eMBT includes a structured way to manage change.  
When the model is updated, an automated impact analysis shows which test scenarios are:

- **Added** (new behaviour introduced)  
- **Removed** (obsolete behaviour)  
- **Updated** (existing path modified)  
- **Unchanged** (remains fully valid)  

This prevents unnecessary manual analysis, keeps test suites maintainable, and reduces false positives and false negatives.

---

## Key Benefits of eMBT

eMBT helps teams:

- **Clarify requirements early** and remove ambiguities before development begins
- **Foster shared understanding** and improve collaboration between business and IT
- **Identify risks and missing behaviour sooner**, avoiding hidden assumptions
- **Design tests automatically and systematically** directly from behavioural models
- **Manage change effectively** through automated impact analysis
- **Reduce rework and defects** in production, protecting true business value

---

## Relation to TestCompass

TestCompass supports the complete eMBT lifecycle:

- **Modelling & Risk Exploration** *(Exploratory Phase)*  
- **Collaborative Reviewing & Iteration** *(Review Phase)*  
- **Automated Test Scenario Generation** *(Coverage Phase)*  
- **Impact Analysis & Execution Support** *(Checking Phase)*  

In addition, TestCompass provides built-in AI capabilities to enhance reasoning:

- ⚡ **AAMC (AI-Assisted Model Creation):** Jumpstart modelling from natural language requirements.  
  ➡️ **Learn more:** [AAMC Documentation](aamc.md)

- 🧐 **AAMR (AI-Assisted Model Reflection):** Acts as a critical partner to uncover hidden risks and open ends.  
  ➡️ **Learn more:** [AAMR Documentation](aamr.md)

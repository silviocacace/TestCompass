[← Back to Documentation Index](index.md)

# early Model-Based Testing (eMBT)

'early Model-Based Testing' (eMBT) is a collaborative, model-driven testing approach that helps teams achieve a shared understanding of requirements early in the software development lifecycle. It does much more than simply optimize or accelerate test design: eMBT actively stimulates critical thinking and communication between business and technical stakeholders. The earlier misunderstandings, ambiguities, or missing details are discovered, the more effectively teams can prevent costly defects later.

---

> 💡 **Why eMBT Matters**  
> This is precisely why early Model-Based Testing (eMBT) supported by TestCompass is so powerful. By visually modelling the intended system behaviour during the initial design phase, you don't just capture specifications—you actively explore them. In doing so, you uncover risks, open ends, wrong assumptions, and test ideas at an early stage. It forces a true shared understanding between business and IT before a single line of code is written.  
>  
> *That’s how you shift from a late 'QA' stamp of approval to driving real customer value right from the start.*

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

-  **AAMC (AI-Assisted Model Creation):** Jumpstart modelling from natural language requirements.  
  ➡️ **Learn more:** [AAMC Documentation](aamc.md)

-  **AAMR (AI-Assisted Model Reflection):** Acts as a critical partner to uncover hidden risks and open ends.  
  ➡️ **Learn more:** [AAMR Documentation](aamr.md)

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**


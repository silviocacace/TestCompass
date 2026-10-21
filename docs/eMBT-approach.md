[← Back to Documentation Index](index.md)

# Early Model-Based Testing (eMBT)

'Early Model-Based Testing' (eMBT) is a collaborative, model-driven testing approach that helps teams achieve a shared understanding of requirements early in the software development lifecycle. It does much more than simply optimize or accelerate test design: eMBT actively stimulates critical thinking and communication between business and technical stakeholders. The earlier misunderstandings, ambiguities, or missing details are discovered, the more effectively teams can prevent costly defects later.

---

## Why eMBT Matters

This is precisely why Early Model-Based Testing (eMBT) supported by TestCompass is so powerful. By visually modelling the intended system behaviour during the initial design phase, you don't just capture specifications—you actively explore them. In doing so, you uncover risks, open ends, wrong assumptions, and test ideas at an early stage. It forces a true shared understanding between business and IT before a single line of code is written.

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

A graphical test model is created to make behaviour explicit.  
The model acts as a shared thinking tool that immediately triggers discussion and reveals misunderstandings.

---

## 2. Review Phase
All questions and uncertainties raised during the exploratory phase are reviewed with the full team.  
Business and IT validate:

- the meaning of the requirements  
- business rules and decisions  
- boundary conditions  
- exceptions  

This phase is iterative.  
Every change in the requirements leads to an updated model and a new review cycle.

---

## 3. Coverage Phase
Once the model is complete and validated, test cases are automatically generated based on the selected coverage level.

The following coverage forms are commonly used:

- **Node coverage (NC)**  
- **Edge coverage (EC)**  
- **Path Pair coverage (PPC)**  
- **Path Triple coverage (PTC)**  
- **Full Path coverage (FPC)**  

The chosen coverage level depends on risk, priority, and desired thoroughness.

---

## 4. Checking Phase
The generated test cases are executed against the system under test.  
Depending on the nature of the test, execution may be:

- manual  
- automated  
- or a combination of both  

The goal is to verify that the system behaves exactly as described in the model.

---

## Impact Analysis
Because requirements change continuously, eMBT includes a structured way to manage change.  
When the model is updated, an impact analysis shows which test cases are:

- added  
- removed  
- updated  
- unchanged  

This prevents unnecessary test work and reduces false positives and false negatives.

---

## Key Benefits of eMBT

eMBT helps teams:

- clarify requirements early  
- reduce misunderstandings  
- identify risks sooner  
- manage change effectively  
- design tests systematically  
- ensure business value is protected  

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

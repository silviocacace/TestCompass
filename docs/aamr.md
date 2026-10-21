[← Back to Documentation Index](index.md)

# AAMR – AI-Assisted Model Reflection

AAMR (AI-Assisted Model Reflection) is an AI-supported capability within TestCompass that helps users critically review and improve existing models.

Rather than generating a model, AAMR analyses a model and presents observations, questions and alternative perspectives that may help identify gaps, ambiguities and potential risks.

AAMR is designed to support reflective thinking while keeping all modelling decisions under the control of the tester.

---

## Purpose

AAMR helps users:

- examine behavioural models from different perspectives
- identify possible gaps or ambiguities
- challenge assumptions
- explore alternative interpretations
- improve model quality and consistency
- support collaborative model reviews

AAMR acts as a modelling partner that encourages critical thinking and discussion.

---

## How AAMR Works

AAMR analyses the structure and semantics of a TestCompass model and generates reflections such as:

- clarification questions
- observations about model structure
- potential ambiguities
- potentially missing behaviour
- alternative interpretations
- risk-oriented discussion points
- model improvement suggestions

The purpose of these reflections is to stimulate analysis and discussion, not to automatically modify the model.

---

## Example Reflections

When analysing a model, AAMR may generate questions such as:

- What happens if this decision evaluates to "No"?
- Is this outcome always valid?
- Can a user return to a previous state?
- Are all exception paths represented?
- Does this process have a defined termination point?
- Could different stakeholders interpret this behaviour differently?

These questions help expose uncertainty and encourage deeper examination of the model.

![TestCompass Node Types and Canvas](AAMR_explanation.png)

---

## Typical Workflow

1. Create or import a model into TestCompass
2. Run AAMR on the model
3. Review the generated reflections and questions
4. Discuss and evaluate the observations
5. Refine the model where necessary
6. Continue with test generation and impact analysis

---

## What AAMR Is Not

AAMR is not:

- an automatic model corrector
- a model generation tool
- a replacement for modelling expertise
- a system that determines the "correct" answer
- a mechanism that automatically changes models

The final modelling decisions always remain with the tester.

---

## Relationship with AAMC

AAMC and AAMR address different stages of the modelling process.

### AAMC (AI-Assisted Model Creation)
AAMC helps create an initial model draft from behavioural descriptions.  
Its primary goal is to accelerate model creation.

### AAMR (AI-Assisted Model Reflection)
AAMR helps review, challenge and strengthen an existing model.  
Its primary goal is to stimulate critical thinking and uncover gaps, ambiguities and potential risks.

Together, AAMC and AAMR support both the creation and continuous improvement of TestCompass models.

---

## Contact

For more information about AAMR or the TestCompass eMBT workflow, please visit the website or reach out via LinkedIn.

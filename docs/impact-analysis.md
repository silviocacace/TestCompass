# Impact Analysis

Impact analysis in TestCompass helps teams understand how changes in requirements affect existing behaviour, models, and generated test scenarios.  
Because requirements evolve continuously, impact analysis ensures that test suites remain accurate, relevant, and aligned with the latest understanding of the system.

This page explains the purpose of impact analysis, how it relates to modelling and test generation, and how TestCompass supports a structured approach to managing change.

---

## Purpose of Impact Analysis

When behaviour changes, the model changes — and therefore the tests must change as well.  
Impact analysis answers four essential questions:

- **What behaviour has been added?**  
- **What behaviour has been removed?**  
- **What behaviour has changed?**  
- **What behaviour remains valid?**

By identifying these differences automatically, TestCompass prevents unnecessary rework and reduces the risk of false positives and false negatives.

---

## How Impact Analysis Works Conceptually

Impact analysis compares two versions of the same model:

1. **The previous version** (before the change)  
2. **The updated version** (after the change)

TestCompass examines:

- structural differences  
- changes in decision logic  
- updated node labels or data  
- added or removed paths  
- modified boundaries or conditions  

Based on this comparison, each generated test scenario receives a status.

---

## Test Scenario Status Types

Each scenario is classified into one of four categories:

### Added
New behaviour has been introduced, resulting in new scenarios.

### Removed
Behaviour no longer exists in the updated model, so the scenario is obsolete.

### Updated
Behaviour still exists, but the path or logic has changed.

### Unchanged
The scenario remains valid and requires no modification.

This classification provides immediate insight into the scope and impact of the change.

---

## Why Impact Analysis Matters

Impact analysis supports:

- **Continuous testing**  
  Tests stay aligned with evolving requirements.

- **Reduced maintenance effort**  
  Only affected scenarios require attention.

- **Traceability**  
  Teams can see exactly why a scenario changed.

- **Risk management**  
  Changes in critical behaviour become visible early.

- **Efficient collaboration**  
  Business and IT can discuss the impact of requirement changes with a shared visual reference.

---

## Relationship to Modelling

Impact analysis is only possible because TestCompass uses explicit behavioural models.  
When the model changes, the impact becomes:

- visible  
- explainable  
- traceable  

➡️ Learn more: **[Modelling](ca://s?q=Open_modelling_documentation)**

---

## Relationship to Test Generation

After running impact analysis, teams can:

- regenerate scenarios  
- update only the affected ones  
- maintain a clean, consistent test suite  

This ensures that generated tests always reflect the latest version of the model.

➡️ Learn more: **[Test Generation](ca://s?q=Open_test_generation_documentation)**

---

Impact analysis ensures that change is not disruptive but manageable — keeping your models, tests, and understanding aligned as the system evolves.

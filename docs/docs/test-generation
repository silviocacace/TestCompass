# Test Generation

Test generation in TestCompass is based on the principle that explicit behavioural models enable systematic, reproducible, and risk‑aligned testing.  
Once a model has been validated and reviewed, TestCompass can automatically generate test scenarios using a selected coverage strategy.

This page explains the conceptual foundations of test generation and describes the coverage forms supported by TestCompass.

---

## Purpose of Test Generation

The goal of test generation is to derive a set of test scenarios that:

- reflect the intended behaviour of the system  
- cover the relevant decisions, paths, and boundaries  
- are reproducible and traceable  
- align with the agreed level of risk and thoroughness  

Because the tests are generated from the model, they remain consistent, structured, and easy to maintain.

---

## Abstract vs. Concrete Test Scenarios

TestCompass distinguishes between two types of scenarios:

- **Abstract test scenarios**  
  Generated directly from the model. They describe the logical flow and help teams understand behaviour, explore ideas, and ask questions.

- **Concrete test scenarios**  
  Created when preconditions, data, or concrete values are added. These scenarios are executable and suitable for manual or automated testing.

This separation ensures clarity: the model defines behaviour, while concrete details are added only when needed.

---

## Coverage Strategies

TestCompass supports multiple coverage strategies, ranging from lightweight to exhaustive.  
Each strategy defines **what must be covered at least once** in the generated test set.

The following coverage forms are available:

### Node Coverage (NC)
Covers **all nodes** in the model at least once.  
Nodes include Action/State, Decision, and Result nodes.  
This is the lightest form of coverage.

### Edge Coverage (EC)
Covers **all edges** in the model at least once.  
Edges represent the transitions between nodes, including Yes/No branches.

### Path Pair Coverage (PPC)
Covers **all combinations of two consecutive test paths**.  
A test path follows the Yes or No branch from a decision node.  
This strategy captures interactions between consecutive decisions.

### Path Triple Coverage (PTC)
Covers **all combinations of three consecutive test paths**.  
Useful when decisions influence each other across multiple steps.

### Full Path Coverage (FPC)
Covers **all possible paths** from Start to End.  
This is the strongest form of coverage and typically produces the largest number of scenarios.

---

## Maximum Number of Test Scenarios

Models may contain loops or complex branching, which can theoretically produce an infinite number of paths.  
To ensure practical generation:

- TestCompass prioritises paths that contribute to coverage  
- Loops are explored in a controlled manner  
- Redundant paths are pruned  
- A configurable maximum number of scenarios is applied  

This ensures that generated scenarios are meaningful, non‑redundant, and aligned with the selected coverage strategy.

---

## Exporting Test Scenarios

Generated test scenarios can be exported to:

- Excel test design  
- Excel decision tables  
- Gherkin feature files  
- CSV  

Exports include:

- node text  
- decision logic  
- expected results  
- preconditions and data (if provided)

➡️ See: **[Export Formats](ca://s?q=Open_export_formats_documentation)**

---

## Relationship to Modelling

The quality of the generated tests depends directly on the quality of the model.  
Clear decisions, explicit boundaries, and well‑defined outcomes lead to stronger and more meaningful test scenarios.

➡️ Learn more: **[Modelling](ca://s?q=Open_modelling_documentation)**

---

## Relationship to Impact Analysis

When requirements change, the model is updated — not the tests.  
Impact analysis identifies which scenarios are:

- added  
- removed  
- updated  
- unchanged  

This keeps test suites aligned with evolving behaviour.

➡️ Learn more: **[Impact Analysis](ca://s?q=Open_impact_analysis_documentation)**

---

Test generation in TestCompass ensures that testing is systematic, transparent, and grounded in explicit behavioural understanding — not assumptions.

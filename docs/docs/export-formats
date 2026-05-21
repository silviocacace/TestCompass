# Export Formats

TestCompass supports several export formats to ensure that generated test scenarios can be used across different teams, tools, and workflows.  
All exports are based on explicit behavioural models, ensuring that the resulting artefacts are structured, traceable, and aligned with the intended behaviour.

This page describes the available export formats and their conceptual purpose.

---

## Purpose of Exporting

Exporting allows teams to:

- use generated scenarios in external test management tools  
- collaborate using familiar formats (Excel, CSV, Gherkin)  
- support both manual and automated testing  
- maintain traceability between models and execution artefacts  
- integrate early MBT into existing pipelines  

Exports are always derived from the model and the selected coverage strategy.

---

## Available Export Formats

### Excel Test Design
A structured test design containing:

- test scenario steps  
- decision logic  
- expected results  
- preconditions and test data (if provided in the model)  

This format is ideal for manual testing or documentation-heavy environments.

---

### Excel Decision Table
A tabular representation of decision logic, suitable for:

- business rule validation  
- regulatory or audit contexts  
- teams that prefer decision tables over flow-based models  

Override labels from the model are included when provided.

---

### Gherkin Feature Files
TestCompass can generate `.feature` files containing:

- Feature  
- Background (optional)  
- Rule (optional)  
- Given / When / Then sequences  
- Examples (if defined in the model)  

This format supports BDD workflows and integrates with tools such as:

- Cucumber  
- SpecFlow  
- Behave  
- Xray (via feature file import)

The generated feature files reflect the selected test coverage.

---

### CSV Export
A generic export format suitable for:

- Jira  
- Zephyr  
- Xray  
- QMetry  
- Azure DevOps  
- Other test management tools  

CSV exports contain structured scenario information that can be mapped to fields in external systems.

---

## Relationship to Test Generation

All export formats are generated from the same underlying model and coverage strategy.  
This ensures consistency across:

- Excel test designs  
- decision tables  
- Gherkin files  
- CSV imports  

➡️ Learn more: [Test Generation](test-generation.md)

---

## Relationship to Integrations

Export formats are designed to map cleanly to external tools.  
Each integration relies on one or more export formats to transfer structured test artefacts.

➡️ Learn more: [Integrations](integrations.md)

---

Export formats ensure that TestCompass fits naturally into diverse workflows, enabling teams to use model-based scenarios wherever they execute or manage tests.


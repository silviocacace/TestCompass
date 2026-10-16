# Export Formats

TestCompass transforms explicit behavioural models into structured test scenarios that can be reviewed, shared and used in different testing workflows.

This page provides an overview of the available export formats and their intended use.

## Test Design and Test Management Exports

### Excel — Test Design

Export generated test scenarios to Excel for review, refinement and execution.

Excel provides a familiar, structured format for teams that want to inspect generated scenarios, collaborate on test design and document test cases.

**Typical use cases:**
- Reviewing generated test scenarios
- Refining test cases before execution
- Sharing test designs with business analysts, testers and stakeholders

### Excel — Decision Tables

Export decision tables to Excel to structure conditions, combinations and expected outcomes.

Decision tables help teams analyse complex business rules and review combinations of inputs and expected results systematically.

**Typical use cases:**
- Reviewing business rules
- Analysing combinations of conditions
- Supporting systematic test design

### Gherkin — `.feature`

Export test scenarios as Gherkin feature files using the Given/When/Then structure.

Gherkin is commonly used in Behaviour-Driven Development (BDD) to express expected behaviour in a structured, readable format.

**Typical use cases:**
- BDD workflows
- Collaboration between business stakeholders, testers and developers
- Preparing scenarios for compatible BDD automation tools

### CSV — `.csv`

Export test scenarios as CSV files for data exchange with supported test management systems and other tools.

CSV is a widely supported tabular format. Depending on the target system, the exported data may need to be mapped to the required fields or adapted to the import template.

**Typical use cases:**
- Preparing test cases for import into test management systems
- Transferring structured test data between tools
- Further processing in spreadsheets or scripts

Compatibility depends on the target tool's import capabilities and the structure it requires.

## Model Import and Export

### Mermaid

TestCompass supports Mermaid import and export for visualising, sharing and documenting behavioural models.

Mermaid represents diagrams as text, making models easier to review, version and share alongside other project documentation.

**Typical use cases:**
- Sharing behavioural models with team members
- Including diagrams in Markdown documentation
- Reviewing model changes in version control

For details, see [Mermaid Import & Export](Mermaid%20Import%20%26%20Export.md).

## Choosing the Right Format

| Format | Primary purpose |
|---|---|
| Excel — Test Design | Reviewing and refining test scenarios |
| Excel — Decision Tables | Analysing business rules and condition combinations |
| Gherkin | Describing scenarios in BDD format |
| CSV | Exchanging structured test data |
| Mermaid | Sharing and documenting behavioural models |

## Exporting and Traceability

TestCompass derives test scenarios from explicit behavioural models. This provides a structured relationship between modelled behaviour and the tests generated from it.

When choosing an export format, consider the intended audience, the next step in your testing workflow and the requirements of the target tool.

For more information, see:
- [Test Generation and Coverage](test-generation.md)
- [Impact Analysis](impact-analysis.md)
- [Integrations](integrations.md)


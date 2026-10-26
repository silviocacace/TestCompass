[← Back to Documentation Index](index.md)

# Mermaid Import & Export

Mermaid import and export in TestCompass help teams exchange models across documentation, development, and quality engineering workflows. Because Mermaid is an open, text-based notation, it supports transparent collaboration, version control, and clear code reviews in Git.

> **Core Purpose**  
> Mermaid serves as a text-based interchange format, enabling teams to embed visual models in documentation and track version changes in Git while maintaining rigorous, coverage-ready eMBT semantics.

This page explains the purpose of Mermaid import and export, how they relate to behavioural modelling, and how TestCompass ensures consistency between text-based diagrams and executable eMBT test models.

---

## Purpose of Mermaid Import & Export

Mermaid import and export enable teams to:

- **Protect and reuse existing assets:** easily convert legacy process models from Visio, BPMN tools, Lucidchart, and Draw.io into Mermaid syntax and import them directly into TestCompass.
- **Include models directly in documentation:** seamlessly render behavioural models within Markdown files, wikis, and GitHub or GitLab repository documentation.
- **Maintain version control in Git:** store models as plain-text files with clean, readable line-by-line diffs during pull requests and code reviews.
- **Reconstruct and evolve models:** convert text-based Mermaid code back into fully interactive, testable TestCompass visual models at any time.
- **Maintain single-source consistency:** keep system behavior synchronized across Product Owners, Developers, and QA Engineers.

By supporting Mermaid as an interchange format, TestCompass eliminates manual re-keying of existing process flows, improves traceability, and bridges the gap between system design, documentation, and automated test derivation.

---

## Import: From Text Diagram to Testable Model

When importing a Mermaid diagram, TestCompass automatically converts the diagram into a structured eMBT model. During import, TestCompass:

- interprets nodes and transitions according to explicit eMBT semantics
- validates the model structure and highlights logical inconsistencies
- preserves incomplete or ambiguous paths for review
- prevents hidden logic or implicit decision branches from being introduced

If a source Mermaid diagram uses unsupported syntax or breaks eMBT structural rules, clear guidance is provided so the diagram can be adjusted for test generation.

*(Tip: You can also use **AAMC – AI-Assisted Model Creation** to automatically generate or fix Mermaid diagrams from raw user stories before importing).*

---

## Export: From Model to Living Documentation

When exporting a model, TestCompass generates Mermaid syntax that reflects the exact structure and semantics of the underlying visual eMBT model. The exported Mermaid code:

- is deterministic and optimized for version control in Git
- can be embedded directly in `README.md` files, wikis, and architecture design documents
- provides a human-readable, visual view of system intent for non-modelling stakeholders
- maintains full structural alignment with the underlying TestCompass model

Exported diagrams support ongoing communication and traceability, while the TestCompass model remains the authoritative source for **coverage calculation, Gherkin generation, Excel Test Design, and impact analysis**.

---

## Relationship to Modelling & eMBT Workflow

Mermaid import and export complement the core TestCompass modelling workflow. They make system behaviour visible across documentation repositories, while TestCompass ensures that the model itself remains:

- **Explicit:** every decision branch (`Yes`/`No`) and outcome is clearly defined.
- **Semantically Correct:** ready for mathematical coverage strategies (Node, Edge, Path Pair, Path Triple, Full Path Coverage).
- **Traceable:** linked to stakeholder intent, preconditions, and test data variations.
- **Maintainable:** supported by automated impact analysis when requirements change.

---

## AI-Assisted Mermaid Conversion (James Bach Skill)

While TestCompass supports standard Mermaid imports, not every valid diagram can be converted directly into a testable eMBT model. TestCompass enforces specific modelling rules to guarantee that mathematical graph coverage algorithms can generate valid test paths.

To support this conversion process, James Bach created a Claude Code skill that analyses Mermaid diagrams, identifies conflicts with TestCompass modelling rules, and assists in producing a fully compatible eMBT model syntax.

This community-contributed resource is particularly useful when adapting complex legacy diagrams or external Mermaid definitions for import into TestCompass.

🔗 **[Download James Bach Claude Code Skill](https://github.com/silviocacace/TestCompass/blob/master/tools/testcompass-claude-code-skill.zip)**

*Special thanks to James Bach for creating and sharing this skill with the TestCompass community.*

*(Note: This skill is an independent contribution from James Bach and is not part of the core TestCompass product.)*

---

> **Key Takeaway**  
> Text-based Mermaid diagrams bridge the gap between human-readable repository documentation and formal eMBT models, ensuring seamless collaboration and version-controlled test design across your application lifecycle.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

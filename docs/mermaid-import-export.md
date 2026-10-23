[← Back to Documentation Index](index.md)

# Mermaid Import & Export

Mermaid import and export in TestCompass help teams exchange models across documentation, development and testing workflows.  
Because Mermaid is a text-based notation, it supports transparent collaboration, version control and readable diffs in Git.

> 💡 **Core Purpose**  
> Mermaid serves as a powerful text-based interchange format, enabling teams to embed models in documentation and track version changes in Git while maintaining rigorous eMBT semantics.

This page explains the purpose of Mermaid import and export, how they relate to modelling and how TestCompass supports a structured approach to maintaining consistency between diagrams and eMBT models.

---

## Purpose of Mermaid Import & Export

Mermaid import and export enable teams to:

- **Protect & reuse existing assets:** Easily convert legacy diagrams from for e.g. Visio, BPMN/BPM tools, Lucidchart and Draw.io into Mermaid syntax and import them directly into TestCompass.
- **Include models directly in documentation:** Seamlessly render behavioral models within Markdown files, Wiki pages, and GitHub/GitLab documentation.
- **Maintain version control in Git:** Store models as text-based files with clear, readable line-by-line diffs during code reviews.
- **Reconstruct & evolve models:** Convert text-based Mermaid code back into fully interactive, testable TestCompass models at any time.
- **Maintain single-source-of-truth consistency:** Keep system behavior descriptions synchronized across development teams, testers, and product owners.

By supporting Mermaid as an interchange format, TestCompass eliminates manual re-keying of existing process models, improves traceability and reduces friction between system design, documentation and automated test derivation.

---

## Import

When importing a Mermaid diagram, TestCompass converts the diagram into a structured eMBT model.  
During import, TestCompass:

- interprets nodes and transitions according to eMBT semantics  
- validates the structure and highlights inconsistencies  
- preserves incomplete or ambiguous behaviour  
- prevents hidden logic or implicit branches from being introduced  

Unsupported Mermaid constructs are reported clearly so the user can adjust the source diagram.

---

## Export

When exporting a model, TestCompass generates a Mermaid diagram that reflects the exact semantics of the underlying eMBT model.  
The exported Mermaid:

- is deterministic and suitable for version control  
- can be embedded in README files, wikis, and design documents  
- provides a documentation-friendly view of the model  
- does not alter or simplify the underlying TestCompass model  

Exported diagrams support communication and traceability, while the TestCompass model remains the authoritative source for test generation and impact analysis.

---

## Relationship to Modelling

Mermaid import and export complement the TestCompass modelling workflow.  
They make behaviour visible in documentation and version control, while TestCompass ensures that the model itself remains:

- explicit  
- semantically correct  
- traceable  
- aligned with eMBT principles  

This combination supports clear communication and consistent understanding across the entire team.

---

## AI-Assisted Mermaid Conversion

While TestCompass supports Mermaid import, not every valid Mermaid diagram can be converted directly into a TestCompass model. This is because TestCompass applies additional modelling rules and constraints to ensure model consistency and support for test generation.

To help with this, James Bach created a Claude Code skill that analyses Mermaid diagrams, identifies conflicts with TestCompass modelling rules, and assists in producing a TestCompass-compatible Mermaid model.

This community-contributed resource may be useful when working with Mermaid diagrams that require adaptations before they can be imported successfully into TestCompass.

🔗 **[Download James Bach Claude Code Skill](https://github.com/silviocacace/TestCompass/blob/master/tools/testcompass-claude-code-skill.zip)**

*Special thanks to James Bach for creating and sharing this skill with the TestCompass community.*

*(Note: This skill is an independent contribution from James Bach and is not part of the core TestCompass product.)*

---

>  **Key Takeaway**  
> Text-based Mermaid diagrams bridge the gap between human-readable documentation and formal behavioural models, ensuring seamless collaboration across your entire project lifecycle.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**


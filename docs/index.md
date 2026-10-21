<<script>
  window.addEventListener('DOMContentLoaded', (event) => {
    // Zoek naar de titel-link bovenaan de pagina en maak hem onklikbaar
    const topLinks = document.querySelectorAll('header a, .page-header a, .site-title a, .project-name');
    topLinks.forEach(link => {
      // Controleer of het om de hoofdtitel gaat
      if (link.textContent.trim() === "TestCompass") {
        link.removeAttribute('href');
        link.style.pointerEvents = 'none';
        link.style.cursor = 'default';
        link.style.color = 'inherit';
        link.style.textDecoration = 'none';
      }
    });
  });
</script>

# TestCompass Documentation   

Welcome to the TestCompass documentation

TestCompass helps teams make system intent explicit, model expected behaviour and derive systematic test scenarios through early Model-Based Testing (eMBT).

<img src="TestCompass.jpg" alt="Generated TestCompass Model" width="500">

---

## How This Documentation Relates to the Product

This documentation explains the **concepts** behind TestCompass:

- why explicit models matter  
- how decisions and paths drive test generation  
- how AI assists reasoning without taking over  
- how impact analysis supports continuous testing  
- how open formats enable integration  

The **Quick Start Guide** (available directly inside TestCompass via the Help menu and Book icon) explains the **practical steps** within the application. Together, they provide a complete understanding, from the underlying philosophy to the daily workflow.

---

## Documentation Index

### Core Concepts
- [TestCompass Overview](overview.md)
- [Behavioural Modelling](modelling.md)
- [The eMBT Approach](eMBT-approach.md)

### AI-Assisted Modelling
- [AI-Assisted Model Creation (AAMC)](aamc.md)
- [AI-Assisted Model Reflection (AAMR)](aamr.md)

### Testing and Analysis
- [Test Generation and Coverage](test-generation.md)
- [Impact Analysis](impact-analysis.md)

### Import, Export and Integrations
- [Mermaid Import and Export](mermaid-import-export.md)
- [Integrations](integrations.md)
- [Export Formats](export-formats.md)

---

If you want to explore a specific topic, start with the links above. Each page is designed to stand on its own while fitting into the broader eMBT workflow.

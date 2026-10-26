# TestCompass Documentation

Welcome to the official documentation repository for **TestCompass**, an Intent-Driven early Model-Based Testing (eMBT) platform designed to help teams reason clearly, uncover risks early, and build shared understanding before code is written.

---

## Quick Navigation

Inside the TestCompass application, you can easily access the Quick Start Guide, documentation, and video tutorials at any time via the **Help menu (`?`)** in the top navigation bar.

For public GitHub Pages documentation, explore the topics below:

### Getting Started & Workflow
- 📄 **[Overview](docs/overview.md)** — Core philosophy, value proposition, and how TestCompass fits into agile delivery workflows.
- 📄 **[The eMBT Approach](docs/eMBT-approach.md)** — The 4-phase eMBT workflow: Exploratory, Review, Coverage, and Checking.
- 📄 **[Quick Start Guide](docs/qsg.md)** — Step-by-step guide to building your first model and deriving tests.

### Modelling & AI Capabilities
- 📄 **[Behavioural Modelling](docs/modelling.md)** — Flowchart-based modelling foundations, node types, and requirements discovery.
- 📄 **[AAMC – AI-Assisted Model Creation](docs/aamc.md)** — Draft semantically correct models from plain text (user stories, spreadsheets, legacy diagrams, etc) in seconds.
- 📄 **[AAMR – AI-Assisted Model Reflection](docs/aamr.md)** — Uncover hidden assumptions and edge cases through interactive 3-question AI reflection loops.
- 📄 **[Mermaid Import & Export](docs/mermaid-import-export.md)** — Bi-directional sync between text-based Mermaid diagrams and testable eMBT models.
- 📄 **[BDD Discovery & Formulation](docs/bdd-discovery.md)** — BDD requirements discovery and formulation supported by TestCompass.

### Test Generation & Maintenance
- 📄 **[Test Generation and Coverage](docs/test-generation.md)** — Derive test scenarios automatically based on Node, Edge, Path Pair, Path Triple, and Full Path Coverage.
- 📄 **[Impact Analysis](docs/impact-analysis.md)** — Automatically detect Added, Removed, Updated, and Unchanged scenarios as models evolve.

### Integrations, Formats & Security
- 📄 **[Export Formats](docs/export-formats.md)** — Overview of Excel (Test Design & Decision Tables), Gherkin (`.feature`), CSV, PNG, and native `.tcmodel` formats.
- 📄 **[Integrations](docs/integrations.md)** — Connecting TestCompass with Azure DevOps, Jira, Zephyr, Xray, and other test management tools.
- 📄 **[Security & Architecture](docs/security-architecture.md)** — Overview of AWS EU hosting, AES-256 encryption, TLS traffic security, BCP/DRP, and GDPR data disposal procedures.

---

## Platform Architecture & Security at a Glance

TestCompass is engineered as a secure, cloud-native SaaS platform built on enterprise standards:

- **Hosting & Infrastructure:** Fully hosted on AWS within the European Union (Frankfurt region / `eu-central-1`) using Elastic Beanstalk (Multi-AZ) and VPC isolation.
- **In-Transit Security:** Enforced HTTPS encryption using SSL/TLS protocols via AWS Certificate Manager.
- **At-Rest Security:** Customer data, databases (RDS PostgreSQL), and backups encrypted using industry-standard **AES-256**.
- **Continuity & Disposal:** Governed by official Business Continuity (BCP-001), Disaster Recovery (DRP-001, RTO < 1h, RPO max 24h), and Data Disposal (DDP-001, 7-day retention purge, GDPR Art. 17) policies.

For full technical and organizational security details, refer to the **[Security & Architecture Overview](docs/security-architecture.md)**.

---

## Video Tutorials & Visual Guides

Prefer learning visually? Explore our video library covering model creation, AI reflection loops, and test generation:

- **Website Tutorials:** [TestCompass Tutorials](https://www.compass-testservices.com/tutorials/)
- **YouTube Channel:** [TestCompass YouTube Channel](https://www.youtube.com/@testcompass9513)

---

## About the Creator

**TestCompass was created by Silvio Cacace**, drawing on over **30 years of practical domain expertise** in software testing, quality engineering, and Model-Based Testing.

Throughout his career leading test transformations across enterprise environments, Silvio recognized that most software defects originate from incomplete specifications and implicit assumptions long before code is written. 

<p align="center" style="margin-top: 20px;">
  <img src="docs\Silvio1.PNG" alt="Silvio Cacace - Creator of TestCompass" width="300" style="border-radius: 8px; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
</p>

To address this, he originally pioneered the **ATS & DTM methodology and DTM tool**, which served as the foundation for modern test design automation. Building on years of practical application, Silvio evolved ATS & DTM into the **early Model-Based Testing (eMBT)** approach and created **TestCompass** as its next-generation platform. Today, eMBT and TestCompass are applied in corporate environments, embedded in professional testing frameworks, and taught within software engineering programs across multiple Universities.

---

## Support & Enterprise Inquiries

For enterprise security reviews, vendor questionnaires, or platform demonstrations, please contact us:

- **Website:** [www.compass-testservices.com](https://www.compass-testservices.com)
- **LinkedIn:** [Silvio Cacace](https://www.linkedin.com/in/silviocacace/)

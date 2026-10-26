[← Back to Documentation Index](index.md)

# AAMR – AI-Assisted Model Reflection

AAMR (AI-Assisted Model Reflection) is an interactive feature in TestCompass that helps teams review and refine their models.

While AAMC helps you build an initial model draft, AAMR acts as a review partner. It analyzes your visual model, asks targeted questions about missing logic, and projects your answers directly back onto the canvas.

> **Purpose & Role of AAMR**  
> AAMR is designed to challenge implicit assumptions, discover missing edge cases, and ensure models are complete before test generation begins. It turns quiet model reviews into active, structured reflection loops.

---

## The 3-Question Reflection Loop

AAMR works through a structured three-step reflection loop, guiding teams from risk identification to model updates.

### 1. Model Analysis
AAMR evaluates the current model structure, identifies open paths, checks boundary conditions, and searches for unhandled exception flows.

### 2. Interactive Questions
Instead of changing the model automatically, AAMR presents short, specific questions to the user, such as:
* *What should happen if the payment gateway times out during authorization?*
* *Is there a retry limit for invalid login attempts?*
* *Does cancellation reset the inventory state immediately?*

### 3. Canvas Projection
Once you answer a question or accept a suggested resolution, AAMR projects the updated logic directly onto your canvas, adding the required nodes, branches, and outcomes automatically.

---

## Key Benefits & Use Cases

Using AAMR during refinement sessions or review loops provides several practical advantages:

* **Uncovering Hidden Assumptions:** Requirements often describe what the system *should* do, but AAMR helps you define what happens when things go wrong.
* **Faster Refinement Sessions:** Instead of manually drawing missing branches during team discussions, you can answer AAMR prompts and let the tool update the canvas.
* **Maintaining Model Integrity:** Every addition made by AAMR strictly follows TestCompass modelling rules, preventing broken paths or missing decision outcomes.

---

## Example: Refining an Order Workflow

Consider an initial model draft covering an order process. The basic happy path is present, but several business rules are missing.

1. **AAMR Detects a Gap:** The tool highlights the payment step and asks, *"What happens if the user cancels the order while payment is processing?"*
2. **User Input:** You select or type the business rule, for example: *"Cancel the payment request and return to the cart."*
3. **Model Update:** AAMR creates the decision branch, connects the nodes, and updates the canvas immediately.

---

> **Summary**  
> AAMR turns model reviews into a fast, guided process. By asking the right questions early, it helps teams spot missing requirements, complete their models, and build test suites with total confidence.

---

## Navigation

⬅️ **[Back to Documentation Index](index.md)**

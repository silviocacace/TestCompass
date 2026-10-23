[← Back to Documentation Index](index.md)

# BDD Requirements Discovery & Gherkin Export

In modern software delivery, effective testing starts long before code is written—it begins with a shared understanding of requirements. TestCompass bridges the gap between high-level requirements and executable specifications by supporting collaborative Behaviour-Driven Development (BDD) discovery practices, such as **Feature Mapping** and **Example Mapping**.

These practices align closely with industry-proven principles from BDD authorities like **John Ferguson Smart** (author of *BDD in Action*), emphasizing that discovering rules and concrete examples together prevents costly ambiguities and aligns business, development, and testing from day one.

> 💡 **Core Purpose**  
> TestCompass integrates collaborative requirements discovery directly into your workflow, allowing you to seamlessly transform discovery maps into explicit behavioural models and generate fully compliant Gherkin feature files automatically.

---

## The Value of Collaborative Discovery

Performing requirements discovery manually often leaves a disconnect between whiteboard sessions, documentation, and the actual test scripts. TestCompass eliminates this friction by providing a unified environment where discovery, modelling, and test generation flow naturally into one another.

### Key Advantages:
- **Shared Understanding:** Bring stakeholders together during refinement or "Three Amigos" sessions to uncover rules and edge cases early.
- **No Lost Context:** Move directly from a brainstorming session to a structured behavioural model without re-keying requirements.
- **Executable Specifications:** Automatically derive clean, structured Gherkin feature files (`.feature`) directly from validated models.
- **Continuous Alignment:** When business rules change, updating the model instantly highlights the impact on your Gherkin files and test scenarios.

---

## Practical Example: "Orders Cancelled Late"

To illustrate this workflow, consider an example inspired by **John Ferguson Smart** regarding order cancellations and late fees:

* **Business Rule:** *Orders cancelled less than 5 minutes before pickup time incur a $1.00 fee.*
* **Feature Mapping:** The team maps out the rule, the trigger condition, and concrete examples during a collaborative session.
* **Model Conversion:** The rule is captured as an explicit decision flow within TestCompass using simple decision nodes and outcomes.
* **Gherkin Export:** TestCompass automatically generates the corresponding Gherkin feature file with `Background`, `Scenario Outline`, and concrete examples.

---

## Step-by-Step: From Discovery to Gherkin

### 1. Perform Discovery
Start by capturing business rules and concrete examples using feature or example mapping principles directly within your collaborative sessions.

### 2. Transform into a Model
Translate your discovery map into an explicit behavioural model using TestCompass’s intuitive canvas. Ensure decisions, actions, and outcomes reflect the agreed business rules.

### 3. Select Test Coverage
Choose your desired coverage strategy (e.g., Node Coverage, Edge Coverage, or Path Pair Coverage) to determine how thoroughly the model paths should be tested.

### 4. Export to Gherkin Feature Files
To export all generated test scenarios as Gherkin scenarios:
1. Navigate to the **Test** tab in TestCompass.
2. Click on the button: **Export To: ‘Feature File’**.
3. If you prefer not to include every test scenario in the feature file, simply uncheck the **Include** box of the specific scenario. Notice that the test coverage percentage adjusts automatically.
4. The complete feature file will open as a text file named after your model with the `.feature` extension. *(Tip: If prompted for the first time, choose your preferred text editor app to open the file).*

```gherkin
Feature: Orders cancelled late
  As a customer
  I want to cancel my order
  So that I am not charged incorrectly

  Background:
    Given a valid user account
    And an active order

  Scenario Outline: Cancel order near pickup time
    Given the order is placed
    When the cancellation is requested <TimeBeforePickup> minutes before pickup
    Then the system should evaluate the late cancellation rule
    And the resulting fee should be <ExpectedFee>

    Examples:
      | TimeBeforePickup | ExpectedFee |
      | 15               | $0.00       |
      | 3                | $1.00       |

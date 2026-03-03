# ApM – BDD API Automation Framework (Cucumber + REST Assured + Java)

This repository contains an end‑to‑end **API automation framework** built using:

- **Java 17**
- **REST Assured**
- **Cucumber BDD**
- **JUnit/TestNG**
- **Maven**
- **Page Object + API Utils design patterns**

The framework is designed for testing REST APIs (Jira APIs in current implementation) using clean, maintainable, and reusable components.

---

## 📂 Project Structure
---

## 🚀 How to Run Tests

### **Using Maven**

Run the full test suite:

```bash
mvn clean test

Run using a specific runner:
mvn test -Dcucumber.filter.tags="@smoke"

Technologies Used





























ComponentDescriptionJava 17LanguageREST AssuredAPI Testing libraryCucumber BDDScenarios & step definitionsMavenDependency & test runnerJSON Schema ValidatorResponse validation

🔧 Configuration
All environment configs are stored in:
src/test/resources/Config.properties

Example:
jira.base.url = https://your-domain.atlassian.net
jira.user     = your-email
jira.token    = your-api-token


📝 Sample Cucumber Feature
CucumberFeature: Jira Issue Creation  Scenario: Create a Jira Issue    Given I have an authenticated Jira request specification    When I create a new issue with summary "Test Summary" and description "Demo"    Then the API status code should be 201    And I remember the issue keyShow more lines

🏗️ Framework Highlights

Reusable APIUtils for request specs
Centralized request body builders
Data-driven scenarios using Scenario Outline
JSON schema validation
End-to-end Jira workflows (create → update → comment → transition)
Modular folder structure


📌 How to Extend
You can easily extend the framework by:

Adding new features in /features
Adding new step definitions in /steps
Creating API request POJOs under /model
Adding new request builder methods in APIUtils


🧑‍💻 Author
Aparna

Automation Developer – API + BDD + Java


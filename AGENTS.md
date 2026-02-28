```markdown
# AGENTS.md - Guidelines for AI Coding Agents

These guidelines are designed to ensure the efficient, maintainable, and high-quality development of AI coding agents within this repository. Adherence to these principles is crucial for successful project execution.

## 1. DRY (Don't Repeat Yourself)

*   **Module Reuse:** Each module (e.g., data processing, agent logic, API interaction) should have a clearly defined, self-contained purpose. Avoid creating overly generic or duplicated code.
*   **Abstraction:**  Where possible, abstract common functionality into reusable components.
*   **Standardized Code Patterns:**  Adopt and consistently apply established patterns for specific tasks.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimize Complexity:** Keep functions and classes as small and focused as possible. Avoid overly complex logic within individual units.
*   **Readability:** Code should be easily understood by other developers. Employ meaningful variable names and clear code structure.
*   **Single Responsibility Principle:** Each function or class should have a single, well-defined responsibility.

## 3. SOLID Principles

*   **Single Responsibility:** Each class should have one primary responsibility.
*   **Open/Closed Principle:** The system should be extensible through addition of new features without modifying existing code. (This is addressed through API contracts and modular design).
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the system.
*   **Interface Segregation Principle:** Clients should not be forced to depend on methods they do not use.
*   **Dependency Inversion Principle:** High-level modules should not depend on low-level modules.

## 4. YAGNI (You Aren't Gonna Need It)

*   **Avoid Unnecessary Code:** Do not write code that is not currently needed or is not required for the current task. Focus solely on the requirements of the current implementation.
*   **Refactor Only When Necessary:** Refactoring should be driven by demonstrable problems or enhancements to code quality, not by an assumption of future needs.

## 5. Development & Testing

*   **Maximum Code Length:** Each file shall not exceed 180 lines of code.
*   **Comprehensive Testing:**  All tests shall have a minimum coverage of 80% (as defined in the Test Coverage section).
*   **Test-Driven Development:** Prioritize writing tests before implementing functionality.  Tests should provide clear and concise expectations for expected behavior.
*   **Unit Testing:**  All code within a file should be thoroughly unit tested.  Each function and class should be tested independently.
*   **Integration Testing:**  Test interactions between modules to verify data flow and system behavior.
*   **Regression Testing:**  After changes, ensure existing functionality remains intact through regression tests.
*   **Code Reviews:**  All code changes must undergo a formal code review process prior to merging into the main branch.


## 6. File Structure (Example - Adjust as Needed)

```
AGENTS.md
├── data/
│   ├── config.json
│   ├── data.db
│   └── ...
├── agent_logic/
│   ├── agent_main.py
│   ├── agent_utils.py
│   └── ...
├── tests/
│   ├── test_agent_main.py
│   ├── test_agent_utils.py
│   └── ...
├── README.md
└── .gitignore
```

## 7.  Test Coverage Metrics

*   **Unit Tests:** Aim for 80%+ coverage.
*   **Integration Tests:** Aim for 70%+ coverage.
*   **System Tests:** Aim for 60%+ coverage (if possible, with well-defined scenarios).

## 8.  Documentation

*   **Comments:**  Provide clear and concise comments to explain complex logic.
*   **Docstrings:** Use docstrings to document modules, functions, and classes.
*   **README:** A README file explaining the project's purpose, setup instructions, and testing procedures.

## 9.  Error Handling

*   **Graceful Failure:** Implement error handling to prevent unexpected crashes and provide informative error messages.
*   **Logging:** Utilize logging to track events and errors during execution.

## 10.  Future Considerations

*   **Model Integration:**  Future modules will integrate with various AI models.
*   **API Management:** Develop a robust API management system.
*   **Agent Networking:**  Implement agent communication and synchronization.

```
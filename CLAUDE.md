# Project Specifications

<!-- 
INSTRUCTIONS FOR AGENTS:
Before starting implementation, scan this document for any remaining [[ ]] placeholders.
If ANY [[ ]] blanks remain unfilled, you MUST ask the user to provide values for each 
unknown before proceeding. Do NOT guess or assume values for unfilled blanks.
List all unfilled [[ ]] items and request clarification.
-->

<!-- Fill in the [[ ]] blanks below. Delete sections that don't apply to your project. -->

---

## 1. Project Identity

**Name:** [[ project name ]]

**Motivation/Goal:**  
[[ Why does this project exist? What problem does it solve? ]]

**Project Type:** [[ web | cli | api | library | other ]]

**Target Platform/Runtime:** [[ e.g., Linux, Windows, Docker, browser ]]

**Python Version:** [[ e.g., 3.11 ]]

---

## 2. Core Requirements

### Must-Have Features
1. [[ feature 1 ]]
2. [[ feature 2 ]]
3. [[ feature 3 ]]

### NOT Included (explicitly out of scope)
- [[ excluded feature 1 ]]
- [[ excluded feature 2 ]]

### Acceptance Criteria
- [[ criterion 1 ]]
- [[ criterion 2 ]]

---

## 3. Technical Constraints

**Language/Framework:** [[ e.g., Python 3.11, FastAPI 0.100+ ]]

**File Structure:**
```
[[ project_root ]]/
├── [[ src/ or main module ]]
├── [[ tests/ ]]
├── [[ config/ ]]
└── [[ other directories ]]
```

**Styling Approach (if UI):** [[ e.g., TailwindCSS, vanilla CSS, none ]]

---

## 4. Dependencies & Integration Points

### Required Packages
- [[ package1 ]] [[ optional version ]]
- [[ package2 ]]
- [[ package3 ]]

### External APIs
- [[ API name ]]: [[ endpoint or description ]]

### Environment Variables
- `[[ VAR_NAME ]]`: [[ description ]]

### Auth Requirements
[[ e.g., API key, OAuth, none ]]

---

## 5. Data & State

### Data Models/Schemas
```python
# Example:
# class User:
#     id: int
#     name: str
#     email: str

[[ Define your data models here ]]
```

### State Management
[[ e.g., in-memory, Redis, database, file-based ]]

### Persistence
[[ e.g., SQLite, PostgreSQL, JSON files, none ]]

---

## 6. UI/UX Spec (if applicable)

### Wireframe/Layout
```
[[ ASCII mockup, description, or link to spec file/image]]

Example:
+------------------+
|     Header       |
+------+-----------|
| Nav  |  Content  |
+------+-----------+
|     Footer       |
+------------------+
```

OR 

```
images/mockup.png
```

### Color Palette / Theme
[[ e.g., dark theme, earth tones, specific hex codes ]]

### Key Interactions
- [[ interaction 1 ]]
- [[ interaction 2 ]]

---

## 7. Project Settings

<!-- Mark [X] to enable, [_] to disable -->

```
[_] Generate and run tests (pytest, >95% coverage)
[_] PEP 8 compliance
[_] Linting with ruff
[_] Type-checking with mypy
[_] Performance profiling
[_] Generate temporary plan file (.md) to confirm before building any feature or function
```

---

## 8. Project Preferences & Limitations

### DO THIS (when possible):
- [[ preference 1 ]]
- [[ preference 2 ]]
- [[ preference 3 ]]

### DON'T DO THIS (ever):
- [[ limitation 1 ]]
- [[ limitation 2 ]]
- [[ limitation 3 ]]

---

## 9. Agent Settings

<!-- Mark [X] to enable, [_] to disable -->

```
[_] Concise interactions
    "In all interactions and commit messages, be extremely concise and sacrifice grammar for the sake of concision."

[_] Task summary after completion
    "After completing a task that involves tool use, provide a quick summary of the work you've done."

[_] Persist through context compaction
    "Your context window will be automatically compacted... do not stop tasks early due to token budget concerns... save your current progress and state to memory before the context window refreshes."

[_] Default to action
    "By default, implement changes rather than only suggesting them. If the user's intent is unclear, infer the most useful likely action and proceed."

[_] Do not act before instructions
    "Do not jump into implementation or change files unless clearly instructed to make changes."

[_] Delegate to subagents when beneficial
    "Only delegate to subagents when the task clearly benefits from a separate agent with a new context window."

[_] Reflect on tool results
    "After receiving tool results, carefully reflect on their quality and determine optimal next steps before proceeding."

[_] Use parallel tool calls
    "If you intend to call multiple tools and there are no dependencies between the tool calls, make all of the independent tool calls in parallel."

[_] Clean up temporary files
    "If you create any temporary new files, scripts, or helper files for iteration, clean up these files by removing them at the end of the task."

[_] Avoid over-engineering
    "Avoid over-engineering. Only make changes that are directly requested or clearly necessary. Keep solutions simple and focused."

[_] No extra features
    "Don't add features, refactor code, or make 'improvements' beyond what was asked."

[_] Minimal error handling
    "Don't add error handling, fallbacks, or validation for scenarios that can't happen. Trust internal code and framework guarantees."

[_] No premature abstractions
    "Don't create helpers, utilities, or abstractions for one-time operations. Don't design for hypothetical future requirements."

[_] Creative frontend aesthetics
    "Avoid generic AI-generated aesthetics... make creative, distinctive frontends that surprise and delight."

[_] Investigate before answering
    "Never speculate about code you have not opened. If the user references a specific file, you MUST read the file before answering."
```

---

## 10. Code Quality Standards

<!-- These are always applied -->

- Break functions into simple, readable, reusable units
- Document all functions with input/output and purpose
- Do NOT over-document (no line-by-line comments)

### Docstring Format
```python
def example_function(param1: str, param2: int) -> bool:
    """
    Brief description of what the function does.

    Args:
        param1: Description of param1
        param2: Description of param2

    Returns:
        Description of return value
    """
    pass
```

---

## 11. Debugging & Investigation Protocol

<!-- Instructions for Claude when issues arise -->

**Systematic Methodology:**
- Reproduce with minimal test case
- Form hypothesis and test systematically
- Binary search approach for issue isolation

**Issue Isolation:**
- State inspection at critical execution points
- Data flow analysis and variable tracking
- Timeline reconstruction for race conditions

**Root Cause Focus:**
- Fix causes, not symptoms
- Prevent recurrence
- Document findings

**Tools to Leverage:**
- Memory debugging (Valgrind, AddressSanitizer)
- Performance profiling
- Log analysis and pattern recognition
- Stack trace interpretation

**Advanced Techniques:**
- Race condition and concurrency detection
- Resource utilization monitoring
- Error propagation analysis

---

## 12. Anti-Hallucination Guardrails

### Assumptions (mock these, don't implement)
- [[ Assume X works ]]
- [[ Assume Y is available ]]

### Complexity Budget
[[ e.g., keep under 500 LOC, max 10 functions, single file ]]

---

<!-- END OF TEMPLATE -->

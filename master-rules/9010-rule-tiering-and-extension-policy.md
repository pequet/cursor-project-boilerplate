---
description: "Defines the application of rule tiers (Universal, Standards, Context-Specific) at the Submodule level and outlines the policy for adding submodule-specific rules."
globs: ["master-rules/*.md", "**/master-rules/*"]
alwaysApply: false
---
# 9010: Rule Tiering and Extension Policy (Submodule Level)

## 1. Purpose

This document provides a definitive analysis of how the framework's rule tiers apply to a **Submodule Archetype**. It confirms that the current rule set is appropriate for an archetypal source and establishes the formal policy for extending it with submodule-specific rules.

## 2. Rule Tier Application at the Submodule Level

The `Rules Distribution Matrix` specifies a tier requirement of **"U + full S"** for a Submodule that serves as an archetypal source, which `cursor-project-boilerplate` does. For simple, single-purpose submodule instances, the requirement is "U (required) + targeted S".

The evaluation of the current rules for this archetypal submodule is as follows:

| Rule Series | Tier | Analysis at Submodule Level | Verdict |
| :--- | :--- | :--- | :--- |
| **0000-9000s**| **U** | The Universal series provides the non-negotiable baseline for safety and behavior. These are **mandatory** to ensure the submodule integrates safely with any parent system. | **Correctly Placed** |
| **2000 Series** | **S** | As an **archetypal source**, this submodule must contain the complete library of standards. This allows any new project or system spawning from this boilerplate to have access to the full set of best practices. | **Correctly Placed** |
| **9999 Index** | **S** | The index is required as this level distributes the full set of Tier S rules. | **Correctly Placed** |

### Conclusion
This submodule is correctly constituted as a canonical source, containing all Universal and Standard rules necessary for spawning new, compliant projects and submodules.

## 3. Policy for Level-Specific Rule Extension (Tier C)

Submodules often contain specialized tools or logic, making **Tier C (Context-Specific)** rules essential for enforcing their unique operational requirements.

### Guiding Principle
Tier C rules in a submodule should govern its specific domain, such as enforcing coding standards for a particular framework, managing a unique deployment process, or interacting with a specific API. They **must not** conflict with Tier U or S rules.

### Numeric Range for Tier C Rules
-   **Reserved Range:** `4000-4999`
-   This range is exclusively for submodule-specific rules to ensure clear separation from Project-level (`3000-3999`) or Root-level experimental rules.

### Procedure for Adding a Tier C Rule
1.  **Justify the Need:** Define why the rule is necessary for the submodule's specific function.
2.  **Select a Number:** Choose an unused number within the `4000-4999` range.
3.  **Write the Rule:** Author the rule following the standards in `9000-effective-rule-writing.md`.
4.  **Add to Index:** Update the submodule's local `9999-index.md` to include the new Tier C rule.

### Example Tier C Rule Justification

-   **File:** `4010-react-component-naming-convention.md`
-   **Justification:** "This submodule is a React component library. This rule enforces that all component files use PascalCase (`MyComponent.jsx`), a convention specific to React. This is too domain-specific for a general Tier S rule but is critical for maintaining consistency within this submodule."

---
description: AI rules derived by SpecStory from the project AI interaction history
applyTo: "*,**/*"
---

## <headers/>

This file defines all project rules, coding standards, workflow guidelines, references, documentation structures, and best practices for the AI coding assistant.

## RULE ORGANIZATION

The rules are organized in `.mdc` files within the `.cursor/rules/` directory. The filenames are prefixed with numbers to indicate their priority. Lower numbers indicate higher priority.

*   `000-rule-organization.mdc`: Documents the rule organization system and numbering conventions

*   `001-effective-rule-writing.mdc`: Defines standards for writing clear and actionable rule files

## GENERAL BEHAVIOR

*   **Never delay action:** Once a direct command is confirmed, execute it immediately. (200-never-delay-action.mdc)
*   **Initialization Behavior:** Follow the defined conversation initialization protocol for reviewing project status. (201-initialization-behavior.mdc)
*   **Critical Truthfulness Protocol:** Do not fabricate information. Report accurately. (202-critical-truthfulness-protocol.mdc)
*   **Questions are not Commands:** Do not misinterpret questions as action commands. (203-questions-are-not-commands.mdc)
*   **Diagnostic Hierarchy and Assumption Checking:** Follow the established progressive diagnostic sequence for troubleshooting issues. (205-diagnostic-hierarchy-and-assumption-checking.mdc)
*   **Direct Integration of Verified Facts:** Treat user-provided facts as ground truth without re-verification. (206-direct-integration-of-verified-facts.mdc)
*   **Timestamp Accuracy Protocol:** Use system commands for generating accurate timestamps. (207-timestamp-accuracy-protocol.mdc)

## MEMORY & CONTEXT

*   **Memory Bank:** The Memory Bank structure and its usage are defined for maintaining project context. (210-memory-bank.mdc)
*   **Memory Reset Protocol:** Follow the established sequence for reviewing context upon initialization or reset. (220-memory-reset-protocol.mdc)

## TECH STACK

(To be populated with project-specific details)

## PROJECT DOCUMENTATION & CONTEXT SYSTEM

(To be populated with links to project documentation, style guides, and any relevant context)

## WORKFLOW & RELEASE RULES

(To be populated with rules about branching, pull requests, testing, and deployment)

## DEBUGGING

(To be populated with specific debugging strategies or tools)
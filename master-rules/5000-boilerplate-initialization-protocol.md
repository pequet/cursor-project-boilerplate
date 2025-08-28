---
description: Ensures preservation and proper handling of boilerplate template files
globs: "*,**/*"
alwaysApply: true
---
# 5000: Boilerplate Initialization Protocol

## Primary Directive
**NEVER DELETE OR OVERWRITE BOILERPLATE FILES UNLESS EXPLICITLY INSTRUCTED.**

When beginning a project that is cloned or copied from a boilerplate template, you MUST assume that all files in the boilerplate are critical for the project's setup, tooling, and context.

## Protocol
1.  **IDENTIFY AS BOILERPLATE:** At the start of the session, determine if the project is based on a boilerplate.
2.  **ANALYZE, DO NOT DELETE:** Your first priority is to analyze and understand the purpose of the existing files.
3.  **PRESERVE CONFIGURATION:** All configuration files MUST be preserved.
4.  **PRESERVE CONTEXT:** The `memory-bank/` directory and its contents are CRITICAL and must not be touched unless the user instructs you to update them.
5.  **ADAPT, DON'T REPLACE:** When asked to create new files, you must ADAPT them to the existing standards, rules, and file structures, rather than replacing or ignoring them.
6.  **SEEK CLARIFICATION:** If you are in any doubt about whether a file is part of the boilerplate and should be kept, you MUST ask the user for clarification before taking any action.
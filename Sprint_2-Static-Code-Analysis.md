# Trivy Static Analysis Report

## Project

**Project:** CastlingChaos  
**Sprint:** Sprint 1  
**Analysis Tool:** Trivy  
**Trivy Version:** 0.75.0  
**Scan Type:** Filesystem scan  
**Execution:** Local Windows 11 machine

## 1. Tools Used

### Programming Language

The project is primarily written in **C#** and is developed using **Unity 6.0.6.4f1**.

### Trivy

- **Tool:** Trivy
- **Version:** 0.75.0
- **Scan type:** Filesystem
- **Execution:** Local
- **Operating System:** Microsoft Windows 11 Home

The Trivy filesystem scan was executed against the CastlingChaos project repository.

## 2. Required Metrics

The Trivy filesystem scan reported the following severity counts:

| Severity | Findings |
|---|---:|
| CRITICAL | 0 |
| HIGH | 0 |
| MEDIUM | 0 |
| LOW | 0 |

### Secrets

Trivy also performed secret scanning.

**Secrets detected: 0**

### Scan Limitation

Trivy reported that no supported language-specific files were found for its vulnerability scanner:

> `Number of language-specific files num=0`

It also reported:

> `Supported files for scanner(s) not found.`

Therefore, the severity counts above represent **no vulnerability findings reported by Trivy**, rather than confirmation that every C# dependency in the project was independently analyzed.

The secret scanner completed successfully and reported no issues.

## 3. Scope

The Trivy filesystem scan covered the CastlingChaos project repository.

The primary application source is located under:

Assets/Scripts/
├── Logic/
├── UI/
└── View/
For the project-level scan, the following Unity-generated or local-development directories were excluded:

- `Library`
- `Temp`
- `Logs`
- `UserSettings`

These directories were excluded because they contain Unity-generated or local user/environment data rather than the project's authored source code.

## 4. Trend

This is the **first sprint**, so there is no previous sprint to compare against.

**Baseline sprint — no prior comparison.**

The results from this scan establish the baseline for future sprints.

## 5. Reflection

The Trivy scan did not identify any secrets, and no vulnerability findings were reported. The primary limitation of this scan was that Trivy did not identify supported language-specific dependency files for vulnerability analysis.

For the next sprint, the team should continue scanning the repository and investigate whether project dependency information can be exposed in a format that allows Trivy to perform more comprehensive dependency vulnerability analysis.

## Required Statement

> “This static analysis was generated using automated tools during this sprint.”

## Scan Result Summary

| Item | Result |
|---|---|
| Trivy Version | 0.75.0 |
| Scan Type | Filesystem |
| Execution | Local |
| CRITICAL | 0 |
| HIGH | 0 |
| MEDIUM | 0 |
| LOW | 0 |
| Secrets | 0 |
| Sprint | **1 — Baseline** |

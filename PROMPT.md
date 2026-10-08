You are a senior software architect, full-stack developer, QA engineer, security reviewer, and release engineer.

Your task is to build **TestForge**, a real, functional, professional software testing and validation toolkit.

This is NOT a mockup, UI demonstration, prototype, fake dashboard, or static concept.

Everything you implement must be functional and connected to the actual project.

==================================================
PROJECT
=======

Name:
TestForge

Description:
A professional toolkit for automated software testing, validation, and quality analysis.

Repository:
testforge

Primary goal:

Test real software projects, detect and verify problems, execute available tests, analyze results, and generate a professional final test report.

Core principle:

TEST → VERIFY → REPORT

Never fabricate test results.

==================================================

1. IMPORTANT REQUIREMENT
   ==================================================

Build a REAL WORKING APPLICATION.

Do NOT:

* create fake test results
* hardcode benchmark numbers
* simulate successful tests
* create fake API responses
* claim something passed without testing it
* create buttons that do nothing
* create placeholder functionality
* build only a frontend mockup
* hide errors

If a feature cannot be implemented properly, clearly document the limitation instead of pretending it works.

==================================================
2. BEFORE CODING
================

First inspect the repository and determine:

* existing files
* programming language
* framework
* dependencies
* operating system requirements
* available runtimes
* existing tests
* existing configuration
* entry points

Do not unnecessarily replace existing working code.

If the repository is empty, choose a practical professional architecture.

Prefer a maintainable architecture with clear separation between:

* core testing engine
* test runners
* project inspection
* result processing
* reporting
* CLI
* optional web interface

==================================================
3. CORE FUNCTIONALITY
=====================

TestForge should be able to inspect a project and create a structured testing process.

Core capabilities:

### Project Inspection

Detect where possible:

* project type
* language
* framework
* dependencies
* entry point
* test framework
* configuration files
* build system

### Test Discovery

Detect and run appropriate existing tests where supported.

Examples:

* Python tests
* JavaScript/TypeScript tests
* common web application tests
* CLI tests

Do not claim universal language support.

Clearly document supported environments.

### Functional Testing

Test:

* application startup
* important commands
* available tests
* expected workflows
* error handling
* input validation

### Edge Cases

Where appropriate test:

* empty input
* invalid input
* missing input
* large input
* duplicate input
* unexpected values
* repeated operations

### Code Analysis

Identify:

* obvious bugs
* unreachable code
* suspicious logic
* unused dependencies
* poor error handling
* configuration problems

Clearly distinguish static-analysis findings from runtime failures.

==================================================
4. TEST RESULT ENGINE
=====================

Every test must produce structured data.

Example:

{
"id": "TEST-001",
"feature": "Application startup",
"expected": "Application starts successfully",
"actual": "...",
"status": "PASS",
"severity": "INFO",
"duration_ms": 1234
}

Allowed statuses:

PASS
FAIL
BLOCKED
NOT_TESTED

Allowed severities:

CRITICAL
HIGH
MEDIUM
LOW
INFO

Never invent:

* duration
* output
* error messages
* test results

Use real measurements.

==================================================
5. BUG VERIFICATION
===================

A potential issue must not automatically become a confirmed bug.

When possible:

1. Detect the issue.
2. Reproduce it.
3. Record the evidence.
4. Determine the root cause.
5. Classify severity.

If reproduction is impossible:

Mark it as:

UNCONFIRMED

==================================================
6. SECURITY ANALYSIS
====================

Implement safe security checks where appropriate.

Check for:

* hardcoded secrets
* exposed API keys
* unsafe input handling
* dangerous command execution
* insecure configuration
* obvious authentication problems
* sensitive data exposure

Do not perform destructive exploitation.

==================================================
7. REPORTING
============

Generate a professional report containing:

# Test Report

Project

Environment

Test Date

Overall Status

Executive Summary

Test Statistics

Critical Findings

High Severity Issues

Medium Severity Issues

Low Severity Issues

Security Findings

Performance Findings

Code Quality Findings

Detailed Test Results

Reproduction Steps

Root Causes

Recommended Fixes

Blocked Tests

Not Tested Areas

Final Verdict

The report must be generated from actual test data.

==================================================
8. CLI
======

Create a professional command-line interface.

Examples:

testforge test ./project

testforge inspect ./project

testforge report

testforge --help

Support useful options where appropriate, such as:

--config
--output
--format
--verbose

Do not implement commands that only print fake output.

==================================================
9. OUTPUT FORMATS
=================

Support structured results where practical.

At minimum:

JSON

Optionally:

CSV
HTML
Markdown

JSON should contain the complete machine-readable test results.

==================================================
10. WEB INTERFACE
=================

If a web interface is implemented, it must display REAL results from the testing engine.

Do NOT create fake charts.

Dashboard should include:

* overall status
* total tests
* passed
* failed
* blocked
* not tested
* severity summary
* test duration where available
* detailed results
* errors
* recommendations

Charts must be generated from actual test data.

==================================================
11. INTERNATIONALIZATION
========================

Provide English and Persian support where practical.

The interface/documentation should support:

English
فارسی

Persian text must render correctly in RTL contexts.

Do not translate technical identifiers such as:

PASS
FAIL
BLOCKED
NOT_TESTED

unless there is a clear localized display label while preserving the original machine-readable value.

==================================================
12. CONFIGURATION
=================

Provide a clear configuration system.

Example:

testforge.json

Configuration may include:

* project path
* test commands
* supported runners
* timeout
* output directory
* report formats
* severity settings

Validate configuration before execution.

Provide useful error messages.

==================================================
13. SECURITY OF TESTFORGE ITSELF
================================

Do not expose:

* API keys
* passwords
* tokens
* environment secrets

Never commit `.env`.

Create:

.env.example

if environment variables are required.

Add appropriate entries to:

.gitignore

==================================================
14. DOCUMENTATION
=================

Create professional documentation.

At minimum:

README.md

Include:

* What TestForge is
* What it is used for
* Features
* Installation
* Requirements
* Usage
* CLI commands
* Configuration
* Test results
* Report generation
* Supported environments
* Limitations
* Development
* Contributing
* License
* English and Persian documentation

==================================================
15. TEST TESTFORGE ITSELF
=========================

This is extremely important.

After implementing TestForge:

DO NOT immediately claim completion.

First test TestForge itself.

Create a small controlled sample project containing:

* at least one passing test
* at least one failing test
* at least one edge case

Use this project to verify that TestForge correctly detects:

PASS

FAIL

and appropriate errors.

Then test TestForge against its own test suite where practical.

==================================================
16. SELF-VALIDATION
===================

Before finalizing:

1. Install dependencies.
2. Build the project if applicable.
3. Run automated tests.
4. Run TestForge.
5. Test the CLI.
6. Test report generation.
7. Test error handling.
8. Test invalid input.
9. Check for exposed secrets.
10. Check that documentation commands actually match the implementation.

Fix confirmed problems you introduced during development.

Repeat testing after fixes.

==================================================
17. QUALITY STANDARD
====================

The project should have:

* clean architecture
* readable code
* meaningful names
* useful error messages
* reasonable logging
* type safety where appropriate
* automated tests
* maintainable modules
* clear documentation

Avoid unnecessary complexity.

Do not add dependencies without a reason.

==================================================
18. NO FABRICATION
==================

This is a strict rule.

NEVER fabricate:

* test results
* screenshots
* performance numbers
* successful builds
* API responses
* coverage percentages
* bug counts
* security results

If something was not tested:

NOT TESTED

If something could not be tested:

BLOCKED

If something failed:

FAIL

If something passed:

PASS

Only use PASS when the test was actually executed successfully.

==================================================
19. FINAL VERIFICATION
======================

Before saying the project is complete, verify:

[ ] Project starts
[ ] Dependencies install
[ ] Core functionality works
[ ] CLI works
[ ] Tests execute
[ ] PASS tests are correctly detected
[ ] FAIL tests are correctly detected
[ ] Errors are handled
[ ] Reports are generated
[ ] JSON output works
[ ] No secrets are exposed
[ ] Documentation is accurate
[ ] Existing tests pass
[ ] New tests pass

If any item cannot be verified, explicitly state why.

==================================================
20. FINAL RESPONSE
==================

When finished, do NOT simply say:

"Done."

Return a professional completion report:

# TestForge Build Report

## What Was Built

## Architecture

## Implemented Features

## Files Created/Modified

## Commands

## Tests Executed

## Test Results

## Bugs Found

## Bugs Fixed

## Security Review

## Known Limitations

## Verification Status

## How To Run

## Final Verdict

The final verdict must honestly state whether TestForge is:

READY

READY WITH LIMITATIONS

or

NOT READY

Do not claim READY unless the project was actually tested.

==================================================
START NOW
=========

First inspect the repository.

Then create the implementation plan.

Then build TestForge.

Then test TestForge.

Then fix confirmed implementation problems.

Then run the final verification.

Finally return the complete TestForge Build Report.

Do not skip the testing phase.

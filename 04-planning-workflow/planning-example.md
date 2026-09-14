
# Planning Workflow Example

## Workplace Scenario

The Medical Documentation Department needs to complete a monthly documentation report. The work includes reviewing the required data, validating the information, preparing the report, completing a quality check, and submitting the final version.

## Planning Objective

The objective was to use generative AI to turn the reporting requirement into a structured action plan with clear tasks, owners, deadlines, phases, and dependencies.

## Weak Planning Prompt

> Create a plan for the monthly medical documentation report.

This prompt is too general because it does not specify the required tasks, roles, deadlines, dependencies, or expected format.

## Structured C.A.R.E. Planning Prompt

> **Context:** I work in the Medical Documentation Department. We need to complete a monthly documentation report and submit the final version by the end of the week.
>
> **Action:** Create a structured implementation plan that breaks the work into phases and actionable tasks.
>
> **Role:** Act as an experienced healthcare operations and documentation project coordinator.
>
> **Expected Output:** Provide a concise table with the phase, task, owner, deadline, and dependency for each task. Prioritize tasks that must be completed first and identify the critical dependencies.

## AI-Assisted Planning Output

| Phase | Task | Owner | Deadline | Dependency |
|---|---|---|---|---|
| 1. Preparation | Confirm reporting requirements and required data | Documentation Team | Day 1 | None |
| 1. Preparation | Gather the required documentation data | Assigned Staff Member | Day 1 | Reporting requirements confirmed |
| 2. Validation | Review data for completeness and accuracy | Assigned Staff Member | Day 2 | Data gathered |
| 2. Validation | Resolve missing or inconsistent information | Assigned Staff Member | Day 3 | Validation completed |
| 3. Report Preparation | Prepare the monthly documentation report | Documentation Team | Day 4 | Data validated |
| 4. Quality Review | Review the completed report for accuracy and completeness | Supervisor | Day 5 | Report prepared |
| 5. Submission | Submit the final approved report | Documentation Team | Day 5 | Supervisor review completed |

## Priorities and Dependencies

### High Priority

- Confirm the reporting requirements.
- Gather the required data.
- Validate the data before preparing the final report.

### Key Dependencies

- Report preparation depends on completing data validation.
- Final submission depends on supervisor quality review.
- Missing or inconsistent information should be resolved before the report is finalized.

## Human Review

The AI-generated plan was reviewed by the user to ensure that the tasks, responsibilities, sequence, and dependencies were reasonable for the workplace scenario.

The plan is intended as a planning aid. Actual owners, deadlines, and organizational procedures should be confirmed before implementation.

## Key Learning

A structured planning prompt produces a more actionable plan than a vague request. Adding context, action, role, and expected output helps generative AI organize work into clear phases, tasks, owners, deadlines, and dependencies.

Human review is still required to confirm that the proposed plan matches actual workplace requirements and responsibilities.

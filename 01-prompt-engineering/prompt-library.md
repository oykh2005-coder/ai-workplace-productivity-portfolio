# Prompt Library

## Purpose

This prompt library contains reusable prompts for common workplace tasks in Health Informatics and Medical Documentation.

The prompts follow the C.A.R.E. framework used in the course:

- **C — Context:** Provide the background, situation, and relevant constraints.
- **A — Action:** Clearly state what the AI should do.
- **R — Role:** Define the perspective, expertise, or voice the AI should adopt.
- **E — Expected Output:** Specify the required format, length, tone, structure, and audience.

The prompts are designed to be reusable by replacing the information inside `[brackets]`. They should be refined when the first output does not meet the required standard.

---

# Prompt 1 — Professional Workplace Email

## Use Case

Use this prompt when drafting a professional email about a workplace update, request, reminder, or change.

## C.A.R.E. Structure

**Context:**  
I work as a Health Informatics Specialist in Medical Documentation. I need to communicate a workplace matter to [recipient/audience]. The situation is: [brief background].

**Action:**  
Write a professional email that communicates [specific purpose or request]. Clearly explain the key information and any required action.

**Role:**  
Act as an experienced healthcare administration and professional communication specialist. Use a professional, respectful, and clear tone.

**Expected Output:**  
- Write a concise email.
- Include a clear subject line.
- Use short paragraphs.
- State the required action or next step clearly.
- Avoid unnecessary details.
- Do not invent facts that are not provided.
- Write in [English/Arabic].

## Reusable Prompt

> I work as a Health Informatics Specialist in Medical Documentation.  
> Context: [brief background].  
>   
> Action: Write a professional email to [recipient] about [purpose]. Clearly communicate [key points] and specify the required next step.  
>   
> Role: Act as an experienced healthcare administration and professional communication specialist.  
>   
> Expected Output: Provide a clear subject line and a concise professional email. Use a respectful tone, short paragraphs, and avoid adding information that was not provided. Write in [language].

---

# Prompt 2 — Meeting Notes to Action Items

## Use Case

Use this prompt to convert unstructured meeting notes into a clear and actionable summary.

## C.A.R.E. Structure

**Context:**  
The following information comes from a workplace meeting: [paste non-confidential meeting notes].

**Action:**  
Extract the key decisions, action items, owners, deadlines, unresolved questions, and risks. Separate confirmed information from items that still require a decision.

**Role:**  
Act as an experienced project coordinator who is skilled at organizing workplace information.

**Expected Output:**  
Present the result in a structured table with these columns:

| Item | Type | Owner | Deadline | Status |
|---|---|---|---|---|

Use these types where appropriate:
- Decision
- Action
- Open Question
- Risk

Do not assume missing owners or deadlines.

## Reusable Prompt

> Context: The following are non-confidential workplace meeting notes:
>   
> [PASTE NOTES]
>   
> Action: Extract the key decisions, action items, owners, deadlines, unresolved questions, and risks. Distinguish confirmed information from items that require a decision.
>   
> Role: Act as an experienced project coordinator.
>   
> Expected Output: Present the information in a table using these columns:
>   
> | Item | Type | Owner | Deadline | Status |
>   
> Use Decision, Action, Open Question, or Risk as the Type. If an owner or deadline is not provided, write "Not specified" instead of guessing.

---

# Prompt 3 — Information Processing and Summary

## Use Case

Use this prompt when workplace information is lengthy, repetitive, or unstructured and needs to be converted into a concise summary.

## C.A.R.E. Structure

**Context:**  
I have the following non-confidential workplace information: [paste information].

**Action:**  
Identify the main points, remove unnecessary repetition, group related information, and summarize the information without changing its meaning.

**Role:**  
Act as an information management specialist who prioritizes accuracy, clarity, and traceability to the source.

**Expected Output:**  
Produce:
1. A short executive summary.
2. Key points in bullet form.
3. Important dates, numbers, or requirements in a separate section.
4. Any unclear or missing information that requires human clarification.

Do not create facts that are not present in the source.

## Reusable Prompt

> Context: I need to process the following non-confidential workplace information:
>   
> [PASTE INFORMATION]
>   
> Action: Summarize the information, remove unnecessary repetition, group related points, and preserve the original meaning.
>   
> Role: Act as an information management specialist focused on accuracy and clarity.
>   
> Expected Output:
> 1. Executive Summary
> 2. Key Points
> 3. Important Dates, Numbers, or Requirements
> 4. Information Requiring Clarification
>   
> Do not invent, assume, or change information that is not supported by the source.

---

# Prompt 4 — Few-Shot Workplace Status Update

## Use Case

Use Few-Shot Prompting when the same type of workplace update is produced repeatedly and a consistent format is required.

The course demonstrates that examples can show the AI the desired format, structure, and level of detail, which can improve consistency for recurring tasks. :contentReference[oaicite:3]{index=3}

## Example 1 — Desired Format

**Input:**  
Project A is on track. The report was completed. The next review is Monday.

**Output:**  
- **Project:** Project A
- **Status:** On Track
- **Completed:** Report
- **Next Step:** Review
- **Next Review:** Monday

## Example 2 — Desired Format

**Input:**  
Project B is delayed because the required data has not been received. The team is waiting for the data. No revised completion date has been confirmed.

**Output:**  
- **Project:** Project B
- **Status:** Delayed
- **Issue:** Required data not received
- **Next Step:** Follow up on data
- **Next Review:** Not specified

## Reusable Few-Shot Prompt

> Convert the workplace update into the exact format shown in the examples.
>
> **Example 1**
>
> Input:  
> Project A is on track. The report was completed. The next review is Monday.
>
> Output:
> - Project: Project A
> - Status: On Track
> - Completed: Report
> - Next Step: Review
> - Next Review: Monday
>
> **Example 2**
>
> Input:  
> Project B is delayed because the required data has not been received. The team is waiting for the data. No revised completion date has been confirmed.
>
> Output:
> - Project: Project B
> - Status: Delayed
> - Issue: Required data not received
> - Next Step: Follow up on data
> - Next Review: Not specified
>
> **Task**
>
> Convert this new workplace update using exactly the same structure and level of detail:
>
> [PASTE NEW UPDATE]
>
> Do not invent missing information. If information is unavailable, write "Not specified."

---

# Prompt Refinement Approach

The first output should be treated as a starting point rather than a final answer. If the result is too vague, incomplete, incorrectly formatted, or inappropriate in tone, refine the prompt by adding clearer context, a more specific action, a better-defined role, or more precise output requirements.

The course emphasizes an iteration loop:

**Ask → Review → Refine → Improve → Repeat**

Small refinements can lead to better results. :contentReference[oaicite:4]{index=4}

---

# Safe Use

These prompts should be used with non-confidential or appropriately authorized information.

Do not include real patient identifiers, confidential medical information, passwords, credentials, or other sensitive organizational information unless the use is explicitly authorized and the approved AI environment provides appropriate protection.

AI-generated content must be reviewed by a human before being used for important workplace communication, documentation, reporting, or decision-making.

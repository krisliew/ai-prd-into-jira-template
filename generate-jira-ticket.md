# Rule: Generating ready-to-copy Jira Epic and Ticket from User Requirements

## Goal

To guide an AI assistant in creating a detailed, step-by-step feature story list in Markdown format based on user requirements, or feature requests. The Jira epic and ticket created should guide a developer through implementation.

## Output

- **Format:** Markdown (`.md`)
- **Location:** `/jira/`
- **Filename:** `epic-[epic-name].md` (e.g., `epic-user-profile-editing.md`)

### Output Structure

```markdown
# [Epic Name] - Implementation Plan & Jira Draft

- Project: [YOUR-PROJECT-KEY e.g. PROJ]
- Target Epic: [to be created / PROJ-???]
- Generated: 2026-01-11
- Feature Owner: [name / team]

## Business / User Goal (1–3 sentences)

Short description why this feature exists, who benefits, and what the main success looks like.

Example:  
Reduce payment drop-off by 15–25% by allowing safe automatic retries with clear user feedback instead of immediate failure.

## Suggested Epic (create this first!)

- **Epic Key:** PROJ-???
- **Summary:** [Feature Area] - [Short business goal]
- **Description:**  
  [2–4 sentences explaining the whole initiative, business impact, success metrics if any]
- **Labels:** feature-[shortname], [module], [quarter/year]
- **Epic Link field name:** (leave blank – Jira auto-populates after Epic is created)
- **Dependencies & Risks:**
  - External API availability
  - Other teams’ deliverables
  - Backward compatibility concerns

## Main User Stories (ready to copy-paste into Jira)

- Use **Feature** type for anything that delivers user/business value

### PROJ-??? Feature – As a [user role], I want [goal], so that [benefit]

- **Type:** Feature
- **Labels:** [frontend/backend/mobile, module, feature-shortname, etc]

**Acceptance Criteria**

- Given … when … then …
- Error case: …
- Edge case: …
- UI/UX requirement: … (if applicable)
- Performance: … (if relevant)
- Analytics event: … (if tracked)

**Notes / Open Questions**

- …

**Quick Checklist Before Starting**

- [ ] Epic created & linked
- [ ] Fix version & label
- [ ] Design / wireframes linked (if UX heavy)
- [ ] Dependencies / other teams informed

### PROJ-??? Feature [Create more feature as needed]

(same structure)
```

## Process

1.  **Receive Requirements:** The user provides a feature request, feature description, or points to existing documentation
2.  **Analyze Requirements:** The AI analyzes the functional requirements, user needs, and implementation scope from the provided information
3.  **Generate Feature Ticket:** Based on the requirements analysis, create the file and generate the epic and features required to implement. Use your judgement on how many additional feature to use. Present these feature story to the user in the specified output structure format above.
4.  **Generate Output:** Generate the final Markdown content into: `/jira/epic-[epic-name].md`

## Target Audience

Assume the primary reader is a **junior developer** who will implement the feature.

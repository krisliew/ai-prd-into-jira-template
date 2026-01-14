# AI Product Requirements Document into Jira Template

Greetings! This repository provides a collection of markdown files designed to assist you in creating PRDs and Jira Tickets with AI-powered IDEs and CLIs. These tools work with any AI coding assistant.

For product owner/manager and developer to generate ready-copy-paste Product Requirements Document (PRD) to confluence and Jira tickets.

## Workflow: From Idea to Implemented Feature

Here's the step-by-step process using the `.md` files in this repository:

### 1. Creating Product Requirements Document

First, lay out the blueprint for your feature. A PRD clarifies what you're building, for whom, and why.

1. Ensure you have the `create-confluence-prd.md` file from this repository accessible.
2. In your AI tool, initiate PRD creation:

```
Use @create-confluence-prd.md
Here's the feature I want to build: [Describe your feature in detail]
Reference files in your project to help you: [Optional: @file1.py @file2.ts]
```

- You may copy the markdown file into your project code to help with reference.

### 2. Creating Jira Epic and Features

With your PRD drafted (e.g., `prd-xxx.md`), the next step is to generate the Jira epic and features ticket.

1. Ensure you have `generate-jira-ticket.md` accessible.
2. In your AI tool, use the PRD to generate:

```
Now take @prd-xxx.md and generate Jira tickets using @generate-jira-ticket.md
```

#### This is inspired by https://github.com/snarktank/ai-dev-tasks

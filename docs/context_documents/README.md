# Context Documents

Context documents are continuation-ready project checkpoints. They preserve enough authoritative state for a person or AI assistant to resume work in a new conversation, on another device, or after a long interruption without reconstructing the project from memory.

They are working records rather than polished introductions. A repository's main `README.md` explains the project to a reader; a context document explains exactly how to continue the work.

## The question each document answers

> If this work had to resume in a fresh environment, what would the next collaborator or AI assistant need to know?

A useful context document preserves:

- the current purpose and scope;
- important terminology and naming decisions;
- repository structure and component responsibilities;
- implementation and experiment status;
- decisions, constraints, and their rationale;
- commands, tests, and known results;
- unresolved questions and risks; and
- immediate, concrete next steps.

Do not merely summarize the latest conversation. Capture the project's current state.

## Documentation hierarchy

```text
Repository README
    -> project brief or charter
        -> context documents / lab notebook
            -> detailed experiment notes and outputs
```

Each layer serves a different reader. Avoid duplicating everything from the repository README inside every context document.

## Where context documents belong

For a particular repository, store them in:

```text
docs/context_documents/
```

The newest applicable document should be easy to identify by filename. Do not place private participant information in a public repository. A private collaboration repository may contain participant-specific working context when the participant understands and approves its use.

## Naming convention

```text
LN_{{SHORT_PROJECT_MARKER}}_YYYY-MM-DD_{{optional-tag}}_-_{{short-slug}}.md
```

Examples:

```text
LN_ral_2026-10-16_ctx01_-_maya-onboarding-and-first-experiment.md
LN_pcp_2026-10-20_parked_-_synthetic-mixture-validation.md
```

`LN` means **Lab Notebook**. Keep the project marker short. Omit the optional tag unless it adds useful information, such as `ctx01`, `parked`, `handoff`, or `submitted-addenda`.

## Context-document template

Copy and complete the following structure. Remove sections that truly do not apply, but preserve concrete state and next actions.

```markdown
*BEGIN: Context Document Header*

# CONTEXT DOCUMENT — Continuation

## Project

**Name:**  
{{Short project name}}

**Description:**  
{{One to three sentences describing the project and what it produces}}

## Continuation metadata

**Prepared at:**  
{{YYYY-MM-DDTHH:MM:SS+/-HH:MM}}

**Continued from:**  
{{Exact chat, session, branch, issue, or prior context-document title}}

**Also involving:**

- {{Related topic, repository, or collaborator}}
- {{Related topic, repository, or collaborator}}
- {{Or: no other subjects specified}}

## Author and source

**Prepared by:**  
{{Person and, if useful, AI assistant}}

**Repository:**  
{{Repository URL or owner/repository}}

**Branch or revision:**  
{{Branch name and latest relevant commit, if known}}

## Intent for this context

{{What this checkpoint should enable the next session to accomplish}}

## Authoritative current state

{{What exists now, what works, and what has been verified}}

## Repository map

{{Important files and directories with their responsibilities}}

## Decisions and rationale

- {{Decision and why it was made}}
- {{Decision and why it was made}}

## Commands and verification

```bash
{{Commands needed to reproduce, test, or inspect the current state}}
```

**Observed results:**

{{What happened when the commands were last run; distinguish observation from expectation}}

## Constraints, risks, and privacy

- {{Known constraint, risk, privacy boundary, or safety rule}}

## Open questions

- {{Question that remains unresolved}}

## Immediate next steps

1. {{Small, concrete next action}}
2. {{Next action after that}}
3. {{Optional later action}}

## Definition of the next stopping point

{{What must be true before creating the next checkpoint or pausing}}

*END: Context Document*
```

## Optional pre-context-document prompt

Before pasting a context document into a fresh AI conversation, this short message can prevent unnecessary summarizing or re-derivation:

```markdown
## Current work

Project: {{Very short project description}}

The next message will be a continuation context document from:

"{{Previous chat or session title}}"

Treat it as authoritative project state. Do not summarize or reformat it. After receiving it:

1. confirm receipt;
2. identify any genuine blocker or contradiction; and
3. help me continue with this immediate task:

{{Concrete, task-oriented, ADHD-friendly next task}}
```

The pre-context prompt is optional. Give it to the **new** conversation, not to the conversation that is composing the context document.

## Creating a strong checkpoint

Before saving a context document:

1. Verify repository status, important filenames, and the current branch.
2. Separate observed results from plans or assumptions.
3. Record why non-obvious decisions were made.
4. Include enough commands to reproduce the current state.
5. Make the first next step small and unambiguous.
6. Remove secrets, credentials, private messages, and unnecessary personal information.
7. Prefer links to stable project documentation over copying large sections verbatim.

## Retrieval and continuation

To resume work:

1. Open `docs/context_documents/`.
2. Sort filenames by date.
3. Choose the newest document relevant to the current branch or task.
4. Check whether a later document supersedes it.
5. Begin with **Immediate next steps**.
6. Create a new checkpoint before another major handoff or long pause.

Context documents are checkpoint files for thinking: detailed enough to preserve momentum, restrained enough to remain usable.


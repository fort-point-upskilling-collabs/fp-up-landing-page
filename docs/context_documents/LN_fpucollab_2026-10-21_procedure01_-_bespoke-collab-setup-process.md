*BEGIN: Context Document Header*

# Bespoke Collaboration Setup Process

**Quick note on names**: certain people have been gracious enough to be the first adopters of the process described here. They will be referred to by first and last initials, which may or may not match their actual names. _Dave_ has done some of the setup, and his last name starts with B, so he would be referred to as _D.B._ with this convention; the combination of italics and the `"{{Letter}}.{{Letter}}."` pattern are to make it clear that an individual is being referred to. You'll see _M.C._, _J.C._, _B.P._, and _J.W.J._ No need to get uptight of there happen to be three initials. If certain of these early adopters agree to have their first names used, you might see names besides _Dave_'s. I might just keep the initials for privacy and security, anyway.

## Purpose and intended readers

This document records the current recommended procedure for creating Fort Point Upskilling Collaborations repositories that are quick to launch but meaningfully adapted to the learner. It is written for organization owners, mentors, future repository stewards, learners who want to understand the setup process, and AI assistants helping with repository preparation.

The goal is **automated-yet-bespoke setup**: reuse a safe, tested project scaffold where reuse helps, then change scope, guidance, code completion, and learning activities according to a participant's actual goals and experience.

## Continuation metadata

**Prepared at:**  
2026-10-21 (America/New_York)

**Built following a conversation between _Dave_ and ChatGPT**

**The chat involved other subjects** that will be important for the procedure, including

- [`fort-point-upskilling-collabs/fp-up-landing-page`](https://github.com/fort-point-upskilling-collabs/fp-up-landing-page) &mdash; the Fort Point landing page 
- `rubric-attribution-lab-mc-db-collab` (renaming from `rubric-attribution-lab-mc-collab` recommended) &mdash; _M.C._'s Rubric Attribution Lab
- `roman-numeral-word-lab-default-collab` &mdash; the default Roman Numeral Word Lab package
- planned _B.P._ and _J.C._ numeral-word collaborations that will work off of the default Roman Numeral Word Lab
- an upcoming walkthrough of _J.W.J._'s JabberVec letter2vec encoding vectorization training and visualization, which will lead to a good parts version of this guide to be found at `docs/COLLABORATION_SETUP_STEPS.md`, which you ~~can~~ `will (eventually)` go to directly by clicking ~~on this link~~~ `[holding spot for link when complete](dead-for-now)`. I think you will (and should) use that condensed version unless you need clarity on one of the points, and then you can click on the link `that will lead` back to this document.

## Author and source

**Prepared by:**  
David Black and kamMA (ChatGPT), from decisions developed collaboratively. **This procedure was conceived of and outlined by Dave and has been implemented with the help of AI.**

**Repository:**  
`fort-point-upskilling-collabs/fp-up-landing-page`

**Intended location:**  
`docs/context_documents/LN_fpucollab_2026-10-21_procedure01_-_bespoke-collab-setup-process.md`

**Branch or revision:**  
`main`; exact commit containing this document not yet known

## Procedure status and scope

This is Procedure 01: the first authoritative checkpoint for the collaboration-setup process. It describes current recommended practice, not immutable organization policy.

### Recommended, not mandatory

The naming pattern, document set, questionnaire route, and default-scaffold route are recommended conventions. Mentors may depart from them when a project's people, subject, schedule, accessibility needs, security boundaries, or learning goals call for something else. When an exception affects continuation or maintenance, document why it was chosen.

### Projects and collaboration shapes covered

The procedure supports one mentor and one learner, multiple mentors with one learner, one mentor with multiple learners, peer collaboration, and larger groups. Repository names identify the primary learner and primary repository steward when that is useful; they should not attempt to encode every participant.

### What this procedure does not standardize

It does not require one teaching method, programming language, editor, AI assistant, notebook style, testing philosophy, or final artifact. It also does not require every learner to complete a questionnaire before beginning.

## Roles and responsibilities

### Mentee or learner

The learner owns their learning goals, decides what personal information to share, performs and understands the work attributed to them, and participates in decisions about public release.

### Primary mentor or repository steward

The primary steward creates or supervises the repository, protects private information, keeps the initial scope finishable, verifies the scaffold, and makes the first handoff understandable.

### Additional mentors

Additional mentors may review code, supply domain knowledge, meet with the learner, or maintain parts of the project. Record them in repository documentation or access controls instead of continually lengthening the repository name.

### Organization owners and supporting members

Owners manage organization-wide settings and sensitive administration. Supporting members or mentor teams should receive only the permissions their work requires. Organization ownership is not a prerequisite for ordinary mentoring.

### AI assistants

AI assistants may help interpret questionnaire responses, reduce or expand scaffolding, write explanations and tests, and check repository consistency. They do not decide what a learner understands, what private material may be published, or whether generated historical and technical claims are reliable.

## Repository naming convention

### Recommended pattern

```text
{project-base}-{primary-mentee-initials}-{primary-mentor-initials}-collab
```

Examples:

```text
rubric-attribution-lab-mc-db-collab
roman-numeral-word-lab-bp-db-collab
roman-numeral-word-lab-jc-db-collab
jabbervec-l2v-jwj-db-collab
```

Use lowercase ASCII letters, numbers when needed, and hyphens. Two-letter initials are a convention, not an identity system; resolve collisions deliberately.

### Multiple mentors or multiple mentees

Use the initials of the primary learner and primary repository steward when there are clear primary roles. Describe everyone else in `README.md`, `CONTRIBUTORS.md`, repository access, or project records. For a true group project without meaningful primary roles, choose a short group marker rather than manufacturing a long combinatorial name.

### Acceptable exceptions

Legacy repositories may retain earlier names as useful history. Public-facing names may omit initials when personal attribution is inappropriate. Renaming an existing GitHub repository is normally preferable to deleting and recreating it because the repository history, settings, access, and redirects are preserved; local remotes should then be updated.

## Privacy and visibility defaults

### Private by default

Create participant-specific repositories as private unless there is a clear reason and informed agreement to begin publicly. Private-first development allows documentation, provenance, and attribution to be corrected before portfolio release.

### Personal information kept outside Git

Keep questionnaire answers, consent records, personal correspondence, credentials, and unnecessary biographical details outside the repository. A participant-specific context file may contain approved project-relevant preferences in a private repository, but it should not reproduce the questionnaire indiscriminately.

### Conditions for eventual public release

Make a repository public only after the learner agrees, secrets and personal information have been checked, third-party licenses and employer boundaries have been reviewed, attribution is accurate, and the repository makes sense to an unfamiliar reader.

## External intake materials

### External START_HERE document

An external `START_HERE_ext_{friend-name}.md` may explain the invitation, account setup, questionnaire, expected next action, and how the eventual private repository will be shared. This file exists before repository access (it's **ext**renal to the repo) and therefore should not depend on the recipient already knowing GitHub. `{friend-name}` is Dave's convention for the friend with whom he is collaborating, also referred to as the person being mentored. Examples could be any of the complete first names of _M.C._, _J.C._, _B.P._, _J.W.J._, or any of the other friend-collaborators who are interested.

### Bespoke project questionnaire

Use `BESPOKE_{friend-name}_PROJECT_ext_QUESTIONNAIRE.md` to elicit existing skills, learning goals, learning style, career goals, interests, available time, preferred tools, accessibility constraints, and desired balance between guidance and independent problem-solving. The questionnaire can remain substantially consistent across participants; the response drives customization. There is `[or soon will be]` a `BESPOKE_general_PROJECT_ext_QUESTIONNAIRE.md`, which will most often be usable as is; that is to say, mentors won't need to create their own questionnaire, though they can do so is they want. this general version can be used simply by downloading it, changing the filename to indicate the learning collaborator, and sending the learner the file via email or another method.

### GitHub account and two-factor authentication guidance

If the recipient does not have a GitHub account, provide a short account-creation route and current official security guidance. Encourage or require two-factor authentication according to organization settings. Do not assume an email invitation alone teaches Git, authentication, or repository navigation.

### Keeping questionnaire responses private

Questionnaire answers are planning inputs, not automatic repository content. Extract only the project-relevant conclusions needed for the learner's context and steps.

## Choosing the setup route

### Route A — Mentor-created bespoke repository

The mentor reviews the questionnaire, selects a project focus, adapts the scaffold and code, verifies it, creates the private repository, and invites the learner. This offers the strongest initial tailoring. Mentors are encouraged to partner with AI Assistants to turn a project idea into a starting scaffold or to create a back-near-the-start version of an existing, possibly completed repo or other project.

### Route B — Default scaffold customized after questionnaire review

Start with a tested, neutral default package. Use questionnaire answers to remove irrelevant options, change comments and incomplete functions, select exercises, and generate participant-specific context and steps. This is the present preferred route when several related collaborations are expected. Again, AI Assistant can be used to accelerate this process; both mentors and mentees should come away from a collaboration with better skills designing and coding with AI.

### Route C — Learner and AI customize the default scaffold

Give the learner the default scaffold, external guidance, and questionnaire. Instruct them to give their answers and selected project files to an AI assistant, request a participant context document and proposed `STEPS.md` (it's a good idea to include the `STEPS_default.md` to give the AI a useful point of reference,) and review the changes with a mentor. This supports higher demand for collaborations while retaining a personalization path.

### Route D — Begin immediately without a questionnaire

A learner may use `START_HERE.md` and `STEPS_default.md` directly. The questionnaire remains available later if they want more tailored scope. Avoid making introspection or AI use a tollgate in front of experimentation.

## Creating the default scaffold

### Neutral project objective

Define a coherent project question broad enough to support several learning paths but small enough to demonstrate. State what the default does and does not claim. In many cases, this can be a previously-completed or partially-implemented project, perhaps in an existing GitHub repository of the mentor. _Dave_ already has several project ideas viewable with `[short](get-url)` or `[long](get-url)` descriptions, and he hopes others will add their project ideas and previous projects in similar catalogs.

### Runnable reference implementation

Provide at least one small path that runs successfully. A learner should be able to distinguish environment problems from intentionally unfinished work. AI Assistants can give suggestions and even lead or complete the short runnable example.

### Intentional learning gaps

Leave work incomplete only when the gap serves an identified learning goal. Prefer a clear `NotImplementedError`, explicit warning, pseudocode, failing exercise test, or documented extension point over a silent `pass`. Do not fill every module with internal narration; comments should support rather than replace reasoning.

### Notebook, terminal, and interactive Python access

It is often helpful and appropriate include a guided Jupyter notebook that imports reusable modules, demonstrates the current project, and gives the learner a presentation-ready path. Jupyter notebooks are an especially good easy to present completed work in an attractive way for hiring managers and recruiters to see. A beginning Python learner should also be told that the same statements can be tried in the interactive Python prompt (`>>>` and `...`) with the necessary imports and correct working directory. Collapsible notebook notes may show equivalent PowerShell and Bash commands to access and use the REPL without overwhelming the main narrative.

### Tests and validation commands

Mentors might want to include a small automated test suite, a demonstration or smoke-test command, and validation for notebook or data structure where practical. If these don't already exist, the mentor can use their own AI Assistant to create them, learning step-by-step (or delegating to the AI) the complete coding of the test, demo, smoke-test, or validation. Record expected and observed results separately.

### Documentation and licensing

The default should normally include `README.md`, `START_HERE.md`, `STEPS_default.md`, `PROJECT_BRIEF.md`, `AI_ASSISTANCE.md`, provenance and safety guidance, a license, dependency information, and domain-specific references. Once again, mentors should consider using AI Assistants to complete these.

### Default ZIP archive

Create a ZIP with one enclosing project directory. Test the archive, calculate a SHA-256 checksum, and provide both to the steward. The checksum detects missing, stale, or corrupted downloads; it does not make untrusted content safe.

### Optional canonical default repository

A private canonical default repository is useful when the scaffold will evolve or generate several bespoke repositories. Customized participant repositories should normally be independent repositories rather than forks that expose an unwanted ancestry or permission relationship. This might be made clearer  by following the naming convention,

```text
{project-base}-{primary-mentee-initials}-{primary-mentor-initials}-collab
```

but changing it to

```text
{project-base}-default-collab
```

## Interpreting questionnaire responses

### Existing technical skills

Determine what the learner can already do independently and what they have only encountered. Do not infer mastery from a tool name alone.

Unless you have the time and inclination to do this all manually, we recommend having your AI Assistant help you perform this analysis more quickly.

Also remember that this landing page repository has `[or soon will have]` a `BESPOKE_general_PROJECT_ext_QUESTIONNAIRE.md` that a mentor can download as-is and simply rename to `BESPOKE_{primary-mentee-name}_PROJECT_ext_QUESTIONNAIRE.md`. If you do that, you can skip the following sections, since they are `[or will be]` covered in the `general` document.

### Learning goals

Identify the primary skill to practice and any secondary goals. These may range from Python fundamentals or basic mathematics to search algorithms, NLP evaluation, tensor reasoning, experiment design, or technical communication.

### Preferred learning style

Translate preferences into repository design: examples before abstractions, pseudocode before code, tests before implementation, notebook-first exploration, terminal practice, visual explanations, short milestones, or greater independent discovery.

### Career and portfolio goals

Choose a result that honestly signals the target skill. A quick portfolio win should still contain a clear question, reproducible method, learner-owned contribution, result, and limitation.

### Desired project scope

Separate an achievable first experiment from optional extensions. Do not make every interesting idea part of the minimum viable project.

### Available time and pacing

Adapt the number of modules, amount of setup, and milestone size. Prefer a finished narrow artifact to an impressive abandoned architecture.

### AI-assistance preferences

Ask whether the learner wants explanation, hints, code review, debugging, pair programming, generated examples, or fuller implementation help. Paid repository-connected assistants are optional.

### Accessibility and setup constraints

Account for operating system, hardware, installation permissions, command-line familiarity, connectivity, energy, scheduling, and any disclosed accessibility needs.

## Designing the bespoke version

### Selecting the learning path

Choose one primary route and make other possibilities visibly optional. Examples include Python foundations, algorithms, NLP analysis, data work, historical research, testing, or mathematical interpretation.

### Choosing what code is complete

Complete infrastructure that would distract from the target lesson, safety-critical validation, a small reference example, and enough integration for the learner to run the project.

### Choosing what code is scaffolded

Scaffold code central to the chosen learning goal. Adjust docstrings, type hints, pseudocode, tests, and error messages to the learner's level. Do not present guesses about types or APIs as authoritative.

### Choosing what the learner implements

Make ownership explicit. A beginner might construct mappings and simple functions; an experienced learner might design depth-first search, pruning, parsing, corpus analysis, evaluation, or visualization.

### Removing irrelevant branches and optional complexity

Bespoke design includes deletion. Remove modules, comments, options, and technologies that do not advance the selected goal. Store genuinely useful advanced branches in an `optional/` area only when their presence will not confuse the main route.

### Defining the smallest credible portfolio result

Write the stopping condition before expanding the project. The learner should know what counts as a first complete result.

## Internal repository documentation

### README.md

Explain the project to an outside reader: question, motivation, current demonstration, structure, reproducibility, attribution, status, and limitations.

### START_HERE.md

Maintain one internal `START_HERE.md`. It should orient the participant, identify the first session, link to their context and steps, explain how to use an AI helper without requiring a paid coding agent, and state privacy boundaries.

### PROJECT_BRIEF.md

State the research or engineering question, intended deliverable, scope, and out-of-scope temptations.

### STEPS_default.md

Keep the reusable baseline route and hints. It can help an AI assistant propose personalized steps, but it should not masquerade as the participant's final plan.

### Personalized STEPS.md

Create `STEPS.md` when questionnaire answers and mentor decisions justify a participant-specific sequence. Keep steps small, testable, and revisable.

### Participant context document

Summarize project-relevant goals, background, constraints, chosen learning path, and AI-assistance preferences without copying private responses unnecessarily. The participant should understand how this context will be used.

### AI_ASSISTANCE.md

Provide a lightweight place to record substantial AI assistance, the files or tasks affected, and what the learner decided or changed.

### Provenance, safety, and licensing guidance

Explain dataset and code sourcing, consent, privacy, licenses, credentials, employer boundaries, and domain-specific hazards.

### Mentor-only or optional materials

Mentor notes containing private planning should remain outside a public repository. Optional advanced material may live in the repository only when its purpose and audience are unmistakable.

## Avoiding onboarding-document proliferation

Do not create separate internal `START_HERE_int_{name}`, `START_HERE_int_gen`, and `START_HERE_int_default` files in every repository. Use one internal `START_HERE.md`, an optional participant context document, `STEPS_default.md`, and a personalized `STEPS.md` only when needed. Put organization-wide explanations in the landing page and link to them.

## Working effectively with AI assistants

### Repository-connected assistants are optional

A learner can work effectively by attaching or copying selected files into an ordinary chat. Do not imply that Claude Code, Codex, or another higher-cost connected tool is required.

### Supplying project and participant context

Begin with `START_HERE.md`, `PROJECT_BRIEF.md`, the approved participant context, and the specific file being changed. Supply `STEPS_default.md` when asking the assistant to propose personalized steps.

### Asking for explanations before complete solutions

Encourage requests for hints, examples, failing tests, pseudocode, code review, or an explanation of a trace before requesting full implementation.

### Requesting less-wordy scaffolding

Explicitly permit the learner to ask an AI helper to make a scaffold less verbose while preserving behavior, types, tests, safety notes, and learning goals. Review the resulting diff.

### Reviewing generated changes and preserving learner ownership

The learner should be able to explain important code and decisions. Generated output is a proposal until inspected and tested.

## Creating the collaboration repository

### Creating the private organization repository

Create an empty private repository under `fort-point-upskilling-collabs` using the agreed name. Avoid initializing remote files when a verified local scaffold will supply the first commit.

### Initializing or cloning locally

Clone the empty repository or initialize the prepared directory, use `main` as the default branch, and add the SSH remote used by the steward's configured GitHub account.

### Extracting the bespoke scaffold

Extract into a temporary directory first when the archive layout is uncertain. Copy the contents of the enclosing repository directory into the local clone. Do not overwrite an existing `.git/` directory.

### Verifying archive identity and contents

Compare the SHA-256 checksum, inspect the top-level layout, and run any supplied validation before committing.

### Committing and pushing the initial scaffold

Review `git status --short`, stage intended files, commit with a specific message, push `main`, establish upstream tracking, and confirm a clean working tree.

## Repository access and collaborator roles

### Inviting a mentee as an outside collaborator

For participant-specific work, normally invite the learner directly to the repository as an outside collaborator rather than making them an organization member. GitHub may resolve an email address to an existing username.

### Assigning Write access

Use `Write` when the learner should clone, push branches, and actively contribute. `Read` is insufficient for ordinary coding collaboration. Do not grant `Maintain` or `Admin` without a concrete need.

### Adding mentors through teams or individual access

Use a mentors team or direct repository access according to the expected duration and number of repositories. Mentors may need broader repository-management rights than learners without needing organization ownership.

### Confirming invitation acceptance

The access page may show an invitation as pending until accepted. Verify the resolved username, assigned role, and eventual acceptance rather than relying only on the invitation email.

### Verifying access from both accounts

The steward confirms administrative access and repository contents. The learner confirms that they can see the private repository and complete the first intended action.

## Initial technical verification

Verify repository structure, dependencies, tests, demonstration scripts, notebook syntax and imports, paths, optional-language components, and absence of accidental private material. Record exact commands and observed results in the participant repository or a setup checkpoint.

## First mentor–mentee handoff

Send the repository invitation and only the external files needed to understand it. Direct the learner to the internal `START_HERE.md` after access is accepted. Make the first task small enough to complete in one sitting and establish how questions, reviews, and scheduling will work.

## Data, intellectual-property, and participant safety

### Third-party code and data provenance

Record source, version, retrieval date, license, and modifications. Do not redistribute word lists, datasets, media, or code merely because they are easy to download.

### Employer and proprietary information

Keep employer-confidential material and independently created collaboration work separate. Do not use internal prompts, evaluations, data, code, or processes unless their use is explicitly authorized.

### Recording consent

Before recording interviews or paired work, obtain explicit permission from every participant. Consent to participate, consent to research use, and consent to public release of a recognizable voice are separate decisions. Offer distinct opt-ins for pre- and post-session audio and permit participation without public voice release.

### Credentials and secrets

Never commit tokens, passwords, private keys, consent records, private email, or sensitive configuration. Perform a secret and privacy check before public release.

## Collaboration workflow

Prefer small branches or commits, visible tests, bounded tasks, clear review, and periodic updates to the participant context and steps. Track substantial AI help. Define stopping points so optional extensions do not prevent a first finished result.

## Preparing a portfolio-quality result

A credible result includes a clear question, reproducible method, learner-owned contribution, tests or validation, observed result, limitations, provenance, and accurate attribution. Avoid inflated claims about originality, historical authority, model performance, or production readiness.

## Deciding whether to make the repository public

Before changing visibility, obtain learner agreement and conduct mentor or organization review. Check privacy, secrets, intellectual property, licenses, documentation, attribution, generated files, history where practical, and whether unfinished scaffolding could misrepresent the learner's contribution.

## Public release and portfolio handoff

After approval, change visibility, verify the public view while signed out when possible, and update the landing page or collaboration catalog. Help the learner write an accurate GitHub description, profile pin, résumé bullet, or LinkedIn description. Preserve both learner and mentor attribution without implying that mentoring code was authored independently by the learner.

## Maintaining the default and bespoke repositories

Feed generally useful fixes back into the canonical default without importing participant-specific material. Bespoke repositories remain independent: apply fixes deliberately rather than automatically synchronizing them. Archive or mark inactive projects clearly while preserving useful history.

## Fast path for multiple interested learners

When demand is high, distribute a verified default package with minimal external intake and a clear first task. Learners may use their questionnaire and an AI assistant to propose context and steps. A mentor reviews scope, safety, and the first portfolio milestone rather than rebuilding everything. A quick start can become more bespoke after work begins.

## Procedure checklist

### Before repository creation

- Confirm the project base name, primary learner, and primary steward.
- Select the setup route.
- Decide what information stays outside Git.
- Define the smallest credible result.
- Verify the default or bespoke scaffold.

### Before inviting the learner

- Confirm the repository is private.
- Verify the initial commit and clean working tree.
- Run tests and the demonstration path.
- Check `START_HERE.md` from the learner's perspective.
- Assign the least role that supports the intended work, normally `Write`.

### Before the first handoff

- Send the correct external guidance.
- Confirm invitation acceptance and repository visibility.
- Identify one concrete first task.
- Establish how and when review will occur.

### Before public release

- Obtain learner agreement.
- Review privacy, secrets, IP, licenses, and provenance.
- Verify tests and reproducibility.
- Clarify learner and mentor contributions.
- Update public catalogs only after the repository is ready.

## Current authoritative state

- The public organization profile and `fp-up-landing-page` repository exist.
- The landing page contains organization documents, project catalogs, and context-document guidance.
- Maya's private Rubric Attribution Lab scaffold has been committed and pushed; Maya was invited with `Write` access as an outside collaborator. Renaming it to `rubric-attribution-lab-mc-db-collab` is recommended for the current naming pattern.
- A verified `roman-numeral-word-lab-default-collab.zip` exists with SHA-256:

```text
d99f6f4fed9876aa635c8d7c5b45b6cf00428c61cfddef900ce590a4414475a6
```

- The default numeral-word package contains a runnable Roman-numeral example, DFS search, tests, notebook, optional C++ validator, and mentor customization guidance.
- Planned bespoke numeral-word repositories are `roman-numeral-word-lab-bp-db-collab` for Brian and `roman-numeral-word-lab-jc-db-collab` for Justin.
- Brian's intended emphasis is Python learning and foundational construction. Justin's intended emphasis is stronger Python, NLP, search, and analysis. Final designs await questionnaire responses and review of planning material.

## Open procedural questions

- Should a canonical default repository be created for every reusable project family, or only after a second participant appears?
- Which organization-wide instructions belong in the landing page rather than being linked or repeated in participant repositories?
- Should mentor access be standardized through a `mentors` team, and what repository-creation or maintenance permissions should that team receive?
- What minimum evidence is required before a repository is declared portfolio-ready?
- How should group projects be named when there is no meaningful primary learner or steward?

## Immediate next steps

1. Save this document under `fp-up-landing-page/docs/context_documents/` and commit it after review.
2. Rename Maya's repository and update the local remote if the current naming convention is adopted immediately.
3. Inspect and publish the default numeral-word scaffold as a private canonical repository if desired.
4. Review Brian's questionnaire and derive `roman-numeral-word-lab-bp-db-collab`.
5. Review Justin's questionnaire and derive `roman-numeral-word-lab-jc-db-collab`.
6. Create separate `proclearningsNN` checkpoints when lessons are worth preserving without expanding this procedure document.

## Definition of the next stopping point

The next procedure checkpoint is warranted after at least Brian's and Justin's repositories have been derived from the same default, launched privately, and used enough to identify which parts of this workflow saved time, created confusion, or required exceptions. Before then, record significant observations in dated `proclearningsNN` documents.

*END: Context Document*

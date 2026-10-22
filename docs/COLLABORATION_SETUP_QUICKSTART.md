# Collaboration Setup Steps

> This is the short, practical version of the Fort Point bespoke-collaboration setup process. For rationale, exceptions, privacy details, and fuller guidance, see the [complete procedure](context_documents/LN_fpucollab_2026-10-21_procedure01_-_bespoke-collab-setup-process.md).

The aim is simple: start from a project idea or existing project, use AI to accelerate the repetitive setup work, and adapt the result to one learner without requiring either the mentor or learner to surrender judgment or understanding.

These are recommended steps, not mandatory rules.

## Files used in the process

The process normally uses:

- `BESPOKE_general_PROJECT_ext_QUESTIONNAIRE.md`: a reusable questionnaire sent before repository access;
- `START_HERE_ext_{friend-name}.md`: optional external invitation and GitHub guidance;
- `{project-base}-default-collab.zip`: a neutral, tested starting repository;
- `START_HERE.md`: the learner's first internal repository document;
- `STEPS_default.md`: a reusable starting plan and input for AI customization;
- `STEPS.md`: the learner's customized working plan, when useful; and
- an approved learner/project context document containing project-relevant conclusions rather than private questionnaire details.

Not every collaboration needs every file.

## The process at a glance

1. Choose a project or project family.
2. Ask an AI assistant to help create a neutral default scaffold.
3. Test the default and package it as a ZIP.
4. Send the general questionnaire to the learner.
5. Use the responses to identify a suitable learning path.
6. Ask an AI assistant to produce a bespoke version of the scaffold.
7. Test and review the bespoke ZIP.
8. Create a private organization repository and push the files.
9. Invite the learner, normally as an outside collaborator with `Write` access.
10. Help the learner use their own AI assistant to propose a personalized `STEPS.md`.
11. Work in small, visible, testable increments.
12. Review privacy, intellectual property, attribution, and readiness before making the repository public.

## Step 1 — Choose a project

The mentor and learner may begin with:

- a new idea;
- a project from the Fort Point catalog;
- an unfinished mentor project;
- a completed project moved back near its beginning; or
- a neutral default scaffold already created for other learners.

Choose a first result that can be finished. Interesting extensions can remain visible without becoming prerequisites.

## Step 2 — Give the source material to an AI assistant

The mentor may provide an existing repository, selected files, planning notes, or a project description. Ask the AI assistant to inspect the material before changing it.

A useful request is:

> Help me turn this project into a neutral teaching scaffold. Preserve one small runnable example, tests or validation, and enough documentation to distinguish working infrastructure from intentional learner exercises. Do not personalize it yet.

The mentor should review the proposed structure and decide what belongs in the default. AI assistance is part of the mentor's learning process too: delegation, inspection, correction, and testing are skills.

## Step 3 — Create and verify the default ZIP

The default should normally provide:

- one obvious starting point;
- one runnable demonstration;
- intentional, clearly marked learning gaps;
- `README.md`, `START_HERE.md`, and `STEPS_default.md`;
- installation or environment guidance;
- a small test or validation path; and
- appropriate licensing, provenance, privacy, and AI-assistance guidance.

When useful, include a guided Jupyter notebook and equivalent terminal or Python-REPL hints. Repository-connected paid assistants are optional; ordinary AI chat with pasted or attached files can be enough.

Before distributing the ZIP:

1. inspect its file tree;
2. run its tests and demonstration;
3. test the archive itself;
4. calculate a SHA-256 checksum; and
5. record the observed results.

A canonical private `{project-base}-default-collab` repository is useful when more than one bespoke repository will be derived from the scaffold.

## Step 4 — Send the external questionnaire

Download `BESPOKE_general_PROJECT_ext_QUESTIONNAIRE.md`, rename its copy for the learner, and send it by email or another private channel. Add an external `START_HERE_ext_{friend-name}.md` when the learner may need GitHub-account, two-factor-authentication, invitation, or first-login help.

The questionnaire should reveal enough to choose scope and teaching style, including:

- current skills;
- primary and secondary learning goals;
- preferred ways of learning;
- career or portfolio goals;
- available time;
- desired balance between guidance and independent work;
- preferred AI-assistance style; and
- relevant setup or accessibility constraints.

Questionnaire answers remain private planning material unless the learner approves a specific use.

## Step 5 — Ask AI for a short interpretation

The mentor gives the questionnaire responses to an AI assistant and asks for a concise, evidence-based interpretation—not a personality diagnosis.

For example:

> From these responses, identify the learner's likely starting level, primary learning objective, useful teaching style, smallest credible first result, and repository changes that would support those conclusions. Separate statements supported by the answers from your suggestions.

The mentor corrects mistaken assumptions and chooses the actual project path.

## Step 6 — Create the bespoke ZIP

Give the AI assistant:

- the verified default scaffold;
- the short questionnaire interpretation;
- any approved learner/project context;
- the intended first result; and
- any mentor decisions that override the default.

Ask it to create the bespoke repository package. Appropriate changes may include:

- removing irrelevant branches;
- changing which code is complete or scaffolded;
- adjusting comments and hints;
- selecting notebook, terminal, testing, mathematical, or visual emphasis;
- adding comparisons with a language the learner already knows;
- choosing useful intermediate output; and
- making the first run rewarding and understandable.

Keep one internal `START_HERE.md`. Avoid multiplying default, general, and named internal start files.

## Step 7 — Review and test the bespoke package

The mentor should inspect the diff from the default and verify:

- the first run works;
- unfinished work fails or warns clearly rather than silently;
- the tests match the intended learner tasks;
- comments support the learner without solving every exercise;
- private questionnaire details were not copied into the repository;
- dependencies and commands are accurate; and
- the result remains small enough to finish.

Package the reviewed repository as a new ZIP and calculate its checksum.

## Step 8 — Create the private collaboration repository

Recommended naming pattern:

```text
{project-base}-{primary-mentee-initials}-{primary-mentor-initials}-collab
```

The initials identify the primary learner and primary repository steward, not every participant. Record additional mentors and contributors in repository access and documentation.

Create an empty **private** organization repository. Clone or initialize it locally, copy in the verified scaffold without replacing `.git/`, review `git status`, commit, push `main`, and confirm a clean working tree.

## Step 9 — Invite the learner

Normally invite the learner as an outside collaborator with `Write` access. Confirm that GitHub resolved the correct account, the invitation was accepted, and both mentor and learner can see the private repository.

Then direct the learner to the repository's `START_HERE.md`.

## Step 10 — Let the learner and their AI customize the working plan

The learner can give their AI assistant:

- `START_HERE.md`;
- `PROJECT_BRIEF.md`;
- their approved context document;
- `STEPS_default.md`; and
- the specific files involved in the first task.

They can ask:

> Help me propose a `STEPS.md` suited to my stated goals and learning preferences. Keep the first steps small and runnable. Explain what I should learn or decide at each step. Do not complete the whole project for me.

The mentor and learner review the proposal together. `STEPS.md` is a working plan, not a contract; revise it when the project teaches something unexpected.

## Step 11 — Work in small increments

Prefer small tasks, commits, demonstrations, and reviews. The learner may ask their AI assistant for explanations, traces, examples, pseudocode, tests, debugging help, or full code when that matches the agreed learning goal.

Record substantial AI help in `AI_ASSISTANCE.md`. The important question is not whether AI was used, but whether the learner can explain the work, evaluate the output, and make meaningful decisions.

## Step 12 — Prepare for public release

When the project has a credible first result, review it with the learner. Before changing visibility, check:

- learner agreement;
- secrets and personal information;
- employer and intellectual-property boundaries;
- data and code licenses;
- provenance and attribution;
- tests and reproducibility;
- clarity about learner and mentor contributions; and
- whether unfinished scaffolding could misrepresent the learner's work.

After approval, make the repository public, inspect the public view, update the Fort Point landing page or catalog, and help the learner describe and pin the project accurately on GitHub. A résumé or LinkedIn description should name the learner's real contribution without hiding mentorship or inflating the result.

## Worked example — A JabberVec collaboration

This example illustrates the process without prescribing another learner's project.

1. _D.B._ supplies an existing, partially implemented `jabbervec-l2v` repository to an AI assistant.
2. _D.B._ and the assistant derive and test a neutral `jabbervec-l2v-default-collab.zip` before personalizing it.
3. _D.B._ sends the external questionnaire to _J.W.J._
4. After receiving the answers, _D.B._ asks the assistant for a short learning-oriented interpretation and corrects it using his direct knowledge of _J.W.J._
5. The assistant derives `jabbervec-l2v-jwj-db-collab.zip` from the verified default.
6. The bespoke first run produces immediately inspectable character-level output before requiring neural-model training.
7. The scaffold may use carefully selected Java comparisons to bridge into Python, visible intermediate output, and optional paths toward vectorization, learned character embeddings, PCA or other projections, and low-rank analysis.
8. _D.B._ tests the package, creates the private repository `jabbervec-l2v-jwj-db-collab`, pushes it, and invites _J.W.J._ with `Write` access.
9. _J.W.J._ gives his approved context and `STEPS_default.md` to his AI assistant and asks for a personalized `STEPS.md`.
10. Mentor, learner, and AI work through small runnable steps. The learner can continue into deeper experiments or stop after a finished portfolio result.
11. After review and agreement, the repository can become public and be pinned to _J.W.J._'s profile, with possible next experiments left as invitations rather than unfinished obligations.

## The shortest acceptable version

When time or mentor capacity is limited:

1. send the general questionnaire;
2. use AI to summarize the learning needs;
3. use a tested default ZIP;
4. ask AI to make only the few justified bespoke changes;
5. test the first run;
6. create the private repository and invite the learner;
7. let the learner's AI propose `STEPS.md`; and
8. review the first result and public-release decision with a human mentor.

That is enough to begin. Further bespoke work can emerge from the collaboration itself.

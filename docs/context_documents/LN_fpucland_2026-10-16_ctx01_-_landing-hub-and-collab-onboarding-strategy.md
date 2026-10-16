*BEGIN: Context Document Header*

# CONTEXT DOCUMENT — Continuation

## Project

**Name:**  
Fort Point Upskilling Collabs landing hub and collaboration onboarding system (`fpucland`)

**Description:**  
This work establishes the public GitHub presence, project catalogs, collaboration documentation, and reusable onboarding pattern for Fort Point Upskilling Collabs. The immediate implementation target is the first private, participant-ready Rubric Attribution Lab collaboration package.

## Continuation metadata

**Prepared at:**  
2026-10-16T09:19:18-04:00

**Continued from:**  
`Upskilling_Create_Colab_Repos`

**Also involving:**

- GitHub organization setup and security
- Public organization profile and landing-page repositories
- Participant onboarding and AI-assisted project customization
- Rubric Attribution Lab
- Pocket Cocktail Party
- Symbol-to-word search, JabberVec, and multilingual authorship projects

## Author and source

**Prepared by:**  
Dave Black with kamMA / ChatGPT

**Repositories:**

- `fort-point-upskilling-collabs/.github`
- `fort-point-upskilling-collabs/fp-up-landing-page`
- planned private collaboration repositories under `fort-point-upskilling-collabs`

**Branch or revision:**  
`fp-up-landing-page`, branch `main`, verified through commit `f5760918` (`Including correct context document README`).

## Intent for this context

Allow a new conversation to resume the organization and collaboration-repository work without reconstructing decisions from the original chat. Preserve the simplified onboarding architecture before building the first participant-specific repository so that later projects remain fast to generate without multiplying confusing entry documents.

*END: Context Document Header*

---

## Authoritative current state

### Organization

The GitHub organization is:

```text
fort-point-upskilling-collabs
```

The organization is intended for mentored, hands-on machine learning, data science, software, AI-evaluation, language, audio, research, and documentation projects. Working collaboration repositories are generally private during early work. Public summaries and participant-approved results may be published later.

Organization security and Actions defaults were reviewed during the originating chat. Relevant current decisions include:

- Require secure two-factor authentication only after accepted members are verified as compliant.
- Prefer passkeys, hardware keys, authenticator applications, or GitHub Mobile over SMS.
- Keep repository administrator access limited; ordinary collaborators normally receive Write access.
- GitHub Actions permits actions created by GitHub and verified Marketplace creators under the selected restricted policy.
- Default workflow token permissions are read-only for repository contents and packages.
- GitHub Actions may not create or approve pull requests by default.
- Repository-level self-hosted runners are disabled; standard hosted runners are enabled.

### Public `.github` repository

The public repository:

```text
fort-point-upskilling-collabs/.github
```

contains:

```text
.gitignore
LICENSE.md
assets/fp-up-logo.png
profile/README.md
```

GitHub displays `profile/README.md` on the organization overview page. It contains the large organization logo, mission, links, participation principles, security guidance, and contact information.

The profile already links to project catalogs and landing-page documents, but the links appear as ordinary bullets beneath `## Start here`. A conspicuous H2-level link to the landing hub is still required.

The `.github` repository is also the eventual home for organization-wide default community-health files:

- `CODE_OF_CONDUCT.md`
- `CONTRIBUTING.md`
- a future `SECURITY.md`
- future issue and pull-request templates

Do not move catalogs, active-collaboration records, questionnaires, or detailed onboarding documentation into `.github`. Those belong in the landing hub.

### Public landing-page repository

The public repository:

```text
fort-point-upskilling-collabs/fp-up-landing-page
```

was created and pushed successfully. Its local Termux checkout is:

```text
~/org_repos_dwb/fp-up-landing-page
```

Verified tracked files include:

```text
.gitignore
CODE_OF_CONDUCT.md
COLLABORATIONS.md
COMMUNITY.md
CONTRIBUTING.md
LICENSE.md
README.md
assets/fp-up-logo.png
catalogs/FP-up_LONG_Catalog_2026-09-28.md
catalogs/FP-up_SHORT_Catalog_2026-09-28.md
docs/context_documents/README.md
```

The accidental space in the short-catalog filename was removed. The corresponding `%20` in the landing README link was also removed. The user checked both filenames and repository text for remaining literal spaces or `%20` escapes and found none relevant.

The landing repository's context-document guide is published at:

```text
docs/context_documents/README.md
```

It defines continuation-ready lab-notebook documents, the `LN_*` naming system, a reusable context template, an optional pre-context-document prompt, privacy rules, and retrieval guidance.

### Branding and licensing

The organization logo is a large square PNG featuring the `FP` mark, an upward arrow, Boston imagery, and the words “Fort Point Upskilling Collaborations.” Copies are stored in both public repositories because each README needs a stable relative image path.

Public text and original artwork are currently described as Creative Commons Attribution 4.0 unless otherwise noted. Individual software collaboration repositories may require a separate software license appropriate to their contents.

## Repository responsibilities

### `.github`

Use for:

- the concise organization-facing profile;
- prominent navigation to the project hub;
- organization-wide community-health defaults; and
- issue and pull-request templates that should apply when individual repositories do not override them.

Avoid maintaining detailed lists here if an authoritative list already exists in the landing repository. In particular, the active-collaboration table in the organization profile may eventually be removed or replaced with a link to prevent drift.

### `fp-up-landing-page`

Use as the public handbook and canonical information hub for:

- short and long project catalogs;
- active collaboration status;
- opt-in community recognition;
- contribution and participation information;
- public onboarding resources;
- general questionnaires and prompts;
- context-document guidance; and
- public templates for creating collaboration packages.

### Private collaboration repositories

Use for:

- participant-specific project scaffolding;
- private questionnaire-derived context when approved;
- working code, experiments, issues, and pull requests;
- project-specific steps and checkpoints; and
- private discussion or artifacts that are not ready for public release.

## Simplified bespoke cookie-cutter collaboration strategy

### Design goal

Create collaboration repositories quickly enough to serve multiple interested participants while still adapting each experience to the participant's goals, background, learning preferences, time, and desired project focus.

The system must avoid two opposite failures:

1. **Cookie-cutter without care:** every participant receives the same generic repository regardless of needs.
2. **Cathedral onboarding:** the participant must understand many overlapping documents, answer an extensive questionnaire, and wait for major customization before doing any project work.

The chosen design provides a working default path immediately and treats customization as an enhancement rather than an entrance requirement.

### Three participant routes

#### 1. Named bespoke route

A known participant receives two documents outside the repository:

```text
START_HERE_ext_{{friend-name}}.md
BESPOKE_{{friend-name}}_PROJECT_ext_QUESTIONNAIRE.md
```

The external start document explains account/access preparation, the project choice, what the questionnaire is for, and what will happen next. The questionnaire gathers the participant's goals, current experience, learning preferences, available time, desired difficulty, interests, preferred AI assistant, and desired project outcome.

Dave and kamMA use the answers to prepare:

- a concise participant/project context document;
- a tailored repository scaffold;
- one obvious internal `START_HERE.md`; and
- when useful, an initial personalized `STEPS.md`.

Questionnaire answers and participant-specific context must not be placed in a public repository without explicit informed approval.

#### 2. Guided general route

An interested person without a completed bespoke intake uses public general versions from the landing hub. The general questionnaire may help the person choose among projects as well as describe how they learn.

The participant may give the completed questionnaire and a documented prompt to an AI coding assistant. The assistant can then propose:

- a participant/project context document;
- a tailored `STEPS.md`; and
- limited goal-based edits to the repository scaffold.

The assistant should preserve the default runnable path and should not redesign the entire repository merely because customization is possible.

#### 3. Immediate default route

A participant who does not want to complete a questionnaire can start immediately from the repository's default path. The default repository must therefore be usable, understandable, and testable without participant context or AI assistance.

### Entry-document rule

Earlier brainstorming produced several possible internal files such as:

```text
START_HERE_int_{{name}}.md
START_HERE_int_gen.md
START_HERE_int_default.md
```

That approach was deliberately simplified. A delivered repository should expose **one obvious internal entry point**:

```text
START_HERE.md
```

The contents of that file may be bespoke, guided-general, or default depending on the delivered package, but the participant should not have to choose among several competing start documents.

At most one optional customization path should be linked from the main start document. Alternative templates may exist in a clearly marked maintainer/template location, but they should not compete for attention at repository root.

### Steps rule

Every starter repository should provide:

```text
STEPS_default.md
```

This is the guaranteed, immediately usable route. It should contain small milestones, verification commands, and clear stopping points.

A customized repository may additionally provide:

```text
STEPS.md
```

`STEPS.md` may be created by Dave and kamMA or proposed by the participant's AI assistant using the approved context document and `STEPS_default.md`. The customized file may reorder, explain, narrow, or extend the default plan, but it must not quietly remove the runnable baseline.

### Context-document role

Participant/project context should tell the selected AI assistant:

- who the learner is in project-relevant terms;
- what the learner wants to practice or produce;
- what support style is useful;
- what should not be assumed;
- the project scope and current repository state;
- what files are scaffolds, partial implementations, or completed references;
- how much code should initially be supplied versus left for the participant; and
- the next concrete task.

Context is meant to preserve intent and reduce re-derivation. It is not permission for an AI assistant to replace the participant's learning with automatic completion.

### Default collaboration package

A project-family starter package will normally contain:

```text
README.md
START_HERE.md
STEPS_default.md
PROJECT_BRIEF.md
CONTRIBUTING.md
AI_ASSISTANCE.md
LICENSE or LICENSE.md
requirements.txt or equivalent environment specification
src/ or project-specific implementation directories
tests/ or validation scripts
data/ or documented data placeholders when appropriate
docs/
optional/
```

Not every repository needs every path. `optional/` is for genuine extensions, alternate scaffolds, or deeper material that should not obstruct the default path.

### Package generation model

The intended workflow is:

```text
project-family baseline
    -> external named or general intake
    -> questionnaire response (optional)
    -> participant/project context
    -> bounded scaffold edits
    -> one START_HERE.md
    -> STEPS_default.md plus optional STEPS.md
    -> private collaboration repository
```

Do not create every repository from nothing. Maintain tested project-family baselines and transform them deliberately.

## Initial collaboration rollout

The first end-to-end prototype is the Rubric Attribution Lab. It should test the external start document, external questionnaire, participant/project context, internal entry point, default steps, repository scaffold, and private GitHub invitation flow.

After the first prototype, likely project families include:

- Pocket Cocktail Party: audio source separation, synthetic mixtures, and FastICA;
- symbol-to-word depth-first search using chemical symbols, Greek numerals, Cyrillic numerals, and optional Roman-numeral constraints;
- JabberVec/Jabberwock character and language representation experiments; and
- multilingual authorship and translation comparison, including Tolstoy/Dostoevsky and French/English/Russian boundaries.

Participant names should not appear in this public continuation document unless public listing permission has been obtained.

## Current Rubric Attribution Lab materials

The originating environment retains:

```text
rubric-attribution-lab-collab.zip
RUBRIC_ATTRIBUTION_LAB_START_HERE.md
rubric-attribution-lab-collab/
```

The unpacked repository currently includes at least:

```text
README.md
PROJECT_BRIEF.md
LEARNING_AND_COLLABORATION_QUESTIONNAIRE.md
AI_ASSISTANCE.md
PROVENANCE_AND_SAFETY.md
LICENSE
requirements.txt
analysis/REPORT_TEMPLATE.md
data/DATA_DICTIONARY.md
data/case_analysis.csv
data/responses/
experiment/PROMPT_AND_CONVERSATION.md
experiment/SUPPLIED_RUBRIC.md
scripts/plot_results.py
scripts/validate_cases.py
```

These materials predate the simplified onboarding architecture and must be inspected rather than blindly pushed. In particular, the questionnaire currently inside the repository should be evaluated for conversion into the external named questionnaire, and the old external start file should be compared against the new one-entry-point strategy.

## Decisions and rationale

- **Landing hub is canonical for public onboarding.** It is easier to browse and can evolve independently of the compact organization profile.
- **`.github` remains the front door and defaults repository.** GitHub gives this repository special behavior; it should not become the full handbook.
- **One internal `START_HERE.md`.** Multiple root-level variants create choice paralysis and maintenance drift.
- **Questionnaire is optional for starting.** Personalization must not block useful work.
- **Named questionnaire lives outside the initial repository.** It can shape the repository before access and avoids embedding private answers or intake mechanics in the learner's workspace.
- **`STEPS_default.md` is always viable.** AI-generated customization is an optional overlay, not a dependency.
- **Public recognition is opt-in.** Names, interests, and collaboration links appear publicly only with permission.
- **Private-by-default working repositories.** Early experiments and participant-specific context remain private until participants approve public artifacts.
- **Project-family baselines are reusable.** Reuse enables rapid onboarding without removing human judgment.

## Commands and verification

### Landing-page repository

```bash
cd ~/org_repos_dwb/fp-up-landing-page
git status
git log -1 --oneline
find . -type f -print
grep -iIRHn '%20' .
```

**Observed results:**

- Commit `f5760918` pushed successfully to `origin/main`, correcting the context-document README after the earlier `c0d60f0` update.
- Local branch reported up to date with `origin/main`.
- Working tree reported clean.
- Corrected short catalog exists as `FP-up_SHORT_Catalog_2026-09-28.md`.
- No remaining `%20` reference was reported by the user's check.

### Organization-profile repository

```bash
cd ~/org_repos_dwb/.github
git status
```

Before editing, confirm the working tree is clean. Then add the prominent project-hub link beneath the centered introductory block in `profile/README.md`, inspect the diff, commit, and push.

## Constraints, risks, and privacy

- Both `.github` and `fp-up-landing-page` are public. Never place questionnaire answers, private emails, employer information, credentials, recovery codes, or participant-specific context in them without explicit approval.
- `docs/admin_notes/` in a public repository is public regardless of its name. Private administration notes require a private location.
- Empty directories are not tracked by Git.
- Duplicate active-collaboration tables can drift; prefer one authoritative detailed list.
- Duplicate default community-health files can drift; later decide whether the landing copies are mirrors, links, or project-specific overrides.
- GitHub Markdown does not offer arbitrary reliable text coloring. Visibility should come from heading level, placement, concise wording, emoji used sparingly, and bold linked text.
- Repository customization must remain bounded. Do not let AI-generated changes erase the default runnable path or complete all intended learning tasks for the participant.

## Open questions

- What exact questions should remain in the general questionnaire versus project-family questionnaires?
- Which parts of the current Rubric Attribution Lab scaffold should be completed examples, partial implementations, or learner tasks?
- Should the public landing repository keep full copies of `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md` after defaults are added to `.github`, or should it link to the canonical defaults?
- What public artifacts, if any, should be extracted from each private collaboration repository?
- What minimum information is needed to generate a useful participant/project context without making intake burdensome?
- Which aspects of AI-assistant behavior belong in `AI_ASSISTANCE.md`, the context document, and `START_HERE.md` respectively?

## Immediate next steps

1. Add a conspicuous H2-level project-hub link near the top of `.github/profile/README.md`; inspect, commit, push, and verify it on the organization overview.
2. Add this context document to `fp-up-landing-page/docs/context_documents/` and commit it when the public-safe content is approved.
3. Inspect the existing Rubric Attribution Lab archive and identify what is kept, moved outside, renamed, simplified, or removed.
4. Draft the first named external start document and external questionnaire without publishing participant-specific information.
5. Produce a participant-ready Rubric Attribution Lab archive with one internal `START_HERE.md` and a viable `STEPS_default.md`.
6. Create or populate the private Rubric Attribution Lab collaboration repository and invite the participant with appropriate access.

## Definition of the next stopping point

The next meaningful checkpoint is reached when:

- the organization overview has a visually prominent link to the public project hub;
- the current public continuation document is safely stored;
- the Rubric Attribution Lab package has one clear internal entry point;
- its external start document and questionnaire are separated from the repository;
- the default project path can be followed without completing the questionnaire; and
- the private collaboration repository is ready for its first participant invitation.

*END: Context Document*


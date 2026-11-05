# norsk-job-hunt

Single source of truth for Tiger's Norwegian job search. Doctrine, journey, CVs, pipeline and playbooks live here as markdown so each session loads only the file it needs and edits by diff, instead of regenerating PDFs and Word files.

## How to use this repo in a session

1. Start with `CLAUDE.md` (short bootstrap, always read).
2. Load only the files the task needs. A new application usually needs:
   - `05-playbooks/application-workflow.md`
   - the CV variant named in `03-cvs/variants.md`
   - `01-doctrine/honesty-locks.md`
3. Log the outcome in `04-pipeline/applications.md`.
4. Render to PDF only at the final step, once, from the markdown.

## Map

| Folder | What it holds | Load when |
|---|---|---|
| `00-journey/` | How the strategy evolved, what failed, what worked | Strategy questions, retros |
| `01-doctrine/` | TIGER_ANIMA_v5.0_UNIFIED (master doctrine), TIGER_OUTREACH_ENGINE_v1.0 (weekly cadence), the lenses, HR/red-team view, honesty locks | Writing any letter, CV, answer |
| `02-profile/` | Verified fact base and research assets | Building or checking any claim |
| `03-cvs/` | CV variants in markdown and the routing rule | Every application |
| `04-pipeline/` | Applications log, contacts, outreach ledger | Every application, weekly review |
| `05-playbooks/` | Step-by-step workflows and skip rules | Every application |
| `templates/` | Job intake template | New posting |

## Privacy rule for this repo

This repo is public. Never commit: phone number, street addresses, fødselsnummer, references' emails or phones, permit or immigration details, confidential EcoTrain material. Those go in the application itself at render time, from a local file outside git.

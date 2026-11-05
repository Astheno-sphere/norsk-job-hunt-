# Red-team protocol (dynamic variables)

The red team changes its weights by the job. Step 1 sets the variables from the posting; every later step reads them. Used by `.claude/agents/red-team.md` or inline.

## Step 1: Set the variables (from the posting and `templates/job-intake.md`)

| Variable | Values | Drives |
|---|---|---|
| `role_tier` | trainee / coordinator / specialist / strategic | Overqualification weight, letter altitude, page count |
| `company_style` | traditional-NO / international / public-sector / startup | Personal details, tone, photo, hobbies (C3) |
| `working_language` | NO-required / NO-preferred / EN | Language gate, CV language (C1) |
| `cv_language_risk` | low / medium / high | Norwegian CV with sub-B1 level against a Norwegian ad = high |
| `experience_cap` | none / total-years / post-grad-years | Which roles may appear; STARZZ-only vs procurement back in |
| `sponsorship_stance` | stated-yes / silent / stated-no | Kill filter weight; stated-no = recommend skip |
| `channel` | warm / recruiter / kontaktperson / portal | Whether a pre-apply call or note is mandatory |
| `domain` | maritime / offshore / energy / fleet / datacentre / procurement / other | Which research asset (one) and which HiMolde modules |
| `reader` | HR screener / hiring manager / panel / recruiter | Six-second scan vs depth read |

Print the variable block at the top of every review.

## Step 2: Kill filters (score each 0 to 3; any 3 = reject risk)
1. Work authorization: weight x3 if `sponsorship_stance` = stated-no or silent at a small firm.
2. Language gate: `working_language` vs locked Norwegian level.
3. Overqualification / flight risk: weight x2 if `role_tier` = trainee or coordinator. Check MSc prominence, research links, thesis framing, "four years".
4. Scatter: more than one placement identity on the page.
5. Fit-for-level: titles pitched above or below the role.
6. Letter/CV mismatch: any role, date, number in one and not the other.
7. Missing commitment signal: no stay/learning-Norwegian/why-Norway line (Thorsdottir).
8. Unverifiable claim: anything Tiger cannot defend for five minutes.
9. Generic: could this letter go to ten companies unchanged?
10. Task-word miss: fewer than half the posting's task words reflected.
11. No call made: ad names a contact person and the letter shows no sign of a call (Ramsli). Weight x2 for portal channel.

## Step 3: Score
- Start at 100. Subtract: kill filter score x weight x 3.
- Report: final score, the one-line hiring-manager reaction, and verdict: SEND / FIX THEN SEND / WRONG VARIANT / SKIP.

## Step 4: Surgical fixes (max 7, ranked)
Format each as:

```
P0|P1|P2  [CV|Letter]  section
- old: exact current line
+ new: exact replacement
why: one line, which filter it closes
```

P0 = would cause rejection. P1 = weakens. P2 = polish. Never more than 2 P2s.

## Step 5: Pre-send moves (from recruiter intel)
- Ad names a kontaktperson: draft the 3-step call script from `06-recruiter-intel/alisa-ramsli.md` section 1, tailored to this ad.
- Always: the follow-up plan (call the contact person 1 to 2 weeks after the søknadsfrist; after an interview, ask the decision date).
- `company_style` = traditional-NO: one human line (hobby, why Norway).

## Step 6: What survives
Two to four lines on what is genuinely strong and must not be cut.

## Escalation
- High-stakes or `role_tier` = specialist/strategic: run the agent cold (a fresh session without the friendly drafting history).
- Honest ceiling: we cannot guarantee a pass. We guarantee only structural risks can fail it.

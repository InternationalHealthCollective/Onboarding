# Working in the IHC GitHub organization

Rules for everyone who works in the InternationalHealthCollective organization.

## 1. What goes on GitHub

| GitHub | Google Drive |
|---|---|
| Code: Apps Script, add-ons, websites, scripts, notebooks | Forms, responses, spreadsheets, reports, slides |
| Docs needed to run the code: READMEs, handoffs, deploy notes | Meeting notes, minutes, transcripts |
| Synthetic sample data (`examples/`) | Anything with real patient, applicant or staff data |

The project repositories are **public**. Never commit real data or secrets: Git keeps history, so a deleted file is
still there.

## 2. Structure

- **One repository per project**, kebab-case name. An org owner creates new ones.
- Each has `README.md` (what it is, owner, how to run and deploy), `HANDOFF.md`, `.gitignore`,
  `.github/pull_request_template.md`, and `src/`, `docs/`, `examples/` folders.
- `Onboarding` (this repository) holds these rules and Git practice.

## 3. Access

- Everyone uses their own GitHub account with two-factor authentication on. Shared team accounts are only for
  ownership continuity, not daily work.
- Give access through **teams** (one per IHC team), not person by person.
- Keep at least two org owners from different cohorts.
- **Offboarding:** when someone leaves a role, remove them from the team (or org) and rotate any secrets they had.

## 4. Day-to-day workflow

1. **Issue:** open an issue for each task.
2. **Branch:** from `main`: `feature/<short-name>`, `fix/<short-name>` or `docs/<short-name>`.
3. **Pull request:** into `main`; fill in the template and link the issue.
4. **Review:** at least one other member approves. Clinical logic (triage rules, lab thresholds, patient-facing
   wording) also needs a clinical lead's sign-off, recorded in `docs/`.
5. **Merge:** squash-merge and delete the branch.
6. **Release:** for deployed tools, tag `vX.Y.Z` and note the change in the README.

Nobody pushes straight to `main`.

## 5. Secrets and incidents

- Keep keys in a git-ignored `.env` or Apps Script properties; commit only `.env.example` with the variable names.
- If a secret is committed, **rotate it at the provider first**, then remove it. Deleting the commit is not enough.
- If real data is committed, tell an org owner at once; do not open a public issue about it. Contact: _fill in_.

## 6. Handoffs and archiving

IHC roles turn over every year. Before you leave a project: update its README and `HANDOFF.md`, move non-code
files to Drive, and make sure someone else has the access they need. A finished project's repository is archived in
its settings, not deleted.

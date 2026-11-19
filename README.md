# Onboarding

> **Fill in:** a one-line purpose for this repository (e.g. onboarding material and starter code for new members).
> This repository is public: everything committed here can be read by anyone.

| | |
|---|---|
| Team leads | _fill in_ |
| Status | Active |
| Non-code files | IHC Google Drive (link: _fill in_) |

## What goes here

Code for Onboarding's projects and the docs needed to run it: scripts (Apps Script, Python, R), add-ons, small web tools,
analysis notebooks. Meeting notes, forms, spreadsheets, reports and anything with real names stay in Google Drive.

## Layout

Each project gets its own top-level folder:

```
Onboarding/
├── README.md             this file: team overview and project index
├── HANDOFF.md            team status and next steps
├── <project-name>/       one folder per project, kebab-case
│   ├── README.md         what it does, owner, how to run and deploy
│   ├── src/              code (Apps Script: clasp layout)
│   ├── docs/             design notes, protocol, sign-off records
│   └── examples/         synthetic sample data only
└── .github/
    └── pull_request_template.md
```

A project that needs its own deploys, CI or outside collaborators can move to its own repository
(`Onboarding-<project-name>`); ask an org owner.

## Projects

| Folder | What it does | Owner | Status |
|---|---|---|---|
| _none yet_ | | | |

## Rules

- **No real patient data or applicant data**, in code, examples, tests, screenshots or logs. Use invented patients.
- **No secrets** (API keys, Supabase keys, passwords, service-account files). Keep them in a git-ignored `.env`
  and share them through the team's password manager or Drive, never in a commit.
- Work on a branch and open a pull request into `main`; another team member reviews before merging.
- Changes to clinical logic (triage rules, lab thresholds, patient-facing wording) need a clinical lead's sign-off,
  recorded in the project's `docs/`.
- Update `HANDOFF.md` when you stop working on something or hand over a role.

Full SOP: [CONTRIBUTING.md](https://github.com/InternationalHealthCollective/.github/blob/main/CONTRIBUTING.md) in the `.github` repository.

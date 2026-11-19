# Onboarding

Where new IHC members learn Git and GitHub, and where the organization's working rules live. This repository is
public: everything committed here can be read by anyone.

## Project repositories

Each project has its own repository:

| Repository | Project |
|---|---|
| [triage-form-upload](https://github.com/InternationalHealthCollective/triage-form-upload) | Triage Form Upload |
| [after-visit-summary](https://github.com/InternationalHealthCollective/after-visit-summary) | After Visit Summary (AVS) |
| [password-generator](https://github.com/InternationalHealthCollective/password-generator) | Password Generator |
| [pqi-dashboard](https://github.com/InternationalHealthCollective/pqi-dashboard) | PQI Dashboard |
| [car-annual-report](https://github.com/InternationalHealthCollective/car-annual-report) | CAR Annual Report |
| [timesheet-analysis](https://github.com/InternationalHealthCollective/timesheet-analysis) | Timesheet Analysis |

A new project gets its own repository (kebab-case name), created by an org owner, with the same starting files:
`README.md`, `HANDOFF.md`, `.gitignore`, `.github/pull_request_template.md`, `src/`, `docs/`, `examples/`.

## Learn Git here

1. Make a GitHub account, turn on two-factor authentication, and ask an org owner to add you.
2. Read [CONTRIBUTING.md](CONTRIBUTING.md): the rules for every IHC repository.
3. Practice the workflow in this repository:
   - create a branch named `practice/<your-github-username>`;
   - add a file `practice/<your-github-username>.md` with one line about which project you will work on;
   - open a pull request into `main` and ask a teammate to review it;
   - after approval, squash-merge and delete the branch.
4. Then do the same in your project's repository for real work.

Only your GitHub username goes in the practice file: no real names, emails or phone numbers.

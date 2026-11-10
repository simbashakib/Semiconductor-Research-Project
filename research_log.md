# Semiconductor Supply-Chain Alpha — Research Log

Maintain dated entries in chronological order. Record decisions and actual work,
including unsuccessful experiments. Preserve earlier entries and explain later
corrections in a new entry. The research roadmap is in `research_protocol.md`.

## 2026-11-10 — Phase 0 initialization

### Objective and agreed approach

Established a fresh project investigating upstream information and future
semiconductor equity returns over 1, 5, 20, and 60 trading days. Simba supplied
the research universe, nine-phase roadmap, integrity rules, and learning-first
workflow. Negative findings are valid outcomes.

Simba will work in VS Code, including the Codex extension and Jupyter notebooks.
GitHub Desktop is installed and available for version control. Research work will
proceed step by step, with explanations before implementation and opportunities
for Simba to write and review code.

### Completed and verified

- Inspected the project directory. It initially contained an initialized Git
  repository on `main`, with no commits or configured remote.
- Simba created `notebooks/`, `src/`, `tests/`, `data/raw/`, `data/processed/`,
  `references/`, and `reports/`. Their presence was verified.
- Created `AGENTS.md` from the initialization brief. Simba read it and approved
  it with “I have read it, looks good”.
- Created `research_protocol.md` to preserve the agreed scope, phases, research
  standards, deliverables, academic starting points, and unresolved decisions.
- Created this research log to support continuity between conversations.

### Environment observations and proposals

Earlier read-only checks found system Python 3.9.6 at `/usr/bin/python3`,
Anaconda Python 3.14.6, Conda 26.7.3, and Jupyter under `/opt/anaconda3/bin/`.
Recheck the environment from VS Code before configuration.

A dedicated Conda environment named `semiconductor-research` with Python 3.12
was proposed. Environment creation and notebook-kernel verification remain
pending. VS Code is the selected notebook interface. Package choices will be
confirmed as setup proceeds.

### Findings and uncertainties

Phase 0 is in progress. Empirical research, data acquisition, formal hypotheses,
and predictive results remain pending. The supplier links and academic references
in the brief await verification during Phase 1.

The protocol carries the requirement to preserve an untouched final test period
into the earlier exploratory phases. Exact split dates and analysis details
remain open and require agreement before the relevant empirical work.

### Files created or modified

- `AGENTS.md` — created and approved by Simba.
- `research_protocol.md` — created from the supplied brief.
- `research_log.md` — created with this initial entry.

### Next steps

1. Review the protocol and this entry for fidelity to the agreed project.
2. Configure the dedicated Python environment and verify notebook execution
   inside VS Code with Simba participating.
3. Add the README, environment specification, and appropriate Git exclusions.
4. Make the initial commit and publish to the intended GitHub repository after
   confirming its name and visibility.
5. Begin Phase 1 with TSMC and its semiconductor-material suppliers after
   completing Phase 0.

## 2026-11-10 — GitHub repository connected and Conda checked

Simba created the GitHub repository at
https://github.com/simbashakib/Semiconductor-Research-Project and authorized
using commits and pushes for version control.

Local inspection confirmed `origin` points to that repository, `main` tracks
`origin/main`, and commit `d230bc2` contains `AGENTS.md`. The protocol and log
were awaiting their first commit at inspection. This entry accompanies the
documentation checkpoint for those files.

Conda is available at `/opt/anaconda3/bin/conda`, version 26.7.3. The environment
list currently contains only `base` at `/opt/anaconda3`. The project environment
and VS Code notebook kernel still need setup and verification.

Next, guide Simba through creating and activating `semiconductor-research`,
then selecting and checking its Python interpreter in VS Code. README,
environment documentation, and Git exclusions remain pending. Phase 0 continues.

## 2026-11-10 — User-led version control and environment creation

Simba clarified that he wants to handle commits and pushes himself to learn
version control. Updated `AGENTS.md` accordingly. This supersedes the earlier
interpretation of permission for the assistant to perform routine Git operations.

The assistant previously created local commit `45bb8d0`, adding the protocol
and research log. Its push was rejected by automatic approval review. The latest
local status shows `main` one commit ahead of `origin/main`. Simba will handle
uploading this commit and committing subsequent changes.

Inspection of the visible VS Code terminal confirmed successful completion of
Simba's `conda create -n semiconductor-research python=3.12 ipykernel` command.
At that inspection the terminal still showed `(base)`. Activation, the installed
Python version, and notebook execution still require verification.

Files modified in this step are `AGENTS.md` and `research_log.md`. The next
environment step is for Simba to activate `semiconductor-research` and check
`python --version` in the VS Code terminal.

## 2026-11-10 — Setup readiness checks

Simba reported completing the commit and push. Local inspection found a clean
working tree and `main` matching the locally recorded `origin/main` at `aa6d5e6`.
This check used the local tracking reference without querying GitHub again.

Direct execution of the project interpreter verified Python 3.12.15 and
ipykernel 7.3.0 at `/opt/anaconda3/envs/semiconductor-research/bin/python`.
VS Code's Microsoft Python and Jupyter extension directories are present.
Notebook execution through the VS Code interface remains to be verified by Simba.

Created `README.md` with the project introduction, current status, setup, layout,
and version-control workflow. Created `environment.yml` using the existing
environment's `defaults` channel and its verified Python and ipykernel versions.
This pins the two direct dependencies but does not lock all transitive packages.
Created `.gitignore` for local datasets, Python environments and caches,
credentials, and macOS metadata.

Files created are `README.md`, `environment.yml`, and `.gitignore`. This log was
updated. Next, Simba should execute a small notebook cell with the project kernel,
then review and commit the setup files. Phase 0 remains in progress until the
notebook execution check is complete.

## 2026-11-10 — Phase 0 environment verification completed

Inspected Simba's executed notebook in VS Code. The selected kernel was
`semiconductor-research (Python 3.12.15)`. The first cell completed successfully
and displayed `/opt/anaconda3/envs/semiconductor-research/bin/python`, Python
3.12.15, and `4` for `2 + 2`.

Phase 0 established the local repository, working instructions, research protocol,
log, directory layout, README, Git exclusions, and Conda environment specification.
The initial documentation commits were published by Simba. The environment works
through VS Code's notebook interface. The scratch notebook is currently unsaved.
This entry records the execution evidence.

Updated `README.md` with the verified status and this log with the phase summary.
Updated the Phase 0 setup paragraph in `research_protocol.md` to replace outdated
pending-configuration wording with instructions to record the verified setup.
The final setup files and these documentation changes await Simba's review,
commit, and push.

Remaining uncertainty concerns the research itself, including supplier links,
source verification, and the open methodological decisions in the protocol.
No empirical findings have been produced. The next research step is Phase 1,
beginning with TSMC's business model, semiconductor-material inputs, and evidence
for its supplier relationships.

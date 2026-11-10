# Semiconductor Supply-Chain Alpha

A learning-led quantitative research project investigating whether upstream
semiconductor material prices and supplier-equity movements help predict future
semiconductor equity returns over **1, 5, 20, and 60 trading days**.

The study will examine information transmission in both directions, common market
movements, plausible economic mechanisms, out-of-sample predictability, and
realistic implementation. Negative findings are valid research outcomes.

## Current status

Phase 0 environment setup is complete. The repository and Python environment are
established, and notebook execution using the project kernel in VS Code was
verified on 10 November 2026. The final setup files await Simba's commit and push.
Phase 1 will begin with TSMC and its semiconductor-material suppliers. Empirical
findings will be recorded as research progresses.

## Research scope

The original equity universe comprises NVIDIA, AMD, Broadcom, TSMC, Micron,
Intel, and ASML, grouped by their supply-chain roles. Initial upstream candidates
include SUMCO, Siltronic, Entegris, Linde, and copper. Commercial relationships,
economic exposures, and data suitability require verification.

See [research_protocol.md](research_protocol.md) for the agreed roadmap and
research standards, [research_log.md](research_log.md) for dated progress, and
[AGENTS.md](AGENTS.md) for the working and teaching approach.

## Python and VS Code setup

Install Conda and the Microsoft Python and Jupyter extensions for VS Code.
From the project root, create the environment using the supplied specification.

```bash
conda env create -f environment.yml
conda activate semiconductor-research
python --version
```

If this environment already exists, activate it directly. The specification
records the verified Python 3.12.15 and ipykernel 7.3.0 versions. Conda resolves
their dependencies during creation, so this file is a minimal environment
specification rather than a complete lock of all transitive dependencies.

Open a Jupyter notebook in VS Code and use **Select Kernel** to select the
`semiconductor-research` Python environment. Check `sys.executable` in a cell
to confirm which interpreter executes the notebook. On the current machine,
the expected interpreter is
`/opt/anaconda3/envs/semiconductor-research/bin/python`.

Research libraries will be added as the corresponding work begins, with changes
recorded in the environment specification and research log.

## Repository layout

| Path | Purpose |
| --- | --- |
| `notebooks/` | Research explanations, code, results, and interpretation |
| `src/` | Reusable Python functions |
| `tests/` | Verification of important calculations |
| `data/raw/` | Original downloaded data |
| `data/processed/` | Reproducible transformations |
| `references/` | Sources and research notes |
| `reports/` | Written findings and final outputs |

Git excludes local datasets, environments, credentials, and generated caches.
Document data acquisition and transformations in tracked research files so the
study can be reproduced. Empty directories are created locally as needed because
Git tracks files. To recreate the layout after cloning, run the following.

```bash
mkdir -p notebooks src tests data/raw data/processed references reports
```

## Version control

Simba reviews changes, commits, and pushes using GitHub Desktop or the terminal
as part of learning the research workflow.

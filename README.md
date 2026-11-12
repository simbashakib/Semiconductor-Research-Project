# Semiconductor Supply-Chain Alpha

A learning-led quantitative research project investigating whether upstream
semiconductor material prices and supplier-equity movements help predict future
semiconductor equity returns over **1, 5, 20, and 60 trading days**.

The study will examine information transmission in both directions, common market
movements, plausible economic mechanisms, out-of-sample predictability, and
realistic implementation. Negative findings are valid research outcomes.

## Current status

As of 12 November 2026, setup and the initial descriptive equity investigation
are complete. The [equity notebook](notebooks/01_semiconductor_equity_analysis.ipynb)
compares daily returns, SPY-adjusted correlations, business subgroups, and two
development subperiods. Positive shared variation remains after SPY adjustment
in both periods and is stronger in 2016–2022. This is descriptive evidence;
causes, statistical significance, and predictive usefulness have not been tested.

The [industry map](references/map%20of%20the%20space.md) provides the supply-chain
overview. Candidate-specific supplier verification and the literature review
remain open. Basket construction and a dedicated covariance analysis are deferred
as recorded in the protocol. The next step is to select and verify one upstream
relationship before acquiring its data.

Exploratory equity data cover 2010–2022. The agreed 2023–2025 final test period
is reserved and excluded from this notebook. The current notebook downloads
fresh Yahoo data on each run; an exact raw snapshot for the saved results is
not established, so revisions may change future reruns.

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
records Python 3.12.15, ipykernel 7.3.0, and the direct research-library versions
verified in the project environment on 12 November 2026. Conda and pip resolve
their dependencies during creation; this is not a complete lock of transitive
dependencies or a guarantee that historical data will remain unchanged.

Open a Jupyter notebook in VS Code and use **Select Kernel** to select the
`semiconductor-research` Python environment. Check `sys.executable` in a cell
to confirm which interpreter executes the notebook. On the current machine,
the expected interpreter is
`/opt/anaconda3/envs/semiconductor-research/bin/python`.

The specification includes NumPy, pandas, Matplotlib, Seaborn, statsmodels, and
yfinance. Add further libraries when the research requires them and record the
change in the environment specification and research log.

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

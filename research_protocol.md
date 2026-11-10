# Semiconductor Supply-Chain Alpha — Research Protocol

Established on 10 November 2026 from Simba's project initialization brief.
This file is the authoritative research roadmap. Record completed work and
current progress in `research_log.md`, and follow `AGENTS.md` for the working
and teaching approach. Explain proposed methodological changes and obtain
Simba's approval before adopting them.

## Research objective

Do upstream semiconductor material prices and supplier-equity movements contain
statistically significant, economically meaningful, and potentially exploitable
information about future semiconductor stock returns?

The agreed prediction horizons are **1, 5, 20, and 60 trading days**. Investigate
information transmission in both directions. Assess contemporaneous correlation,
predictive information, plausible economic mechanisms, and realistic trading
implementation as distinct questions. Negative findings are legitimate outcomes.

The initial motivation was observed co-movement among seven semiconductor-related
stocks. This observation motivates investigation and requires empirical assessment.

## Initial research universe

The groups below preserve the starting classification. Phase 1 will investigate
business activities, exposure, and commercial links in greater detail.

| Group | Initial companies or candidates | Role in the study |
| --- | --- | --- |
| A — Fabless chip designers | NVIDIA (NVDA), AMD (AMD), Broadcom (AVGO) | Original semiconductor equity universe |
| B — Semiconductor manufacturers | TSMC (TSM), Micron (MU), Intel (INTC) | Original semiconductor equity universe |
| C — Manufacturing equipment | ASML (ASML) | Original semiconductor equity universe |
| D — Candidate upstream suppliers | SUMCO, Siltronic, Entegris (ENTG), Linde (LIN) | Potential upstream equity signals |
| E — Raw materials | Copper initially, with investigation of semiconductor-grade silicon wafers, specialty gases, gallium, germanium, and relevant chemicals | Potential material-price signals |
| F — Market benchmarks | Potentially SPY, SOXX, SMH, and relevant market or industry factors | Common-movement controls and benchmarks |

The proposed exposure of SUMCO and Siltronic is semiconductor silicon wafers,
Entegris specialty materials and contamination control, and Linde industrial and
specialty gases. Verify these exposures and actual commercial relationships using
reliable sources. The initial list is a set of candidates for investigation.

Add variables only when economic relevance and data quality justify inclusion.
Confirm exchanges, instruments, currencies, and histories before acquisition.

## Phase 0 — Establish the research environment

Set up the local repository, permanent project documentation, a reproducible
Python environment, and Jupyter notebooks within VS Code. Use GitHub Desktop
for repository operations as appropriate.

Required project documentation comprises `AGENTS.md`, this protocol,
`research_log.md`, and `README.md`. Maintain `notebooks/`, `src/`, `tests/`,
`data/raw/`, `data/processed/`, `references/`, and `reports/` as work develops.
Create useful artifacts as needed and exclude local data and environment files
from Git where appropriate.

Completion requires a verified notebook execution environment, documented setup,
and an initial commit published to the intended GitHub repository. Record verified
Python and package versions in the environment specification and research log.
Simba manages the GitHub repository and its visibility.

## Phase 1 — Industry research and supply-chain mapping

Begin with a detailed investigation of TSMC and its semiconductor-material
suppliers. Expand to the seven original companies and candidate upstream signals.
Read official filings, verify commercial relationships and semiconductor exposure,
review relevant academic literature, and formulate precise economic hypotheses.

Explain mechanisms and possible directions of information transmission. Document
the evidence and uncertainties supporting each proposed link.

**Deliverable:** A sourced supply-chain map, literature review, and formal
research hypotheses.

## Phase 2 — Semiconductor equity analysis

Collect historical equity prices, calculate adjusted returns, construct
semiconductor baskets, and investigate correlations, covariance, volatility,
market exposure, and common movements. Explain adjustment conventions and basket
construction before implementation.

**Deliverable:** A Jupyter notebook establishing the statistical properties of
the original semiconductor universe.

## Phase 3 — Upstream data acquisition

Collect justified supplier-equity and commodity series. Audit sources, missing
observations, adjustments, timestamps, trading calendars, revisions, and
reproducibility. Record source and retrieval details and the meaning of each field.

**Deliverable:** A clean, documented research dataset.

## Phase 4 — Exploratory relationship analysis

Investigate contemporaneous and rolling relationships, lagged correlations,
conditional returns, and differences between economic subgroups. Explore both
directions of information transmission and record the analyses attempted.

**Deliverable:** A descriptive analysis identifying relationships worth formally
testing.

## Phase 5 — Formal predictive modelling

Assess whether upstream information improves forecasts at each of the four agreed
horizons. Begin with simple regression, explicit mathematical hypotheses,
appropriate statistical tests, simple forecasting baselines, and relevant controls.
Define the target, information set, and forecast decision time before estimation.
Justify inference and address the set of hypotheses tested.

**Deliverable:** A formal statistical assessment of predictive relationships.

## Phase 6 — Out-of-sample validation

Evaluate forecasts using chronological training, validation, and untouched final
testing periods. Investigate robustness across regimes, parameter choices, and
alternative explanations. Account for overlapping outcomes and training/test
boundaries. Fit data-dependent transformations using the permitted training data.

Preservation of the final test period applies during earlier phases too. Agree
and record the sample split and permitted exploratory sample before inspecting
data that could compromise the final test. Exact dates and boundary handling
remain design decisions to resolve before the relevant analyses.

**Deliverable:** A robust out-of-sample evaluation.

## Phase 7 — Trading strategy development

Proceed if predictive evidence justifies a trading investigation. Specify
executable entry times, transaction costs, slippage, sizing, risk, turnover, and
benchmarks. Explain how forecast horizons translate into positions and potentially
overlapping holdings. Preserve sufficient records to audit reported performance.

**Deliverable:** An auditable trading backtest if justified. Otherwise document
the evidence and decision against proceeding at this stage.

## Phase 8 — Extensions

Consider cointegration, error-correction models, supply-disruption event studies,
or nonlinear relationships when economic reasoning and earlier evidence support
them. Justify additional complexity and record secondary investigations explicitly.

**Deliverable:** Clearly identified secondary investigations, where warranted.

## Phase 9 — Final research report

Produce a mathematically rigorous report, reproducible notebooks, documented
Python code, and a professional GitHub repository. Present evidence, uncertainty,
limitations, negative findings, and the research decisions needed to reproduce
the conclusions.

**Deliverable:** A complete quantitative research project demonstrating research
competence.

## Standards applying throughout the study

1. Never invent sources, data, relationships, calculations, or findings.
2. Define variables, explain or derive methods, state assumptions, and justify
   statistical conclusions.
3. Use predictive information available before the forecast or trading decision.
   Document international trading hours and release times.
4. Prevent leakage through rolling features, overlapping returns, revisions,
   preprocessing, model selection, and sample boundaries.
5. Pre-specify primary analyses, preserve holdout data, and record alternatives
   and unsuccessful experiments to address data snooping.
6. Account for autocorrelation, heteroskedasticity, nonstationarity, and overlapping
   5-, 20-, and 60-day outcomes where relevant.
7. Distinguish correlation, prediction, causality, and profitable implementation.
8. Document sources, parameters, decisions, mathematical methods, and results.
9. Start with interpretable methods and justify additional complexity.
10. Critically review unsupported claims and methodological weaknesses.
11. Explain techniques before implementation and let Simba attempt research code.
12. Explain proposed changes and obtain approval for changes to hypotheses,
    research designs, datasets, or validation standards.

## Notebook and phase documentation

Each research notebook should contain its research question, mathematical
methodology, sources and assumptions, Python implementation, results and figures,
interpretation, and limitations and conclusions. Important figures and results
must be understandable without inspecting the code.

At the end of every phase, record the investigation, completed work, findings,
uncertainties, files created or modified, and next steps in `research_log.md`.

## Academic starting points awaiting verification

The initialization brief supplied the following references. Verify bibliographic
details and read reliable versions before citing or relying on their findings.

- Cohen & Frazzini (2008), *Economic Links and Predictable Returns*.
- Valcarcel, Vivian & Wohar (2017), *Predictability and Underreaction in
  Industry-Level Returns: Evidence from Commodity Markets*.
- Engle & Granger (1987), *Co-Integration and Error Correction: Representation,
  Estimation, and Testing*.

Also investigate literature on backtest overfitting, multiple hypothesis testing,
robust financial time-series inference, and implementation costs.

## Open decisions

Resolve and record these before the corresponding empirical work. Current entries
are questions to settle, rather than completed design choices.

- Exact supplier relationships, semiconductor exposures, and primary hypotheses.
- Data providers, instrument identifiers, currencies, and sample coverage.
- Return definitions, basket weights, and adjustment conventions.
- Forecast decision times, information alignment, and executable trading times.
- Chronological split dates, permitted exploratory sample, and boundary handling.
- Primary predictors, lag choices, controls, baselines, evaluation metrics,
  inference methods, and treatment of multiple testing.
- The evidence required to justify proceeding to trading-strategy development.

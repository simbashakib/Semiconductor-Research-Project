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

## 2026-11-10 — Phase 1 begins with TSMC

Simba confirmed readiness to begin. Local Git inspection found a clean working
tree and `main` matching the locally recorded `origin/main` following the setup
commits. Phase 0 is complete.

Located and read the business overview, raw-material sourcing, and raw-material
risk discussion in TSMC's official 2025 Form 20-F. Created
`references/tsmc_business_and_inputs.md` with the source URL, access date,
reading locations, brief source observations, and a first exercise for Simba.
Updated `README.md` to reflect Phase 1 and appended this log entry.

The exercise asks Simba to explain the business, identify material dependencies,
and reason through supply-disruption and demand-growth scenarios. The scenarios
are prompts for economic reasoning. Formal hypotheses, named supplier links,
and predictive relationships remain to be established. The 2025 report provides
current background; historical studies will need time-appropriate evidence.

Next, review Simba's answers, clarify the mechanisms and assumptions, then begin
verifying individual supplier relationships against primary sources.

## 2026-11-12 — Descriptive semiconductor equity chapter closed

Completed `notebooks/01_semiconductor_equity_analysis.ipynb` for NVDA, AMD, AVGO,
TSM, MU, INTC, ASML, and the SPY benchmark. Yahoo Finance data were downloaded
through yfinance for 2010–2022, using `Adj Close` and simple daily returns without
filling missing inputs. The saved sample has 3,271 returns per ticker, from
5 January 2010 to 30 December 2022. The agreed 2023–2025 final test period is
reserved and is not downloaded or analysed by this notebook.

The analysis covers return summaries, original correlations, separate OLS
regressions on SPY with intercepts, residual correlations, four business subgroups,
and a comparison of 2010–2015 with 2016–2022. Regressions were refitted separately
in each subperiod. These calendar splits are exploratory, not predictive tests or
verified economic regimes. Subgroup statistics average distinct stock-pair
correlations; within-group estimates are undefined for the single-stock foundry
and equipment groups.

| Period | Mean original stock-pair correlation | Mean SPY-residual correlation |
| --- | ---: | ---: |
| 2010–2015 | 0.447 | 0.162 |
| 2016–2022 | 0.577 | 0.267 |

Positive co-movement remains after SPY adjustment in both periods and is stronger
in the later sample. The TSM–ASML residual correlation rises from 0.195 to 0.419.
Within-group relationships are not uniformly stronger than cross-group ones.
These are descriptive findings for selected companies; no formal uncertainty,
causal attribution, upstream predictability, or trading performance has been
established. Removed the unsupported AI/datacentre explanation from the notebook.

The temporary addition of Samsung and SK hynix was reversed. The earlier
ten-ticker CSV remains in local `data/raw/`; it is not asserted to be the exact
input to the current saved results. The notebook still downloads fresh data on
rerun, and its exact retrieval timestamp/raw snapshot was not recorded. Subsequent
experiments need retained raw inputs and retrieval provenance. Price adjustments
and independent session completeness remain unverified.

The researcher reported a successful top-to-bottom notebook run. Saved code cells
have consecutive execution counts 50–72 and no error outputs. Documentation cleanup
preserved every analysis code cell and its outputs; no new market-data download
was required. The installed project interpreter and direct library versions were
checked: Python 3.12.15, ipykernel 7.3.0, NumPy 2.5.4, pandas 3.1.0,
Matplotlib 3.11.2, Seaborn 0.13.2, statsmodels 0.15.0, and yfinance 1.8.0.
The environment specification now records these direct dependencies; it is not
a complete transitive lock or proof of a fresh environment installation.

Agreed stopping point: close the descriptive H1 chapter, rather than claim the
entire original Phase 2 scope has been delivered. Basket targets/weights are
deferred until the forecasting target is chosen; dedicated covariance analysis
is deferred until required. The market-plus-sector extension was discussed but
not implemented. Candidate-specific supplier verification and literature work
from Phase 1 remain open. Next, select and verify one upstream relationship and
assess data suitability before acquisition.

Files updated: the equity notebook, `research_protocol.md`, `research_log.md`,
`README.md`, and `environment.yml`. No files were added to the repository.
Review, commit, and push remain with Simba.

## 2026-11-18 — Repository review and next research task

Reviewed the project instructions, protocol, complete log, industry map, README,
environment specification, Git exclusions, and all 31 notebook cells with their
saved outputs. The working tree was clean before this entry. Commit `70a25e1`
records the descriptive equity work; `main` matches the locally recorded
`origin/main`. No remote refresh was performed, so this is a local Git check.

| Protocol stage | Evidence and current status |
| --- | --- |
| Phase 0 — Setup | Complete as previously recorded; the environment specification includes the direct research dependencies. |
| Phase 1 — Industry research | The sourced industry map is present. Historical supplier–customer verification, the literature review, and specific predictive hypotheses remain open. |
| Phase 2 — Equity analysis | The descriptive H1 chapter is closed under the 12 November scope decision. Basket construction and dedicated covariance analysis remain deferred, not completed. |
| Phase 3 — Upstream data | A justified, audited upstream dataset has not yet been assembled. The ten-ticker equity CSV is an earlier experiment, not that deliverable. |
| Phases 4–7 — Upstream relationships, prediction, validation, trading | No upstream lead–lag estimates, predictive models, final-test results, or cost-aware trading results are recorded. The equity subgroup and period comparisons are descriptive preparatory work. |

The notebook remains valid nbformat-4, contains 23 code cells with saved execution
counts 50–72, and has no saved error outputs. Code syntax and environment YAML
were checked; no new notebook execution or market-data download was performed.
The saved means remain 0.447/0.162 before/after SPY adjustment in 2010–2015 and
0.577/0.267 in 2016–2022. These findings support further investigation of shared
variation, not causal attribution, formal significance, or predictive performance.

The key reproducibility gap remains the absence of an exact raw snapshot tied to
the saved seven-stock results. Current background filings in the industry map
also do not establish that each supplier relationship existed throughout
2010–2022. Preserve the reserved 2023–2025 final test and resolve historical
evidence and timing before predictive analysis.

Next task: screen one upstream supplier–customer relationship before acquiring
data. Entegris–TSMC is proposed as the first candidate to investigate, not yet an
approved predictive signal or dataset addition. The short screening note should
identify dated primary evidence, the supplied product and economic transmission
mechanism, why information might lead rather than be priced simultaneously, and
the suitability of the intended stock listings and histories. Record a reasoned
proceed/reject decision; expand the candidate set only if the pilot requires it.
Forecast targets, precise information cutoffs, development validation splits,
and inference choices still need definition before a predictive experiment.

Starting sources located for the screening task:
[TSMC's 2018 annual report, section 5.3.4](https://investor.tsmc.com/static/annualReports/2018/english/ebook/files/basic-html/page80.html)
and [Entegris' 19 October 2011 Taiwan facility announcement](https://www.entegris.com/en/home/about-us/news/news101911.html).
These are historical research leads. Distinguish a list of major worldwide
suppliers or regional operations from evidence of an actual bilateral purchasing
relationship; neither implies a predictive return signal or full-period coverage.

Only this log was modified during the repository review. The next supplier
investigation is a research task, not a new empirical finding or phase completion.

## 2026-11-18 — Uploaded report review and focused analysis proposal

Simba delegated large-document reading and synthesis to concentrate his own work
on quantitative analysis. Screened 46 uploaded PDFs: 40 unique documents,
7,976 unique PDF pages. Extracted searchable text where available, examined
relevant business, manufacturing, supply and contract sections, and visually
checked the key evidence pages. This was a targeted review, not a page-by-page
reading of every document. Extraction and rendered-page intermediates remain
outside the repository.

Six TSMC reports are duplicated in the NVIDIA folder. The Micron files are
Schedule 14A proxy statements rather than annual 10-Ks. Intel's 2003 report is
image-only and outside the development window; some later Intel text layers are
garbled, so relevant pages were checked visually. Originals were preserved.

| Link or exposure | Evidence located | Interpretation and limits |
| --- | --- | --- |
| TSMC → NVIDIA wafer manufacture | NVIDIA FY2012, Manufacturing, printed p. 7 / PDF p. 111; FY2022, printed p. 9 / PDF p. 121 | NVIDIA explicitly names TSMC as a wafer manufacturer. This supports a direct foundry–designer link, not a forecast lead. |
| Micron → NVIDIA memory | NVIDIA FY2018, printed p. 9 / PDF p. 116; FY2022, printed p. 9 / PDF p. 121 | NVIDIA explicitly names Micron among memory suppliers. Do not assume identical sourcing throughout 2010–2022. |
| TSMC–ASML collaboration | TSMC 2018, section 5.6, printed p. 87 / PDF p. 45 | Names an R&D funding agreement running 31 October 2012–31 December 2017, with EUR276m funding scheduled for 2013–2017. Expired contract; not a measure of equipment purchases or proof of continuation. |
| Entegris and wafer-materials candidates | TSMC 2015, printed pp. 70–71 / PDF p. 37; 2018, pp. 78–79 / PDF p. 41; 2022, pp. 104–105 / PDF p. 54 | Names Entegris under chemicals and gases, and SUMCO/Siltronic under raw wafers. Category listings do not establish bilateral purchasing volumes or continuous relationships. |
| Intel's mixed activities | Intel 2022, Fundamentals of Our Business, printed p. 8 / PDF p. 12 | Describes internal factories, third-party foundry capacity and foundry services. Existing group labels are coarse exposures, not exclusive business models. |

Source files: NVIDIA's `2012-annual-report-insert-web-ir-update.pdf`,
`2018_annual-report-insert-web-ir-update.pdf` and
`2022-annual-report-insert-web-IR-update.pdf`; TSMC's `e_11.pdf` (2015),
`e_all_5.pdf` (2018) and `2022 Annual Report-E.pdf`; Intel's
`0000050863-23-000039.pdf` (2022), all under the respective `references/` folders.
Filled the existing `references/entegris_tsmc.md` screening note with evidence,
mechanisms and limits. Exact publication dates remain unverified. Later reports
were screened for context, not used as historical predictive inputs.

Proposed next study: compare the economically linked TSM–NVDA, MU–NVDA and
TSM–ASML pairs using the existing panel; consider ENTG–TSM as the first materials
extension, subject to Simba's agreement and data audit. Focus on same-day
stability and one-session lead–lag relationships in both directions, before
formal forecasts at the agreed 1/5/20/60-day horizons. Lagged daily-return
correlations and cumulative-horizon forecasts are different objects. These
analyses have not been implemented or approved as a fixed predictive design.

Same-day SPY adjustment is useful descriptively but leaves semiconductor-wide
influences; it does not isolate causal transmission. A predictive experiment
still needs timestamped information, baselines, chronological validation and
dependence-aware inference. No new price data, correlations, forecasts or trading
results were produced; 2023–2025 remains reserved. The protocol, notebook and
datasets were unchanged. Phase 1 literature and precise predictive design remain
open; a complete supplier census is not a prerequisite for the proposed pilot.

## 2026-11-18 — Keep downloaded reports outside Git

Simba requested that the large downloaded reports remain local rather than be
uploaded to GitHub. The PDFs were untracked, not staged or committed, in the
inspected checkout. Added `/references/**/*.pdf` to `.gitignore`; source reports
remain on disk and research Markdown remains eligible for version control.
Local PDF links require the corresponding downloads on another computer.
No report was deleted and no commit, push or history rewrite was performed.

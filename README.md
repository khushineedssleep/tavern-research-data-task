# Tavern Research – Survey Research Technical Assessment

This repository contains my submission for the Tavern Research Survey Researcher technical assessment. The project includes survey design, polling methodology, exploratory data analysis, toplines, crosstabs, and a proposed Python-based fielding workflow for a statewide public opinion survey.

## Repository Structure

```text
.
├── data/
│   ├── nv_housing_raw.csv
│   └── nv_housing_codebook.csv
│
├── Deliverable 1 - Survey Questionnaire.pdf
├── Deliverable 2 - Polling plan.pdf
├── Deliverable 3 - Best Python practices opinions.pdf
├── Deliverable 3 - Survey Pipeline.pdf
├── Deliverable 4 - Crosstabs.pdf
├── Deliverable 4 - Memo.pdf
├── Deliverable 4 - Toplines.pdf
│
├── surveyor_workflow.png
├── svy_researcher_task.ipynb
└── README.md
```

---

## Deliverables

### Deliverable 1 — Survey Questionnaire
Designed an 8-question public opinion instrument measuring Utah voter attitudes toward AI data center expansion, including:

* Issue salience and awareness
* Favorability and policy tradeoffs
* Water, energy, tax, governance, and environmental concerns
* Programming logic, randomization, and attention checks
* Survey-programmer-ready formatting

### Deliverable 2 — Polling Plan
Prepared a one-page polling methodology memo covering:

1. Universe definition
2. Sample design and strategy
3. Target sample size and MOE estimation
4. Quotas and weighting
5. Crosstab analysis plan
6. Ranked methodological risks
7. Texas expansion strategy


### Deliverable 3 — Fielding Workflow Design
Designed a Python-oriented workflow for operationalizing the survey through Surveyor APIs:

* Survey creation
* YAML conversion and validation
* Deployment and fielding
* Quota monitoring
* Export/report generation

Includes:

* API sequencing
* Pseudocode
* Workflow diagram
* Python engineering practices and design philosophy

### Deliverable 4 — Nevada Housing Survey Analysis
Conducted exploratory data analysis (EDA) and polling analysis using raw Nevada statewide survey data.

#### Analysis included:
* Data structure inspection
* Missingness analysis
* Distribution analysis
* Topline generation
* Crosstab analysis
* Methodological evaluation
* Client-facing memo

#### Key topics analyzed:
* Housing affordability seriousness, support for housing expansion, rent increase limits, corporate buyer restrictions, housing-development tradeoffs

## Exploratory Data Analysis Workflow

The EDA workflow followed standard survey analysis practice:
1. Understand survey structure and target universe
2. Inspect variable types and missingness
3. Examine univariate distributions
4. Generate toplines
5. Produce strategically useful crosstabs
6. Evaluate methodological limitations
7. Summarize findings in memo form

The full notebook is available in:

```text
svy_researcher_task.ipynb
```

## Tools and Technologies

* Python
* pandas
* numpy
* Jupyter Notebook
* Survey methodology theory / polling analysis workflows

## Python Engineering Philosophy

Some engineering principles emphasized in this project:

* Use reproducible project structures (`pyproject.toml`, installable packages, clear environments)
* Prefer readable, testable, Pythonic code
* Use doctests and small reproducible examples where possible
* Treat official documentation and error messages as primary sources
* Design workflows that survive real operational launch conditions

## Notes
All survey findings in Deliverable 4 are based on the provided raw data files. The Nevada dataset did not contain survey weights, so toplines and crosstabs were treated as unweighted directional estimates rather than fully representative population estimates.

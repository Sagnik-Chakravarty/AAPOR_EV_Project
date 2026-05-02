# Repository Structure

This repository preserves the original project layout while adding professional documentation for portfolio and reviewer use.

```text
.
├── README.md
├── Electronic_Vehicle_Sentiment/
│   ├── WebScrapping/
│   │   ├── LLM/
│   │   ├── NYT/
│   │   └── Reddit/
│   ├── Visualizations/
│   ├── Statistical Test/
│   └── WorkableData/
├── docs/
│   ├── project_overview.md
│   ├── methods_summary.md
│   ├── repository_structure.md
│   └── limitations.md
├── analysis/
│   └── README.md
└── outputs/
    └── README.md
```

## Main Directories

### `Electronic_Vehicle_Sentiment/`

Original project directory containing the core data collection, cleaning, visualization, and statistical testing workflows.

### `Electronic_Vehicle_Sentiment/WebScrapping/LLM/`

LLM sentiment workflow, including LLM-generated sentiment outputs and cleaning scripts.

### `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/`

Reddit data collection and sentiment workflow, including subreddit search, comment scraping, and sentiment aggregation.

### `Electronic_Vehicle_Sentiment/WebScrapping/NYT/`

News data workflow for electric vehicle-related media coverage.

### `Electronic_Vehicle_Sentiment/Visualizations/`

R/Quarto visualization workflows for LLM and Reddit sentiment outputs.

### `Electronic_Vehicle_Sentiment/Statistical Test/`

Statistical comparison workflow and summary outputs.

### `Electronic_Vehicle_Sentiment/WorkableData/`

Processed and analysis-ready sentiment datasets.

### `docs/`

Professional documentation for reviewers, including project overview, methods, repository structure, and limitations.

## Suggested Future Cleanup

A future production version could reorganize the repository into:

```text
analysis/
  01_collect_reddit.qmd
  02_clean_llm_outputs.qmd
  03_statistical_comparison.qmd
  04_visualization.qmd
scraping/
  reddit/
  news/
data/
  raw/
  processed/
outputs/
  figures/
  tables/
docs/
```

The current repository keeps the original structure to avoid breaking existing paths and project links.

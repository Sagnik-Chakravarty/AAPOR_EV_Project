# Electric Vehicle Public Sentiment: LLMs vs. Digital Trace Data

This repository contains the code, data-processing workflows, and documentation for a research project comparing large language model-generated sentiment estimates with observed public discourse about electric vehicles across online platforms and news sources.

The project was selected for presentation at the **80th Annual AAPOR Conference**.

## Repository Description

Research project comparing LLM-generated electric vehicle sentiment with observed public discourse from Reddit, news, and other digital trace sources using sentiment analysis, platform comparisons, and reproducible R/Python workflows.

## Project Motivation

Large language models can generate plausible summaries of public opinion, but it is not obvious that those outputs match real-world discourse. This project evaluates whether LLM-generated sentiment estimates can approximate observed public sentiment about electric vehicles and where those estimates diverge from platform-based digital trace data.

The broader methodological question is whether LLMs can be used as substitutes, supplements, or diagnostic tools for public opinion measurement in market, policy, and survey-adjacent research.

## Research Questions

1. How does LLM-generated sentiment about electric vehicles compare with sentiment observed in digital trace data?
2. Do platform-specific sentiment patterns differ across Reddit communities, news coverage, and other online sources?
3. Where do LLM estimates overstate, understate, or smooth public sentiment relative to observed discourse?
4. What are the limitations of using LLMs as proxies for public opinion measurement?

## Data Sources

The project uses a multi-source digital trace approach, including:

- Reddit posts and comments from electric vehicle-related communities,
- New York Times/news data,
- LLM-generated sentiment outputs,
- cleaned sentiment summaries and platform-level aggregation files.

## Methods

The workflow includes:

- web scraping and data collection,
- Reddit subreddit and comment extraction,
- text cleaning and preprocessing,
- sentiment analysis,
- LLM-based sentiment estimation,
- platform-level aggregation,
- statistical comparison of sentiment summaries,
- visualizations using R/Quarto,
- interpretation of validity limits for LLM-based public opinion approximation.

## Repository Structure

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

## Main Files

### LLM Sentiment

- `Electronic_Vehicle_Sentiment/WebScrapping/LLM/LLMSentiment.ipynb`: Notebook for LLM-based sentiment estimation.
- `Electronic_Vehicle_Sentiment/WebScrapping/LLM/LLM_cleaning.qmd`: Cleaning workflow for LLM outputs.
- `Electronic_Vehicle_Sentiment/WebScrapping/LLM/cleaned_llm.csv`: Cleaned LLM sentiment data.

### Reddit Data

- `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/Subreddit_Search/ev_data_scrapping.qmd`: Reddit data collection workflow.
- `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/Subreddit_Search/SubredditURLSentiment.qmd`: Subreddit URL sentiment workflow.
- `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/Subreddit Comments Sentiment/OverallSentimentCalculations.qmd`: Reddit comment sentiment aggregation.

### News Data

- `Electronic_Vehicle_Sentiment/WebScrapping/NYT/NYTFinal.qmd`: News data collection/processing workflow.

### Statistical Testing and Visualizations

- `Electronic_Vehicle_Sentiment/Statistical Test/StatisticalTest.qmd`: Statistical comparison workflow.
- `Electronic_Vehicle_Sentiment/Visualizations/VisualizationLLM.qmd`: LLM sentiment visualization workflow.
- `Electronic_Vehicle_Sentiment/Visualizations/VisualizationReddit.qmd`: Reddit sentiment visualization workflow.

### Processed Outputs

- `Electronic_Vehicle_Sentiment/WorkableData/sentiment_analysis_summary.csv`: Main sentiment summary output.
- `Electronic_Vehicle_Sentiment/Statistical Test/sentiment_analysis_summary.csv`: Statistical-test-ready sentiment summary.

## Key Outputs

- Platform-level sentiment summaries.
- Comparison of LLM-generated sentiment with observed digital trace sentiment.
- Reddit community-specific sentiment outputs.
- Visualizations of sentiment distributions and platform differences.
- Methodological interpretation of when LLMs may fail as substitutes for observed public discourse.

## Skills Demonstrated

- Computational social science
- Survey-adjacent public opinion measurement
- Sentiment analysis
- LLM evaluation
- Reddit data collection
- News data processing
- R/Quarto reporting
- Python notebooks
- Data cleaning and aggregation
- Statistical comparison
- Research presentation for AAPOR

## Limitations

This project should be interpreted as a measurement-validity analysis rather than a definitive estimate of U.S. public opinion about electric vehicles. Digital trace data are not representative samples of the population, and LLM outputs should not be treated as direct substitutes for survey responses. The project focuses on comparing signals across sources and evaluating where LLM-based approximations diverge from observed discourse.

## How to Use

1. Review `docs/project_overview.md` for the research motivation and main design.
2. Review `docs/methods_summary.md` for the data-processing and comparison workflow.
3. Use the notebooks and Quarto files inside `Electronic_Vehicle_Sentiment/` to inspect data collection, cleaning, sentiment scoring, visualization, and statistical testing.
4. Use `Electronic_Vehicle_Sentiment/WorkableData/sentiment_analysis_summary.csv` as the main processed sentiment summary file.

## Authors

- **Sagnik Chakravarty**
- **Namit Shrivastava**

## Conference

Selected for presentation at the **80th Annual AAPOR Conference**.

## Author Contact

**Sagnik Chakravarty**  
M.S. Survey and Data Science, University of Maryland, College Park  
Portfolio: https://sagnik-chakravarty.github.io/  
GitHub: https://github.com/Sagnik-Chakravarty

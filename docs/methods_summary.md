# Methods Summary

## 1. Data Collection

The project combines multiple sources of electric vehicle discourse:

- Reddit posts and comments from EV-related communities,
- news data, including New York Times-related workflows,
- LLM-generated sentiment estimates,
- cleaned platform-level sentiment summaries.

## 2. Reddit Workflow

The Reddit workflow collects and processes discourse from electric vehicle-related communities. Repository files include subreddit search, URL-level sentiment scoring, comment scraping, and overall sentiment calculations.

Relevant files include:

- `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/Subreddit_Search/ev_data_scrapping.qmd`
- `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/Subreddit_Search/SubredditURLSentiment.qmd`
- `Electronic_Vehicle_Sentiment/WebScrapping/Reddit/Subreddit Comments Sentiment/OverallSentimentCalculations.qmd`

## 3. LLM Sentiment Workflow

The LLM workflow produces model-generated sentiment estimates about electric vehicles and cleans these outputs for comparison with observed data.

Relevant files include:

- `Electronic_Vehicle_Sentiment/WebScrapping/LLM/LLMSentiment.ipynb`
- `Electronic_Vehicle_Sentiment/WebScrapping/LLM/LLM_cleaning.qmd`
- `Electronic_Vehicle_Sentiment/WebScrapping/LLM/cleaned_llm.csv`

## 4. News Workflow

The news workflow processes EV-related media coverage and prepares sentiment-related outputs for comparison.

Relevant file:

- `Electronic_Vehicle_Sentiment/WebScrapping/NYT/NYTFinal.qmd`

## 5. Statistical Comparison

The statistical workflow compares sentiment summaries across sources and evaluates whether LLM-generated estimates align with observed digital trace data.

Relevant file:

- `Electronic_Vehicle_Sentiment/Statistical Test/StatisticalTest.qmd`

## 6. Visualization

Visualization workflows produce interpretable summaries of LLM and Reddit sentiment outputs.

Relevant files:

- `Electronic_Vehicle_Sentiment/Visualizations/VisualizationLLM.qmd`
- `Electronic_Vehicle_Sentiment/Visualizations/VisualizationReddit.qmd`

## Methodological Interpretation

The project treats public sentiment as a measurement problem. Reddit, news, and LLM-generated outputs are not equivalent data sources. Each reflects different selection mechanisms, platform incentives, language patterns, and coverage biases. The core contribution is comparing these signals rather than assuming that one source directly represents public opinion.

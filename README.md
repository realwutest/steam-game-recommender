# Steam Game Recommendation System

A group final project for UCSB PSTAT 134. We use Steam playtime data to build two collaborative filtering models with cosine similarity:

- **Item to item:** recommend games similar to a selected game.
- **User to item:** recommend games based on similar players, excluding games the target user already played.

## Files

- `PSTAT Final.qmd`: R code and project write-up.
- `PSTAT Final.html`: the rendered report.
- `PSTAT Final_files/`: styles and scripts used by the HTML report.
- `steam-200k.csv`: the 200,000-row Steam interaction dataset used in the analysis.
- `134 Project Memo.docx`: the project memo.

The data comes from the public Steam Video Games dataset on Kaggle. The analysis keeps play records, filters active users and popular games, explores playtime patterns, and builds item-based and user-based recommendations.

## Read the Report

Clone or download this repository, then open `PSTAT Final.html` in a browser. Keep the `PSTAT Final_files/` folder alongside it so the report's formatting works.

## Run the Analysis

Install R and Quarto, then install the R packages in an R console:

```r
install.packages(c("tidyverse", "Matrix", "knitr", "rmarkdown"))
```

From this repository's root folder, render the report:

```bash
quarto render "PSTAT Final.qmd"
```

You can also open the QMD in RStudio and select **Render**. The included CSV is loaded from the project folder; no API key is required.

This repository preserves the existing final project and its rendered results. The analysis has not been rerun as part of this upload.

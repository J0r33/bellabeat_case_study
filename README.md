# bellabeat_case_study (Google Data Analytics Capstone Project)

Data analysis of Fitbit user activity and sleep patterns for the Bellabeat case study. Includes data cleaning, visualization, and marketing insights built in **R** with tidyverse, and a parallel **SQL**-first version to demonstrate querying, joining, and aggregation skills. Part of the Google Data Analytics Capstone project.

This repository contains my analyses of the Bellabeat fitness tracker dataset:

- `bellabeat_case_study.Rmd`: full, reproducible analysis in R
- `bellabeat_case_study.html`: knitted report (view in browser)
- `bellabeat_case_study.ipynb`: the same analysis logic implemented in SQL (BigQuery-style) to show data preparation, view creation, and business-driven queries

> The notebook version mirrors the Google DA process (Ask → Prepare → Process → Analyze → Share → Act) but executes the *Process* and *Analyze* steps with SQL instead of R. It includes joins across activity, sleep, and hourly tables; date/time parsing; creation of analysis views (e.g. hourly patterns, weekday vs weekend); and queries that lead directly to marketing insights.

## Project Files

All `.csv` files necessary to run the code are available in the **`project_files` branch** of this repository.  
You can clone or download that branch to access the raw Fitbit data used in this analysis.

---

## Presentation

This repository includes a summary presentation of the Bellabeat case study that walks through the full Google DA process (Ask → Prepare → Process → Analyze → Share → Act).

**What it covers:**

- Business task and stakeholders
- Data sources (Fitbit public dataset) and limitations
- Cleaning and transformation steps in R (tidyverse, janitor, lubridate)
- Key analyses (hourly activity, weekday vs weekend, intensity vs calories, daily steps, sedentary vs active time)
- Marketing/engagement recommendations for Bellabeat

**Intended audience:** non-technical stakeholders (Bellabeat marketing leadership) and portfolio reviewers.

You can view the slides here:  
`/bellabeat_case_study_slides.md`

---

## Data Source

**Data Source:** [Fitbit Fitness Tracker Data (Kaggle)](https://www.kaggle.com/datasets/arashnic/fitbit/discussion/614417#3311391) by Mobius — licensed under [CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/).

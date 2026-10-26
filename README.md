# Retail Campaign Effectiveness: Exploratory Data Analysis

## Overview

This project asks whether direct-marketing campaigns, such as coupons sent to chosen households, actually increase what households spend, and whether every type of household responds in the same way. It uses two years of household-level grocery shopping data. At this stage the project is a descriptive analysis: it explains the data, checks its quality and describes how households shop. No campaign effects have been measured yet, and no inferential statistics (e.g. significance testing, regression) have been run.

------------------------------------------------------------------------

## What's in this project currently

-   **`retail-campaign-effectiveness.qmd`** — the report: background and key terms, a variable dictionary, data quality checks (missing values, duplicates, zero and negative values, demographic coverage), and descriptive statistics with charts of line-item sales, household spend, basket value and weekly sales.
-   **`retail-campaign-effectiveness.html`** — the rendered report.

## Data in use

-   **Transactions** — about 2.6 million purchase lines from 2,500 households over two years (102 weeks), recording the product, store, quantity, sales value and any discounts.
-   **Supporting tables** — product details, household demographics (available for 801 households only), the 30 campaigns and their dates, which households each campaign targeted, and coupon redemptions.
-   **Not used yet** — the in-store display and mailer file and the coupon-to-product lookup.
-   **Raw data is not stored in this repository.** The files are too large for GitHub. To reproduce the analysis, download the data and place the files in `data/raw/` (see `data/README.md`).
-   **Focus:** household spend, shopping trips and campaign response at a single retailer.
-   **Source:** dunnhumby, "The Complete Journey" public dataset (<https://www.dunnhumby.com/source-files/>).

------------------------------------------------------------------------

## Tools & Languages

-   **R** — primary analysis language
-   **Quarto** — literate programming and reporting
-   Packages: `tidyverse`, `janitor`, `magrittr`, `ggplot2`, `scales`, `kableExtra`, `pacman`

------------------------------------------------------------------------

## Next steps

-   Measure whether households targeted by each campaign spent more during the campaign than before it, compared with households that were not targeted.
-   Compare the response across household segments and demographic groups.
-   Analyse coupon redemption.

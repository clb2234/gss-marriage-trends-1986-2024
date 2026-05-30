# Changing Patterns of Marriage in the United States: A GSS Analysis of 1986 and 2024

## Project Overview

This project analyzes changes in marital status in the United States using data from the General Social Survey (GSS) for 1986 and 2024. The goal of the project is to compare marital status distributions across time, examine whether these changes appear across different U.S. regions, and create a simple 20-year projection for 2044 based on the observed change between 1986 and 2024.

The analysis focuses on five marital status categories: married, widowed, divorced, separated, and never married. The results show a substantial decline in the proportion of married respondents and a large increase in the proportion of never-married respondents between 1986 and 2024.

## Research Questions

This project asks:

1. How did marital status distributions change between 1986 and 2024?
2. Did the decline in marriage and increase in never-married status appear across different U.S. regions?
3. What might marital status distributions look like in 2044 if the 1986–2024 trend continues linearly?

## Data

The project uses two General Social Survey datasets:

* `GSS1986.dta`
* `GSS2024.dta`

The datasets were imported into R, converted from labelled Stata values into readable factor labels, and combined into one dataset. Each observation was identified by survey year so that marital status distributions could be compared across time.

## Variables Used

The main variables used in the analysis are:

* `year`: Survey year, either 1986 or 2024
* `marital`: Respondent’s marital status
* `region`: Respondent’s U.S. region

The `marital` variable was grouped into five categories:

* Married
* Widowed
* Divorced
* Separated
* Never married

Missing and non-substantive responses, including “no answer” and “skipped on web,” were excluded before calculating counts and proportions.

## Methods

The analysis was conducted in R using the following steps:

1. Imported the 1986 and 2024 GSS Stata files.
2. Combined the two datasets into one file.
3. Cleaned the marital status variable by excluding missing and non-substantive responses.
4. Calculated counts and proportions of marital status categories by year.
5. Calculated marital status proportions by both year and region.
6. Created visualizations comparing 1986 and 2024 marital status distributions.
7. Created a simple 2044 projection by extending the observed 1986–2024 change forward by 20 years.

The 2044 projection is based on a simple linear trend and should be interpreted as an illustrative projection, not a precise forecast.

## Key Findings

The overall analysis shows that marriage became less common among GSS respondents between 1986 and 2024. In 1986, married respondents made up 56.2% of the sample. By 2024, this proportion had declined to 41.8%.

At the same time, the proportion of never-married respondents increased from 18.1% in 1986 to 33.6% in 2024. This was the largest increase among the marital status categories.

The regional analysis shows that this pattern occurred across the Northeast, Midwest, South, and West. In every region, the proportion of married respondents decreased, while the proportion of never-married respondents increased.

The 2044 projection suggests that if the observed trend continues, never-married respondents may become the largest marital status category overall by 2044.

## Tools and Packages

This project was completed in R using Quarto. The main packages include:

* `haven`
* `dplyr`
* `tidyr`
* `ggplot2`
* `scales`
* `gt`

## Notes

The 2044 projection is based only on the difference between 1986 and 2024. Because it uses only two observed time points, it should not be interpreted as a definitive prediction. Instead, it provides a simple visual illustration of what marital status distributions could look like if the same linear trend continues.

## Author

Carey Byron
Columbia University
UN2102: Applied Statistical Computing

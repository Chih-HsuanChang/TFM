# Code Accompanying Master's Thesis — *Social Media Platform Use and Perceived Polarization of Online Discourse in Taiwan*

> By Chih-Hsuan Chang

![R](https://img.shields.io/badge/R_code-%23276DC3?logo=R&labelColor=white&logoColor=%23276DC3)
![Tidyverse](https://img.shields.io/badge/tidyverse-R_package-%23276DC3?logo=Tidyverse&logoColor=black&labelColor=white&color=%23276DC3)
![LaTeX](https://img.shields.io/badge/LaTeX-manuscript-008080?logo=latex&logoColor=white&labelColor=white&color=008080)
![License](https://img.shields.io/badge/license-GPL--3.0-blue)

## Introduction

This repository contains the analysis code and supporting materials for a Master's thesis investigating how patterns of social media platform use relate to citizens' perceived polarization of online political discourse in Taiwan. Using nationally representative survey data, the study estimates a series of binary logistic regression models to test whether the **breadth** of platforms a person uses, and the specific **repertoires** of platforms they combine, predict the likelihood of perceiving online discourse as polarized with control variables, demographics, income, and trust in news media.

## Project Overview

The thesis project consists of the following components:

1. **Data preparation:** import of the 2024 Taiwan Communication Survey (TCS), Phase 3 Year 3, cleaning of raw variables, and recoding of social media platform-use items.

2. **Variable construction:** two complementary measures of platform use are built from the recoded items:
   - **Platform breadth** — a count of the distinct platforms a respondent reports using.
   - **Platform repertoires** — combinations of platforms constructed with a Boczkowski-style *accumulative* method, capturing not just how many platforms are used but which co-occur.
   - **Controls** — demographic variables, income quantile, and trust in news media.

3. **Modeling:** estimation of binary logistic regression models. Models 1–3 use platform breadth as the focal predictor across increasingly saturated specifications; Models 4 substitute platform repertoires. Results are interpreted via odds ratios with 95% confidence intervals.


## Note on data availability

This study uses the **2024 Taiwan Communication Survey (TCS), Phase 3 Year 3**, collected by Academia Sinica and distributed through the **Survey Research Data Archive (SRDA)**. The data are subject to SRDA's access and use conditions and **are not redistributed in this repository**.

Researchers who wish to reproduce the analysis must request the dataset directly from SRDA:
- SRDA: <https://srda.sinica.edu.tw/>

## Disclaimer

This project was developed exclusively for academic purposes as part of a Master's thesis at master program of comupational social science in Universidad Carlos III de Madrid. The code and materials are intended for research and educational use only. The underlying survey data remain the property of Academia Sinica / SRDA and are governed by their terms of use.

## License

Distributed under the GPL-3.0 License. See `LICENSE` for details.

# FDL LIC-DSAs Database: A Guide

# Background 

This document introduces the FDL LIC-DSAs Database, which collects Debt Sustainability Analyses for Low-Income Countries as published by the World Bank and the IMF, between 2013 and 2024.
LIC-DSAs are published by default, unless requested by country authorities. This transparency is an important tool for civil society and other stakeholders more broadly to understand and assess debt risks, and possibly challenge the IMF and World Bank analyses. However, those documents are systematically provided in pdf format, preventing researchers to use them for quantitative analysis. Hurley (2024) provides a comprehensive analysis of transparency gaps regarding LIC-DSAs and its counterpart for emerging markets and advanced economies, the Sovereign Risk and Debt Sustainability Analysis (SRDSA). She notes that while this transparency is useful, it could be enhanced by being searchable. The objective of this database is to enhance transparency by providing a systematic collection of DSAs and their main standardized tables.

# Description

LIC-DSAs are relatively standardized. They follow a framework – the LIC-DSF – published by the IMF and the World Bank . Over the period covered by the database, the IMF and the World Bank reformed their methodologies in 2017, creating slight differences in the variables used as outcomes and published. but the broad principles and variables remained the same. DSAs published between 2013 and early-2018 follow the 2013 template  and the subsequent ones adopt the 2017 reform . 
To construct the database, we scraped a set of standardized tables from the DSAs and collected all variables described there. The tables we use are the standardized tables of macroeconomic assumptions and debt outcomes, as well as standardized tables for the outcome of the DSA, some key assumptions and parameters. The two main tables of a DSAs are those describing debt dynamics and its determinants, whose outcomes are represented in the key charts.


## Table 1: External debt dynamics

This table includes major information on the external framework for the country. It includes projections for key external sector variables and outcomes: growth, exports, imports, as well as debt outcomes both on external and external public (PPG). It also provides assumptions on future aid flows. The projections usually start in the year of publication and cover a 20 year horizon (year-by-year for projections at 5 years, and then for horizon at 10 and 20 years).
It also includes the contributions of various factors to the evolution of overall external debt.

## Table 2: Public debt dynamics

Similar to table 1, this table focuses on fiscal dynamics, with more information on government spending and revenues. It provides information on overall public debt situation (public debt to GDP ratios, etc).

## Tables 3 and 4: Sensitivity Analysis for Key Indicators of Public and Publicly Guaranteed External Debt and Public Debt

The DSA also considers various shocks and their impact with stress test scenarios. Some are standardized and some have tailored assumptions. Tables 3 and 4 contains information on both, respectively for external PPG debt and overall public debt.

We also include tables on the results and parameters of the DSA, as well as some assumptions which are published in a standardized manner.

## Table A: Result of the DSA
This table typically contains the result of the DSA, including the assessment on external and overall debt distress risk, as well as whether judgement was applied.

## Table B: Debt coverage 
This table typically contains the perimeter of debt coverage, which varies by country, as well as some of the key assumptions regarding contingent risks of liability assumptions. 

## Table C: Debt carrying capacity
A key determinant of the risk level is the debt carrying capacity (DCC), which is in turn determined by actual and projected variables. The table provides the average of those projections for each component of the DCC.
 
## Table D: Borrowing assumptions for stress tests
General assumptions on the borrowing rates are not published, but the additional shocks for stress tests are, and we also scrape the corresponding table. 
 
# Using the database

As of December 09, 2024, the database comprises 606 DSAs from 2013 to 2023 for 68 LICs. 303 DSAs are collected under the methodology preceding the 2017 reform and 303 DSAs under the following methodology. 
The database is available on the FDL Website and on the FDL Github account.

## Data Dictionary :
Because of significant differences in variables presented for pre- and post-2017 review, we provide a dictionary of variables which allow to check which variables are present in which version.
The dictionary file has 5 tabs: a readme (“README”), a detailed table (“TRACKER”) with all DSAs in our database, a detailed table of all variables names and their shortened name in our database, both for pre- and post-2017 variables (“VAR_PRE-2017”) and (“VAR_POST-2017”) and a tab comparing available variables in both sets of DSAs (“VAR_COMPARISON”). 
This excel contains information about the variables in the database (Label, units, alternatives, comparison between methods). A 'readme' is present on the first sheet of this workbook for further information. 

## Data
There is a single identifier dsa.id, which is coded as ISO3_YEAR_MONTH

The final database is divided in two parts: 
1)	Part 1: “DSA_id.xlsx” which includes tables A, B, C and D with all non-time-varying variables (as well as dsa_id and the corresponding country, year and month)
2)	Part 2: “DSA.dta.xlsx” which includes Tables 1-4 with projection by year for all time varying variables

The two parts are formatted “wide”.


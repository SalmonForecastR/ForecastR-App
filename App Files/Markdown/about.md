### Citation

**Project Proposal to the Pacific Salmon Commission**

Vélez-Espino, L.A., Parken, C.K., Clemons, E.R., Peterson, R., and Ryding, K. 2018. Automating procedures for forecasting of terminal run and escapement of Chinook, Coho and Chum salmon stocks using open-source statistical software: Chapter 2. Southern Boundary Restoration and Enhancement Fund, Pacific Salmon Commission, Vancouver BC.

**Final Report**

Vélez-Espino, L.A., Parken, C.K., Clemons, E.R., Peterson, R., Ryding, K., Folkes, M., and Pestal, G. (2019). ForecastR: tools to automate procedures for forecasting of salmonid terminal run and escapement. Final Report submitted to the Southern Boundary Restoration and Enhancement Fund, Pacific Salmon Commission, Vancouver BC.
[Available Online](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&ved=2ahUKEwiMi47T1rrvAhVVJjQIHQ-nCNYQFjAGegQIChAD&url=https%3A%2F%2Fwww.psc.org%2Fdownload%2F585%2Fvery-high-priority-chinook%2F11704%2Fs18-vhp15a-forecastr-tools-to-automate-forecasting-procedures-for-salmonid-terminal-run-and-escapement.pdf&usg=AOvVaw2ZHMiJb0dBhjytGgM8lgvZ)

### Project Overview

ForecastR relies on the open-source statistical software R (R Core Team 2018) to generate age-specific (or total abundance) forecasts of salmon escapement or terminal run using a variety of generic models and enabling users to perform interactive tasks with the help of a Graphical User Interface (GUI). These tasks include: 

a) the selection of forecasting approaches from a wide set of statistical and/or mechanistic models for forecasting terminal run and escapement;

b) the selection of several measures of retrospective forecast performance (e.g., MRE, MAE, MAPE, MASE, RMSE); 

c) the comparison of forecasting models and model selection and ranking; and, 

d) the reporting of forecasting results (point forecasts and interval forecasts) and diagnostics by producing either  detailed reports or executive-summary reports. 

The original design of ForecastR involved the generation of age-specific or total-abundance forecasts using several forecasting approaches, including: (i) simple and complex sibling regressions with the ability to include environmental/biological covariates; (ii) time series models such as ARIMA, exponential smoothing, and naïve models (based on any number of preceding years in abundance time series); and (iii) mechanistic models such as average return rate models that depend on auxiliary data such as the number of outmigrant juveniles, the number of hatchery fish released or the number of spawners in previous years. For both age-structured and non-age-structured data, AIC-based model selection takes place within model types (e.g., ARIMA and exponential smoothing) prior to model ranking across model types based on the abovementioned metrics of retrospective evaluation.

After six developmental phases, the latest release has successfully implemented most of the originally envisioned capabilities for this tool. Additional information about the project and older ForecastR Releases can be found in the GitHub site: https://github.com/SalmonForecastR/ForecastR-Releases. Previous releases have focused on improvements and refinements to the GUI and incorporated a Kalman-Filter sibling regressions module to consider the effects on forecasts of potential trends in survival and/or maturity. In addition, two important developments took place during the last two phases of the ForecastR project: (1) the code for forecasting and model ranking approaches was converted into and R-package to facilitate distribution of the program, allow optimal tracking of functions, and provide the ideal environment for future development; and, (2) an html-based Shiny application (that relies on the R-package for forecasting and model ranking operations) has been produced to allow online forecasting exercises. Progress was also made on two other forecasting approaches, namely the complex-sibling-regression module and the return-rate mechanistic module. These two modules were completed and incorporated in the previous release. Detailed information about ForecastR’s current capabilities and description of forecasting models, including the complex-sibling-regression and return-rate, can be found in the Final Report.

Converting ForecastR into an R-package was an important accomplishment because it provided a simple way to distribute the tool and corresponding documentation. From the user’s point of view, the R-package is easy to install and use without risking its integrity. From the developer’s perspective, having an R-package helps to keep track of the miscellaneous R functions, and in the future it would help the process of potential debugging and the development of new capabilities.
Counting with an html-based Shiny application allows online forecasting exercises without users having ForecastR installed in their computers. The App can be accessed through two different servers: (https://psc1.shinyapps.io/ForecastR/ and https://solv-code.shinyapps.io/forecastr/).

ForecastR is considered a ‘working project’ in which additional forecasting modules and program capabilities to assist can be incorporated in the future to support the ForecastR's community."



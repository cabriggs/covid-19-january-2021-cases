## Files included

- covid-19-january-2021-cases.ipynb: a Jupyter notebook containing the analysis and narrative.
- covid-19-january-2021-cases-report.pdf: a report summarizing the findings
- covid-19-january-2021-cases-presentation.mp4: a multimedia presentation of the findings
- data_full.csv: the daily cases data by state scraped from worldometers.info

## Background

Coronavirus disease 2019 (COVID-19) is an ongoing pandemic, affecting nearly every country in the world. COVID-19 is caused by the pathogen SARS-CoV-2. As of June 2021, the first officially recognized case was in Wuhan, China in December 2019, but investigations into the origin are ongoing. COVID-19 began sweeping the globe by at least early 2020.

In this study, the winter wave of 2020-21 coronavirus cases in the USA are modeled, in order to examine the daily case behavior in January 2021.

## Problem statement

During late January 2021, the number of new COVID-19 cases per day dropped precipitously across the United States. Was this drop expected given standard epidemiological modelling approaches, or did the drop in new cases exceed the expectations of such models?

## What data

We have a dataset of 469 records showing the daily new cases of COVID-19 for US states (and DC, Guam, and Puerto Rico) during March 2020 - June 2021.

## What methods

First, Gaussian curves are fit to the winter wave, and found to be a poor fit. A modified Gaussian curve (replacing the square with an absolute value) is then used, with a better fit resulting.

### Technology

The analysis was performed in a Jupyter notebook, leveraging the pandas, numpy, scipy, requests, and BeautifulSoup libraries.

## What conclusions

The cases in late January 2021 experienced a dropoff which was faster than predicted by the models fitted in this study.

## What questions remain

Are the models used here optimized? Can we fit a model to the multiple waves, therefore incorporating information about the varying underlying carrying capacity of the disease?

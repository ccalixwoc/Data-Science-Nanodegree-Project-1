# Data-Science-Nanodegree-Project 1

## Table of Contents
1. [Installation](#Installation)
2. [Motivation](#Motivation)
3. [File Descriptions](#FileDescriptions)
4. [Results](#Results)
5. [Licensing, Authors and Acknowledgment](#Licensing,AuthorsandAcknowledgment)

## Installation
To run this project, I used Python 3 and installed the following libraries: numpy, pandas and plotly.

## Motivation
As part of my Udacity Nanodegree in Data Science, I ran an exploratory analysis on COVID-19 to help myself understand more about the virus in the midst of the global pandemia. The questions that my analysis are aimed at answering are the following:
- How does the number of cases differ between the two viruses?
- What are the countries with the highest number of cases in both outbreaks?
- How do recovery rates and mortality rates compare among both diseases?

### How does the number of cases differ between the two viruses?
This question allos us to understand the spread and severity of both viruses. The variable confirmed cases provides insights into the volume of cases for each disease. The variables date/observation can be used to get the day number in order to create this trend. 

The COVID-19 dataset was grouped at a country level, since it included data at a state/province level. To retrieve the day number, the day number of each country was calculated based on the earliest entry date in each dataset. Both datasets were merged after all columns had the same nomenclature. 

The dataset was subsequently plotted as a line chart showing how each disease evolved across time

### What are the countries with the highest number of cases in both outbreaks?

This question aims to show how each disease has evolved across countries. Similar to the previous analysis, the variable confirmed cases will help us answer this question, except that the data will be grouped by the variable country/region. After grouping the data by country and filtering it by countries with the highest confirmed cases, the data was plotted using bar graphs.

### How do recovery rates and mortality rates compare among both diseases?
This question aims to compare both mortality and recovery rates across countries for the countries with the highest volume of cases. We can use the variables confirmed cases, recovery cases and deaths to answer this question. Recovery and mortality rates can be calculated by dividing the number of recovery and deaths over the number of total confirmed cases after the data has been grouped by country. These rates are then compared using bar graphs. 

## File Descriptions
My analysis can be found in this [file](https://github.com/ccalixwoc/Data-Science-Nanodegree-Project-1/blob/master/dsnd-project-1.ipynb). This Jupyter notebook demonstrates all the related work to answer the questions above. It includes the preprocessing steps required to analyze both datasets on COVID-19 and SARS together. Additionally, it includes all the Plotly visualizations used to answer these questions. 

## Results
You can find my results in this Medium [post](https://medium.com/@ccalix.woc/a-small-comparative-analysis-between-covid-19-and-sars-de23a3574216).


## Licensing, Authors and Acknowledgment
All data was retrieved from Kaggle. You can find the datasets for [COVID-19](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset) and [SARS](https://www.kaggle.com/imdevskp/sars-outbreak-2003-complete-dataset/kernels) here.

# Skin Cancer Analysis 
### Project description:
You've just joined Pymaceuticals, Inc., a new pharmaceutical company specialising in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a common form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice identified with SCC tumours received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. This study aimed to compare the performance of Pymaceuticals' drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

### Project outline
- Data prep and cleansing
- Creating summary statistics for the study
- Analysis
    - Implementation of linear regression (scipy library)

#### TLDR - Conclusions
- The following drug regimens had the most positive effect on mice over the time points of the study (a key indicator for the effectiveness of a given medicine can be the tumour size in cubic millimetres over the whole period, in particular the mean, median and variance results, **the lower the results are over the timepoints of the study, the better the effect of the medicine on mice**):
    - Capomiulin
    - Caftamin
    - Infubinol
    - Ramicane
- Ceftamin and Infubiol were in the top four amounts; however, relative to the dataset, we didn't have enough observations as opposed to other medicines.**In contrast**, Capomulin and Ramicane were in top four the amount and had the highest amount of observations over the time points of our study. In general, the amount of observations over the time points directly affects the quality of our results and the level of confidence we have in our results.
- Even though we had more female mice in our study, the difference between males and females in percentage spread is insignificant. 
- There is a positive correlation between the weight(g) and cubic millimetre size of the tumour. One conclusion can be that the heavier the mice are, the greater the size of the tumour. However, given that we haven't observed the age of the mice we can't conclude that the weight is a factor for an increase in tumour size (i.e. the age of the mice could change and is not necessarily directly related to the weight of the mice). 


#### Folder structure
``` yml
.
├── Starter_Code
│   ├── Pymaceuticals                      # This folder contains the analysis & dataset's folder. 
│   │   ├── data                           # This folder contains the datasets
│   │   |   ├── Mouse_metadata.csv
│   │   |   ├── Study_results.csv  
│   |   ├── pymaceuticals_starter.ipynb    # Analysis notebook                        
|___README.md
``` 
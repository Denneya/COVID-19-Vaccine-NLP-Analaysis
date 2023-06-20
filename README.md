# COVID-19-Vaccine-NLP-Analaysis 💉
Text analysis of VIRA datasets regarding the COVID-19 vaccination in the UK.

<i>As this analysis was created using Google CoLab, allowing all code chunks to be viewed and executed, I have provided the overview below, as well as a link to view the analysis as a html file.</i>

## Natural Language Processing Application
### Overview

This markdown uses data collected from the Vaccine Information Resource Assistance (VIRA), release by IBM research. There are two datasets which differ slightly in terms of their use. Both datasets will be used in order to identify any insights or important attributes from the chat bot (VIRA) regarding COVID-19 vaccine hesitancy and people's overall trust of the vaccine.

Before exploring and analysing the datasets, it's important to establish questions based on potential discoveries, which can assist in understanding the general climate towards the COVID-19 vaccination. The questions below have been developed based on the current understanding of the datasets and will hopefully be answered at the end of this analysis.

1. Is there an overall positive reaction to the COVID-19 vaccine?
2. Are people mostly hesitant to get the vaccine because of the side effects?
3. Are there many people who believe COVID-19 isn't real, and is this fuelling their distrust in the vaccine?
4. Are people concerned if they have pre-existing conditions?

As these datasets were released for potential modelling purposes, the decision to merge the training, validation and test datasets was made due to the imbalance in distribution of features, as well as more data used in this analysis, the better results. A short summary of each dataset is provided below.


**Covid-19 Vaccine Intent Expressions Dataset**

This dataset contains varying expressions for common questions about the Covid-19 Vaccine. Each expression has been matched to a common question, resulting in 181 common questions. The data dictionary below shows the name and a description of each column in the dataset.



*Data Dictionary- Intent Expressions Dataset*

| Column | Description|
| :- | :- |
| sentence | the expression written by an annotatior, or taken from VIRADialogs (chat bot)|
| label | the common question for which the expression was written |
| label_idx | the running class index associated with this label, between 0 and 181 |


**Covid-19 Vaccine Trust Annotations Dataset**

This dataset contains the VIRADialogs, as used in the Intent Expressions Dataset, however this time they have been annotated and matched with a trust level. The data dictionary below displays the columns and a description of the contents of the Trust Annotations dataset. 


*Data Dictionary- Trust Annotations Dataset*

| Column | Description|
| :- | :- |
| text| the user input VIRADialogs (chat bot)|
| label | the trust label:0 - low institutional trust, 1 - low agent trust, 2 - neutral, 3 - high trust  |


Lastly, citations for these datasets are included here:
1. VIRATrustData: A Trust-Annotated Corpus of Human-Chatbot Conversations About COVID-19 Vaccines
Roni Friedman, João Sedoc, Shai Gretz, Assaf Toledo, Rose Weeks, Naor Bar-Zeev, Yoav Katz, Noam Slonim
arXiv, 2022
2. Benchmark Data and Evaluation Framework for Intent Discovery Around COVID-19 Vaccine Hesitancy
Shai Gretz, Assaf Toledo, Roni Friedman, Dan Lahav, Rose Weeks, Naor Bar-Zeev, João Sedoc, Pooja Sangha, Yoav Katz, Noam Slonim
arXiv, 2022

Read the full analysis here!

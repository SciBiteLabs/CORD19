# CORD19
### Sentence level annotations for the COVID-19 Open Research Dataset Challenge using biomedical ontologies from SciBite ###



## Overview ##
In March 2020 in response to the COVID-19 pandemic, The White House, AI2, CZI, MSR, Georgetown and NIH released an open research dataset along with a call for action (https://www.whitehouse.gov/briefings-statements/call-action-tech-community-new-machine-readable-covid-19-dataset/) from the science and technology community. The call asks that artificial intelligence experts to develop new text and data mining techniques that can help the science community answer high-priority scientific questions related to COVID-19. The original datasets can be accessed at Kaggle: https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge

## What is in this SciBite annotated dataset? ##

Our ontology and SciBiteAI teams have used our software to produce sentence level annotations on this dataset to help those trying to identify biomedical entities within the text. The following have been identified


Ontology Type | Total Hits | Unique Hits
------------ | ------------- | -------------
SPECIES | 2918832 | 3234
GOONTOL - gene ontology terms | 1792505 | 7980
INDICATION | 2796144 | 5222
SARSCOV - coronavirus strains and viral processes | 269567 | 247
COUNTRY | 383215 | 227
HPO - human phenotypes | 779931 | 4256
GENE | 930098 | 11491
CVPROT - proteins of COVID-19 | 200180 | 14
DRUG | 449977 | 9636

## Possible use examples of this annotated dataset ##

Identfying biomedical entities within sentences can be incredibly useful in narrowing down the space of 26,000 documents that researchers or algorithms are required to look at. For instance, if a specific gene or phenotype is of interest, then this data can be easily used to find those documents which contain them. Building knowledge graphs 


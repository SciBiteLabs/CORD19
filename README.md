# CORD19
### Sentence level annotations for the COVID-19 Open Research Dataset Challenge using biomedical ontologies from SciBite ###



## Overview ##
In March 2020 in response to the COVID-19 pandemic, The White House, AI2, CZI, MSR, Georgetown and NIH released an open research dataset along with a call for action (https://www.whitehouse.gov/briefings-statements/call-action-tech-community-new-machine-readable-covid-19-dataset/) from the science and technology community. The call asks that artificial intelligence experts to develop new text and data mining techniques that can help the science community answer high-priority scientific questions related to COVID-19. The origina datasets can be accessed at Kaggle: https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge

## What is in this SciBite annotated dataset? ##

Our ontology and SciBiteAI teams have used our software to produce sentence level annotations on this dataset to help those trying to identify biomedical entities within the text. The following have been identified

'''
SPECIES
Total hits: 2918832
Unique hits: 3234
'''

GOONTOL - gene ontology terms
Total hits: 1792505
Unique hits: 7980

INDICATION
Total hits: 2796144
Unique hits: 5222

SARSCOV - coronavirus strains and viral processes
Total hits: 269567
Unique hits: 247

COUNTRY
Total hits: 383215
Unique hits: 227

HPO - human phenotypes
Total hits: 779931
Unique hits: 4256

GENE
Total hits: 930098
Unique hits: 11491

CVPROT - proteins of covid-19
Total hits: 200180
Unique hits: 14

DRUG
Total hits: 449977
Unique hits: 9636



## Possible use examples of this annotated dataset ##

Identfying biomedical entities within sentences can be incredibly useful in narrowing down the space of 26,000 documents that researchers or algorithms are required to look at. For instance, if a specific gene or phenotype is of interest, then this data can be easily used to find those documents which contain them. Building knowledge graphs 


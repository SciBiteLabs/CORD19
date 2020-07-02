# COVID-19 Annotated Data v1.5

As part of our efforts to help the community with the CORD-19 challenge, we have released several resources to help.

1. [Sentence level annotations for the COVID-19 Data version 6 (3rd April release)](https://github.com/SciBiteLabs/CORD19/blob/master/README.md#sentence-level-annotations-for-the-covid-19-open-research-dataset-challenge-using-biomedical-ontologies-from-scibite)
1. [Entity co-occurrence data within sentences](https://github.com/SciBiteLabs/CORD19/blob/master/README.md#entity-co-occurrence-data-within-sentences)
1. [Vocabularies used in this work describing coronavirus family and (specifically) COVID-19](https://github.com/SciBiteLabs/CORD19/blob/master/README.md#vocabularies-used-in-this-work-describing-coronavirus-family-and-specifically-covid-19)

## Accessing the data in this GitHub Repository ##

The large files in this repo are uploaded using [GitHub Large File Sotre (LSF)](https://git-lfs.github.com/). To pull this content you can use the command:

`git lfs clone https://github.com/SciBiteLabs/CORD19.git`

## Sentence level annotations for the COVID-19 Open Research Dataset Challenge (version 6) using biomedical ontologies from SciBite ##

https://github.com/SciBiteLabs/CORD19/tree/master/annotated-CORD-19

### Overview ###
In March 2020 in response to the COVID-19 pandemic, The White House, AI2, CZI, MSR, Georgetown and NIH released an open research dataset along with a call for action (https://www.whitehouse.gov/briefings-statements/call-action-tech-community-new-machine-readable-covid-19-dataset/) from the science and technology community. The call asks that artificial intelligence experts to develop new text and data mining techniques that can help the science community answer high-priority scientific questions related to COVID-19. The original datasets can be accessed at Kaggle: https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge The annotations are made against version 6 of this data released 3rd April.

### What is in this SciBite annotated dataset? ###

Our ontology and SciBiteAI teams have used our software to produce sentence level annotations on this dataset to help those trying to identify biomedical entities within the text. The following have been identified

Ontology Type | Total Hits | Unique Hits
------------ | ------------- | -------------
SPECIES - NCBI Taxon | 2918832 | 3234
GOONTOL - Gene Ontology terms | 1792505 | 7980
INDICATION - MeSH | 2796144 | 5222
SARSCOV - coronavirus strains and viral processes | 269567 | 247
COUNTRY - Standard country codes | 383215 | 227
HPO - human phenotypes | 779931 | 4256
GENE - HGNC | 930098 | 11491
CVPROT - proteins of COVID-19 | 200180 | 14
DRUG - ChEMBL | 449977 | 9636

### Example of use ###

Identfying biomedical entities within sentences can be incredibly useful in narrowing down the space of 29,000 documents that researchers or algorithms are required to look at. For instance, if a specific gene or phenotype is of interest, then this data can be easily used to find those documents which contain them. Building knowledge graphs can be enhanced by being able to perform sentence cooccurence across large documents and forming edges depending upon the types contained. Sentence level sentiment/topic analysis using machine learning methods might also be peformed using the entity types. A full list of tasks are available on Kaggle: https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge/tasks


## Entity co-occurrence data within sentencesversion 1.2 ##

https://github.com/SciBiteLabs/CORD19/tree/master/sentence-co-occurrence-CORD-19/

### Overview ###
This data set represents a way to quickly look for connections between entities in the literature. It has the following columns:

`document_id, sentence_id, entity_uris, entity_types_plus_ids`

In most cases the URIs will link to external resources (such as ontologies) which may be amenable to scraping and often have their own APIs so you can navigate out into the broader life science datascape should you wish to do so.

### Example of use ###

As an example of how you can use this to rapidly hone in on points of interest, we filtered out some sentences which have: a GENE or DRUG hit, and a CVPROT hit, and a hit for coronaviruses (an entity of type INDICATION):

`MERS-CoV first binds, via its S protein, to the receptor DPP4 on the target cell [16] , and then releases its RNA genome, through plasma or endosomal membrane fusion, into the target cell.
To demonstrate that the colocalization of hel/N complexes with M at late times postinfection was due to translocation of existing hel/N complexes to sites of M accumulation rather than to de novo synthesis of hel or N at a new location, we analyzed the effect of the translation inhibitor cycloheximide on hel/N relocalization (Fig. 4) . A 100 g/ml concentration of cycloheximide has been previously determined to be sufficient for inhibition of gene 1 translation in coronavirus-infected cells (Kim et al., 1995; Perlman et al., 1987; Sawicki and Sawicki, 1986) . When infected cells were incubated with cycloheximide beginning at 5.5 h p.i. and continuing throughout the remainder of infection, extensive colocalization of hel or N with M was still observed at 12 h p.i. (Figs. 4A and 4B ).
However, on the basis of only these results, we could not determine whether these amino acid substitutions affected receptorbinding affinity between human DPP4 receptor and MERS-CoV S protein.`


## Vocabularies used in this work describing coronavirus family and (specifically) COVID-19 ##

https://github.com/SciBiteLabs/CORD19/tree/master/vocabularies-CORD-19

### Overview ###
Two vocabularies have been released, both of which were used for this work; a vocab specific to COVID-19 and one more generally around coronavirus family. This includes common names and synonyms for the viruses, common genes and proteins investigated in these strains along with relevant gene ontology terms.


## Contact Us ##

If you have any questions or feedback or are interested in additional data annotations you can get in touch with us by emailing: cvdata@scibite.com or by raising a ticket in this GitHub repo. 

## License ##

The SciBite data annotations and vocabs are released under GPL https://github.com/SciBiteLabs/CORD19/blob/master/LICENSE

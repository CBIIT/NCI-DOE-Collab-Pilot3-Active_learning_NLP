# Active Learning framework for Natural Language Processing of pathology reports.

## Description

This repository implements an active learning loop for natural language processing (ALNLP) of pathology reports related to NCI Pilot 3 project. It implements two methods for embedding extraction of the unstructured text: 1) bag-of-words with dimensional reduction methods, and 2) pre-trained BERT model. Deterministic and Bayesian classifiers are available to predict attributes contained in the pathology reports.

ALNP is an algorithm developed as a part of the Joint Design of Advanced Computing Solutions for Cancer ([JDACS4C] (https://datascience.cancer.gov/collaborations/joint-design-advanced-computing)) pilot projects, to improve the assessment of the pathology report. Researchers can use ANLP to perform prediction of attributes on pathology reports.

## User Community

Researchers who want to compute and analyze membrane surfaces or study their properties for large computational jobs such as those carried out by the [JDACS4C Pilot 3 program] (https://datascience.cancer.gov/collaborations/joint-design-advanced-computing/population-pilot).

## Usability
Requires many software dependencies, even on well-supported high-performance computing systems such as NIH's Biowulf.


## Technical Details
  
Data scientists can train the provided untrained model on their own data, or use the trained model to test the data from [20 newsgroups dataset] (http://qwone.com/~jason/20Newsgroups/). The dataset contains 18000 newsgroups posts on 20 tppics that is available via sklearn package to download and used to test this capability.

Refer to this [README](./README-installation.md).


#License
LLNL released ALNLP under GNU GPL-3.0 license.

For details, refer to LICENSE and NOTICE.

LLNL-CODE-797271
  
# Authors

- André R. Gonçalves (goncalves1@llnl.gov)
- Hiranmayi Ranganathan (ranganathan2@llnl.gov)
- Braden C. Soper (soper3@llnl.gov)
- Pryiadip Ray (ray34@llnl.gov)
- Ana Paula Sales (deoliveirasa1@llnl.gov)

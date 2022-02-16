# Active Learning Framework for Natural Language Processing of Pathology Reports

## Description

This repository implements an active learning loop for natural language processing (ALNLP) of pathology reports related to the NCI Pilot 3 project. This framework implements the following methods for embedding extraction of the unstructured text: 
 * Bag-of-words with dimensional reduction methods, and 
 * Pre-trained BERT (Bidirectional Encoder Representations from Transformers) model. 

Deterministic and Bayesian classifiers are available (in our code repository) to predict attributes in the pathology reports.

ALNP is an algorithm developed as a part of the Joint Design of Advanced Computing Solutions for Cancer ([JDACS4C](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing)) pilot projects, to improve the assessment of pathology reports. Researchers can use ANLP to perform prediction of attributes on pathology reports.

## User Community

Researchers who want to compute and analyze membrane surfaces or study their properties for large computational jobs such as those carried out by the [JDACS4C Pilot 3 program](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing/population-pilot).

## Usability
Requires many software dependencies, even on well-supported high-performance computing systems such as NIH's Biowulf.


## Technical Details
  
Data scientists can train the provided untrained model on their own data, or use the trained model to test the data from the [20 Newsgroups](http://qwone.com/~jason/20Newsgroups/) dataset. The dataset contains 18,000 newsgroup posts on 20 topics that are available via sklearn package to download and test this capability.

Refer to the [installation README](./README-installation.md).


## License
Lawrence Livermore National Laboratory (LLNL) released ALNLP under GNU GPL-3.0 license.

For details, refer to LICENSE and NOTICE.

LLNL-CODE-797271
  
## Authors

- André R. Gonçalves (goncalves1@llnl.gov)
- Hiranmayi Ranganathan (ranganathan2@llnl.gov)
- Braden C. Soper (soper3@llnl.gov)
- Pryiadip Ray (ray34@llnl.gov)
- Ana Paula Sales (deoliveirasa1@llnl.gov)

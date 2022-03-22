# Active Learning Framework for Natural Language Processing of Pathology Reports

## Description

This repository implements an active learning loop for natural language processing (ALNLP) of pathology reports related to the NCI Pilot 3 project. This framework implements the following methods for embedding extraction of the unstructured text: 
 * Bag-of-words with dimensional reduction methods, and 
 * Pre-trained BERT (Bidirectional Encoder Representations from Transformers) model. 

Deterministic and Bayesian classifiers are available (in [classifiers](classifiers)) to predict attributes in the pathology reports.

ALNP is an algorithm developed as a part of the Joint Design of Advanced Computing Solutions for Cancer ([JDACS4C](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing)) pilot projects, to improve the assessment of pathology reports. Researchers can also use ANLP to perform prediction of attributes on pathology reports.

## User Community

 * Data scientists interested in guiding the ground truth augmentation process to enhance a performance of a classifier of free form texts (such as pathology reports, clinical trials, abstracts, and so on). 
 * Researchers who want to perform improved assesssment and prediction on pathology reports are carried out by the [JDACS4C Pilot 3 program](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing/population-pilot).

## Usability
Requires many dependencies (available in the environment.yml file), even on well-supported high-performance computing systems such as NIH's Biowulf.

## Uniqueness
The community can use a neural network and multiple machine learning techniques to perform multi-tasks such as predicting drug response cell line classification. The general rule is that classical methods like random forests would perform better for small datasets, while neural network approaches like UnoMT would perform better for relatively larger datasets.

Active learning is an existing technique in machine learning. This example shows how active learning can be used during the generation of the ground truth of free text documents. 

This is not the first example to perform active learning for NLP. However, the ALNLP algorithm in this repository compares multiple acquisition functions to select the next batch of samples to be labeled (such as random, entropy, marginal sampling, abstention, and so on). 

## Technical Details
  
Data scientists can use the trained model to test the data from the [20 Newsgroups](http://qwone.com/~jason/20Newsgroups/) dataset. The dataset contains 18,000 newsgroup posts on 20 topics that are available via sklearn package to download and test this capability.

Refer to the [installation README](./README-installation.md).


## Release Number

LLNL-CODE-797271
  
## Authors

- André R. Gonçalves (goncalves1@llnl.gov)
- Hiranmayi Ranganathan (ranganathan2@llnl.gov)
- Braden C. Soper (soper3@llnl.gov)
- Pryiadip Ray (ray34@llnl.gov)
- Ana Paula Sales (deoliveirasa1@llnl.gov)

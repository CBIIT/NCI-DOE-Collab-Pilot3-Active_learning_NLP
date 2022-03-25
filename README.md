# Active Learning Framework for Natural Language Processing of Pathology Reports

## Description

This repository implements an active learning loop for natural language processing (ALNLP) of pathology reports related to the NCI Pilot 3 project. This framework implements the following methods for embedding extraction of the unstructured text: 
 * Bag-of-words with dimensional reduction methods, and 
 * Pre-trained BERT (Bidirectional Encoder Representations from Transformers) model. 

Deterministic and Bayesian classifiers are available (in [classifiers](classifiers)) to predict attributes in the pathology reports.

ALNP is an algorithm developed as a part of the Joint Design of Advanced Computing Solutions for Cancer ([JDACS4C](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing)) pilot projects, to improve the assessment and prediction of attributes in the pathology reports.

## User Community

 * Data scientists interested in guiding the ground truth augmentation process to enhance a performance of a classifier of free form texts (such as pathology reports, clinical trials, abstracts, and so on). 
 * Researchers who want to perform improved assesssment and prediction on pathology reports are carried out by the [JDACS4C Pilot 3 program](https://datascience.cancer.gov/collaborations/joint-design-advanced-computing/population-pilot).

## Usability
To use the software package in this repository, users must meet the following criteria:
* Possess the basic skills to program and run Python scripts.
* Understand the input parameters of the ALNLP algorithm, so that they can set the parameters appropriately to execute the algorithm.

To use the optimization loop (simulation), users have to be familiar with natural language processing techniques, training of classifiers, and active learning methods.In the ActiveLearningLoop's execute method, the user can inform the percentages of data initially used for training, the size of test set, and the how many new samples will be selected to be labeled at every iteration of the active learning loop.

## Uniqueness
Active learning is an existing technique in machine learning. This example shows how active learning can be used during the generation of the ground truth of free text documents.There are other examples to perform active learning for NLP. However, the ALNLP algorithm presented in this repository compares multiple acquisition functions to select the next batch of samples to be labeled (such as random, entropy, marginal sampling, abstention, and so on). 

## Technical Details

Refer to the [installation README](./README-installation.md).


## Release Number

LLNL-CODE-797271
  
## Authors

- André R. Gonçalves (goncalves1@llnl.gov)
- Hiranmayi Ranganathan (ranganathan2@llnl.gov)
- Braden C. Soper (soper3@llnl.gov)
- Pryiadip Ray (ray34@llnl.gov)
- Ana Paula Sales (deoliveirasa1@llnl.gov)

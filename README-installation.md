## Installation and Testing on Biowulf


To install the active learning framework for natural language processing (ALNLP) of pathology reports:

1. Log in to [Biowulf](https://hpc.nih.gov/docs/connect.html). 

2. Go to the `/data` partition of Biowulf. For example: 

   1. Run the following command:
   
      ```cd /data/$USER/export```
   
   2. Export the current working directory to the `$alnlp_INSTALL` variable. For example: 
   
      ```export alnlp_INSTALL=$(pwd)```

   Do this on Biowulf. (That is, not from a Biowulf compute node, where GitHub access is limited.)
 
3. Clone this repository: 

   ```bash
   cd $alnlp_INSTALL
   git clone https://github.com/CBIIT/NCI-DOE-Collab-Pilot3-Active_learning_NLP.git
   ```
4. Allocate a compute node for the installation process:

   ```bash
   sinteractive --mem=2g
   ```
5. Install the [Miniconda package manager](https://docs.conda.io/en/latest/miniconda.html). Create and activate an `alnlp` environment:

    ```bash
   conda env create -f environment.yml -n alnlp
   conda activate alnlp
    ```

6. In your conda environment, load python dependencies:

   ```
   python
   >>> import nltk
   >>> nltk.download('stopwords')
   >>> nltk.download('punkt')
   ```

## Testing the Installation

You can test the installation via:

```
cd $alnlp_INSTALL/NCI-DOE-Collab-Pilot3-Active_learning_NLP/experiments
python experiment_001.py
```
The above example script runs the active learning loop for four logistic regression models, each one using a different acquisition function. This example uses the [20 Newsgroups](http://qwone.com/~jason/20Newsgroups/) dataset. In the loop's execute method, you can specify what percentages of data you want to initially use for training, the size of test set, and how many new samples you want each iteration of the loop to select for labeling. After the execution, the example script creates a report with all the results and plots in the given output folder. The Python script also creates a sub-folder with the same name as the script (experiment_001 in this case) to store the plots in PDF format.

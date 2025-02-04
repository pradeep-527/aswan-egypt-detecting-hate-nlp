# Clean Datasets

This folder will contain all clean datasets for Arabic. 

Please create a folder for each clean dataset and name it following the repository's naming conventions. Name the dataset file with their name as indicated in the raw datasets' table. Feel free to add a README.md with details on the dataset and yourself. 

> In case of doubt, please do not hesitate to be in contact with the task leaders. Those unsure about how to use GitHub and/or unwilling to modify the repository structure can simply share their clean datasets with the task leaders on Slack.

## Clean Datasets

| Dataset Name | Link | Engineer |
|-|-|-|

________________________________________________________________

## Pre-processing guidelines

### File structure

The output of the pre-processing has to be a .cvs file. Please create one file for each dataset.

The file will be organised in 5 columns as follows:

 | corpus_name | raw_sentence | label | clean_sentence_training | clean_sentence_EDA |
  |-|-|-|-|-|
 | | | | | |
 | | | | | |
  
 Please respect the column order and naming. For the corpus name, please use the same label you use as a name for your directory (e.g., HateXplain).
 
 ### Labels
 
 > Please note that the labels have changed!
 
 The labels will be:
 - '2' for RISKY sentences (eg., 'hateful' or 'abusive');
 - '1' for POTENTIALLY RISKY sentences (e.g., 'offensive)';
 - '0' for NON RISKY sentences.

We leave to the collaborators the task to determine how to fit the original labels in the three classes above. Please contact the task leaders if unsure about the classification. We'll be most happy to help you decide how to re-label your dataset.

### Preprocessing

The pre-processing for the 'clean_sentence_training' column will involve the following steps:

1- delete all rows containing null values;

2- stopwords removal;

3- removal of digits and words containing digits, punctuation and special characters, extra spaces, links;

4- lemmatization (no NOT perform stemming at it can yield undesirable results).

Please do NOT change the case of your sentences as the distinction between lowercase and uppercase can be meaningful in this context.

The pre-processing for the 'clean_sentence_EDA' will involve all the steps above, *plus the deletion of all emojis* (if present).

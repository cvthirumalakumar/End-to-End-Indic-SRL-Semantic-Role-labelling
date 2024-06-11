# NLP Project - Semantic Role Labelling
Full details about the project are mentioned in `report.pdf`


## Implementation
1. `code` folder contains scripts for training SVM based baseline and Bert finetuning scripts in different folders.
2. Each of the folders has `data_preparation_scripts` folder which contains code to process the data for training the models.
3. Data preparation for Bert involves different steps, run the following scripts in the same order `format_urdu_data.ipynb`, `aligning_sentences.ipynb` and `create_final_labelled_data.ipynb`. Please be careful in changing the file names as requires as output of one script will be input for the successive/next script.
4. After running data preparation scripts run the main scripts `finetuning_bert_final.ipynb` for bert or `train_test_svm_urdu_final.ipynb` for SVM. Please check the notebooks carefully while running and follow instructions written in the notebooks. Change any training configuration as required.




## Pretrained models
Pretrained models are available in the [Drive link](https://iiitaphyd-my.sharepoint.com/:f:/g/personal/chowdam_v_research_iiit_ac_in/Er7zBe3Nx-9NuX_kl0XWR5kB93ZJoiLOtBIR7hWEbkdl1Q?e=bD4G9k)

## Data
1. Urdu data is used as a source language data and can be downloaded from this [link](https://ltrc.iiit.ac.in/hutb_release/)
2. The downloaded data don't have chunk head information, further to get chunk head information we have used the [github repo](https://github.com/Pruthwik/CHUNK-HEAD-COMPUTATION-WITH-ILMT-POS-TAGS).

## Translation
For translataion we have used google translate and translation should be done after running `format_urdu_data.ipynb`, as this script will generate a text file having all Urdu sentences.




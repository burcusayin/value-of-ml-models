# rethinking-ml-models

This repo includes **the companion code for the paper "Rethinking and Recomputing the Value of ML Models"**. We provide different notebooks to use based on your task. In order to run the value analysis on your own <model,task> pair, you should have the required csv files for your data and a ".npy" formatted file of the confidence scores of your model on validation and test sets. 

We provide the notebook "_create_and_save_confidence_array.ipynb_" for an example of running a simple Logistic Regression model and saving its confidence outputs as a ".npy" file. Then, you can use either "_value_analysis_binary.ipynb_" or "_value_analysis_mclass.ipynb_" notebooks based on your classification task (binary or multi-class). 

If you would like to test what happens if you first calibrate your model via temperature scaling and then run the value analysis, you should use one of the following notebooks: "_value_analysis_with_temperature_scaling_binary.ipynb_" or "_value_analysis_with_temperature_scaling_mclass.ipynb_". 

If you would like to tune the empirical threshold on the test set for the value analysis, you should use one of the following notebooks: "_value_analysis_tuning_threshold_on_test_set_binary.ipynb_" or "_value_analysis_tuning_threshold_on_test_set_mclass.ipynb_". 

Finally, we also provide a notebook which shows how to fine-tune GPT-3 on Multi-Domain Sentiment Dataset and run the tests for binary sentiment analysis: "_fine_tuning_and_testing_GPT3_on_MDS_dataset.ipynb_". We inluded explanations in each notebook to guide you set the required parameters. 

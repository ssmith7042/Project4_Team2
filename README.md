# Project 4 - UPenn Data Science Boot Camp

Group Members: Rajib Maji, Hannah Whang, Michael Cariello, Theresa Bravo, Nick O'karma, Stephen Smith, Arame Diasse.

## Alzheimer Detection and Comparison Between Different Models

The goal for our project was to use machine learning techniques to predict the likelihood of an individual receiving a diagnosis of Alzheimer's disease. Our approach involved utilizing datasets containing medical data and patient details in order to create and train predictive models for patient diagnosis. 

## Questions to Consider:

1. Given the data available, are there certain characteristics such as age, sex, or education that correlate with an Alzheimer diagnosis?
2. Is there a preferred diagnostic method?
3. Of the models that we create, what classifier is the most accurate?
4. What tests correlate with the diagnosis of Alzheimer’s according to the DSM?


## Early Detection of Alzheimer 

First we tried to find out whether any early detection is feasible for Alzheimer / Dimnetia. We had used a Dataset from Kaggle ( https://www.kaggle.com/code/ahmedghobashi/detecting-early-alzheimer-s/input ) to find out which feature can be used to detect early alzheimer. Definitely early detection is better so that , more clinical options can be tried on patients as well as Patient's family can be prepared early if they know patient might have Alzhimer in future. 
We had used Logistic regression Model to find out which patient might have early symptomops of Alzheimer. 
There are 3 features - Age , MMSE ( Mini Mental State Examination ) and CDR ( Clinical Dementia Rating ) - These 3 features have pretty good correlation with symptomatic Alzheimer ( Demented ) . 
We had saved the Model and built a simple UI Screen to predit early detection of Alzheimer. 
Here is the Modules and description 
Supervised_RegressionModel_Alzheimer_Logistic regression.ipynb - Doing data fetch , data cleansing and model export
final_model.pkl - Final Model pkl file 
column_names.pkl - Input features pkl file
Flask_api_model_deployment.py - Flask API to predict the model 
UI_Predict.html - HTML Code to give inputs and predict the value. 

## Convolutional Neural Network

Next we explored supplementary image processing techniques using a dataset comprised of MRI brain scans. Our objective was to create a Neural Network that could determine if a new image of a MRI scan could lead to the diagnosis of Alzheimer's disease. A total of 3000 images were organized on Google Drive and catagorized into four groups: Moderate Demented, Mild Demented, Very Mild Demented, and Non Demented.  

The MRI dataset of patients diagnosed with Alzheimer's can be found [here.](https://www.frontiersin.org/articles/10.3389/fnins.2018.00777/full)

* Image size: approximately 4KB.
* Preprocessing and loading of images was done for each category. 
* Data  was trained, tested, one hot encoded, and a CNN model was created. 
* Initial accuracy was 50%.
* After more refinement, acurracy increased to 85%.
* Considerations: MRI scans can be costly to run. It can be difficult to explain neural networks because there are many parameters.

## Model using EEG data

The EEG data can be found [here](https://openneuro.org/datasets/ds004504/versions/1.0.6) as well as the [article](https://www.mdpi.com/2306-5729/8/6/95) and [Github](https://github.com/OpenNeuroDatasets/ds004504.git) links.
* Data was comprised of EEG resting state-closed eyes recordings from 88 subjects in total. A total of 36 were diagnosed with Alzheimer’s disease (AD group), 23 were diagnosed with frontotemporal dementia (FTD group), and 29 were cognitive and neuropsychological (CN). The CN state was evaluated by the international Mini-Mental State Examination (MMSE).
* EEG data is easier to process compared to MRI scans.
* Considerations: MMSE to determine different groups? Discuss efficacy? 

## Conclusions
	
**add here later!**


## Difficulties

Obtaining data for this project was difficult because medical data can be heavily restricted due to privacy concerns.

## Suggestions for the future

Find other datasets and pretrained models to compare model accuracy. Which method is the most accurate? 



# Problem Statement
> BeHealthy’ has a web platform that allows doctors to list their services and manage patient interactions and provides services for patients such as booking interactions with doctors and ordering medicines online. Here, doctors can easily organise appointments, track past medical records and provide e-prescriptions.

 Let’s take a look at the following snippet of medical data that may be generated when a doctor is writing notes to his/her patient or as a review of a therapy that he or she has done.

“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”

As you can see in this text, a person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where you can understand the terms ‘cancer’ and ‘chemotherapy’. 

We have been given such a data set in which a lot of text is written related to the medical domain. As we can see in the dataset, there are a lot of diseases that can be mentioned in the entire dataset and their related treatments are also mentioned implicitly in the text, which we saw in the aforementioned example that the disease mentioned is cancer and its treatment can be identified as chemotherapy using the sentence.


# Objective

- Our aim is to determine the disease name and its probable treatment from the dataset

- Two types of architectures suggested for analyzing videos using deep learning:

# Steps 

- Data preprocessing
- Concept identification
- Defining the features for CRF
- Getting the features words and sentences
- Defining input and target variables
- Building the model
- Evaluating the model
- Identifying the diseases and predicted treatment using a custom NER

## Define the features with the PoS tag as one of the features.
- While defining the features in which we have used the PoS tags, we also consider the preceding word of the current word. The use of the information of the preceding word makes the CRF model more accurate and exhaustive.
- Mark the beginning and the end words of a sentence correctly in the form of features

## Getting the features and the labels of sentences

-  Get the features value of a sentence after defining the features in the previous step.
-  Get a list of labels of a given preprocessed label line that you have created earlier

## Defining input and target variables

- Extract the features values for each sentence as an input variable for the CRF model in the test and the train dataset.
- Extract the labels as the target variable for the test and the train datase

## Model Description:
> Build the CRF model for a custom NER application using the features and the target variables.

## Conclusion

- We are able to predict the treatment given for the given disease
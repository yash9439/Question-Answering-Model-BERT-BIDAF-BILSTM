# Question Answering on Squad Dataset
This project explores different models for question answering on the Squad dataset, including BiLSTM, BIDAF, BERT Uncased, and DistilBERT. We evaluate these models based on their EM and F1 scores on the train and validation datasets. We also create an ensembling model that selects the answer with the highest F1 score among the four models for each question answer pair.

## Dataset
The Squad dataset is a collection of questions and answers that require a deep understanding of a given context paragraph. The dataset consists of over 100,000 question-answer pairs that are categorized into different topics.

## Models
We used four different models for question answering:
    1. BiLSTM
    2. BIDAF
    3. BERT Cased
    4. DistilBERT

We trained each model on the Squad dataset using the training split and evaluated their performance on the validation split. We also created an ensembling model that combines the outputs of these models to improve the overall performance.

## Results
=============================================================
<br>
EM Score on Validation Dataset using BiLSTM Model = 00.04433060782188947
F1 Score on Validation Dataset using BiLSTM Model = 28.518230394810734
<br>
---------------------------------
<br>
EM Score on Train Dataset using BiLSTM Model = 00.05989334377627533
F1 Score on Train Dataset using BiLSTM Model = 26.962483004132115
<br>
=============================================================
<br>
EM Score on Validation Dataset using BIDAF Model = 54.47480447480447
F1 Score on Validation Dataset using BIDAF Model = 66.80005949338813
<br>
---------------------------------
<br>
EM Score on Train Dataset using BIDAF Model = 49.979049303971324
F1 Score on Train Dataset using BIDAF Model = 65.12755191469993
<br>
=============================================================
<br>
EM Score on Validation Dataset using BERT Model = 57.90863668807994
F1 Score on Validation Dataset using BERT Model = 75.69647922632181
<br>
---------------------------------
<br>
EM Score on Train Dataset using BERT Model = 82.08618068677455
F1 Score on Train Dataset using BERT Model = 91.23183533851784
<br>
=============================================================
<br>
EM Score on Validation Dataset using DistilBERT Model = 56.13732637178603
F1 Score on Validation Dataset using DistilBERT Model = 75.30296296892632
<br>
---------------------------------
<br>
EM Score on Train Dataset using DistilBERT Model = 70.5635733290333
F1 Score on Train Dataset using DistilBERT Model = 87.81218393573155
<br>
=============================================================


After Ensembling the 4 models, 
EM Score on Validation Dataset using DistilBERT Model = 77.49800955414012
F1 Score on Validation Dataset using DistilBERT Model = 91.59243882523839
<br>
---------------------------------
<br>
EM Score on Train Dataset using DistilBERT Model = 85.91103408430431
F1 Score on Train Dataset using DistilBERT Model = 95.87697927456512


## Usage
To use this project, follow these steps:

## Download the Squad dataset.
Preprocess the data to extract questions, contexts, and answers for each example.
Train each model on the training split of the dataset.
Evaluate the performance of each model on the validation split of the dataset.
Create an ensembling model that combines the outputs of these models.
Evaluate the performance of the ensembling model on the validation split of the dataset.

## Conclusion
In conclusion, this project shows that BIDAF, DistilBERT, BERT and ensembling models are effective for question answering on the Squad dataset, while BiLSTM did not perform well. Ensembling can further improve the performance of individual models. However, more advanced models and techniques could be explored to enhance the performance of question answering systems.


Note : The code for the 4 Models are present in their respective model name folders.
Note : For all the Saved model are in savedModel inside each model folder.
Note : EMBEDDING Contains the GLOVE embedding used.
Note:  ensemble contains the ensembling model
Note: The same submission with all the saved Model are present at : 

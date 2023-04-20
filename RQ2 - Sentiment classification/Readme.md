# Sentiment classification 
### Potential of automatic labelling to enrich datasets  


**Setup with human labels (vote) and automatic labels (VACER, Textblob, Afinn**  
  
Experiment #    | Train labelling           | Test labelling  
_1 		| human labelling       | human labelling  
2 		| automatic labelling | automatic labelling  
3 		| automatic labelling | human labelling_  



### Overview of experiments with small random sample of cleaned Parlvote data  
**Parlvote shape:** 30144 rows × 26 columns  
**Random sample:** 1000 rows  
**BiLSTM parameters:**   
NO cross-validation | NO parameter optimization  
lstm_units=64  
spatial_dropout_rate=0.2  
dense_units=32  
learning_rate=1e-3  
batch_size=32  
epochs=10  


**Experiment 1: HUMAN --> TRAIN: human | TEST: human**  
Accuracy: 0.58  
Precision: 0.6726315789473685  
Recall: 0.58  
F1-score: 0.46799999999999997  
Majority baseline for vote_positive, vote_negative:  
  Majority class: vote_positive  
  Baseline accuracy: 54.60%  
  
**#Experiment 2 VADER --> TRAIN: automatic | TEST: automatic**  
Accuracy: 0.85  
Precision: 0.8375893769152196  
Recall: 0.85  
F1-score: 0.8322198892918498  
Majority baseline for vader_positive, vader_negative:  
  Majority class: vader_positive  
  Baseline accuracy: 81.50%  
  
**#Experiment 3 VADER --> TRAIN: automatic | TEST: human**  
Accuracy: 0.575  
Precision: 0.5971939517301541  
Recall: 0.575  
F1-score: 0.4884296478451401  
Majority baseline for vote_positive, vote_negative:  
  Majority class: vote_positive  
  Baseline accuracy: 54.60%  
  
**#Experiment 4 TEXTBLOB --> TRAIN: automatic | TEST: automatic**  
Accuracy: 0.89  
Precision: 0.89  
Recall: 0.89  
F1-score: 0.89  
Majority baseline for textblob_positive, textblob_negative:  
  Majority class: textblob_positive  
  Baseline accuracy: 89.60%  
  
**#Experiment 5 TEXTBLOB --> TRAIN: automatic | TEST: human**  
Accuracy: 0.555  
Precision: 0.6043147208121827  
Recall: 0.555  
F1-score: 0.4099085846380162  
Majority baseline for vote_positive, vote_negative:  
  Majority class: vote_positive  
  Baseline accuracy: 54.60%  
  
**#Experiment 6 AFINN --> TRAIN: automatic | TEST: automatic**  
Accuracy: 0.815  
Precision: 0.8057187499999999  
Recall: 0.815  
F1-score: 0.8083229162903284  
Majority baseline for afinn_positive, afinn_negative:  
  Majority class: afinn_positive  
  Baseline accuracy: 75.40%  
  
**#Experiment 7 AFINN --> TRAIN: automatic | TEST: human** 
Accuracy: 0.54  
Precision: 0.49877717391304344  
Recall: 0.54  
F1-score: 0.43732511872673596  
Majority baseline for vote_positive, vote_negative:  
  Majority class: vote_positive  
  Baseline accuracy: 54.60%  


# Emotion Recognition with Multi-modal data using AI techniques
## Overview
Identifying emotion from speech is a non-trivial task pertaining to the ambiguous definition of emotion itself. In this work, we build light-weight multimodal machine learning models and compare it against the heavier and less interpretable deep learning counterparts. Our experiments show that the light-weight models are comparable to the deep learning baselines and even outperform them in some cases, achieving state-of-the-art performance on the IEMOCAP dataset.
The dataset is used to train two types of models:

ML-based: Logistic Regression and Random Forest.

DL-based: LSTM Classifier, CNN and Transfomer.

This project was conducted with significant guidance from prior research and insights drawn from various peer-reviewed research papers particularly from -"MULTIMODAL SPEECH EMOTION RECOGNITION AND AMBIGUITY RESOLUTION", by [Gaurav Sahu](https://github.com/Anshika101/Minor_Dissertation/blob/main/Paper%20Review.pdf) which provided a strong theoretical and methodological foundation for the work.

For a more detailed explanation, please check the [report](https://github.com/Anshika101/Minor_Dissertation/blob/main/Report%20(1).pdf).
## Datasets
The [IEMOCAP](https://github.com/Anshika101/Minor_Dissertation/blob/main/IEMOCAP.pdf) dataset was used for all the experiments in this work.
You can access the preprocessed data files from here:
(https://www.dropbox.com/scl/fo/jdzz2y9nngw9rxsbz9vyj/h?rlkey=bji7zcqclusagzfwa7alm59hx&dl=0)
## To Run the Code
1. Run `Emotion_Recognition_with_Multi_modal_data.ipynb` to train ML and DL classifiers for text
2. Run `Emotion_Recognition_with_Multimodal_Data_2.ipynb` to train ML and DL classifiers for audio
3. Run `Emotion_Recognition_using_multimodal_data_3.ipynb` to train ML and DL classifiers for audio+text
## Results
Accuracy, F-score, Precision and Recall has been reported for the different experiments.

**Audio**

Models | Accuracy | F1 | Precision | Recall
---|---|---|---|---
RF | 56.9 | **56.3** | 58.0 | **57.3**
LR | 32.3 | 15.0 | 19.1 | 21.2
CNN | 49.8 | - | - | -

**Text**

Models | Accuracy | F1 | Precision | Recall
---|---|---|---|---
RF | 61.4 | 60.7 | 63.8 | 62.3
LR | 61.4 | 62.7 | 67.2 | 60.8
LSTM | 63.1 | - | - | -

**Audio + Text**

Models | Accuracy | F1 | Precision | Recall
---|---|---|---|---
RF | 66.1 | 66.2 | 71.4 | 65.7
LR | 63.1 | 64.3 | 68.6 | 62.0
CNN | 67.1 | - | - | -
TRANSFORMER | 63.6 | - | - | -
## Conclusion
This Dissertation demostrates that multimodal data, specifically the combination of text and audio, significantly enhances the performances of emotion through Machine Learning and Deep Learning models compared to individual modalities.
The findings indicate the integrating both text and audio data leads to improved accuracy. Intrestingly, the study also reveals that simple Machine Learning models, uch as Random Forest or Logistic Regression, perform comparably to more complex Deep Learning Models suggesting that for certian tasks, the additional complexity of Deep Learning Models may not always yield substantial improvements or we need to incorporate some additional changes to deep learning models.
These results underscore the potential of multimodal fusion for improving model accuracy while also highlighting the efficiency and practicality of using simpler machine learning algorithms in such tasks. 


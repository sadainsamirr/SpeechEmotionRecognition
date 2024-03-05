# Speech Emotion Recognition

Involves recognizing human emotions and affective states from speech audio data. Using machine learning techniques, particularly deep learning, the program analyzes audio files and classifies them into different emotion categories such as anger, disgust, fear, happiness, neutral, sadness, and surprise. The model is trained on a dataset containing audio recordings of various emotions and achieves high accuracy in predicting the emotional content of new audio samples. SER has applications in call centers for analyzing customer interactions, in-car systems for ensuring driver safety, and various other fields where understanding human emotions from speech is valuable.

## Introduction

But first, we need to learn about what Speech Emotion Recognition (SER) is and why we are building this project. Speech Emotion Recognition, abbreviated as SER, is the act of attempting to recognize human emotion and affective states from speech. This is capitalizing on the fact that the voice often reflects underlying emotion through tone and pitch. This is also the phenomenon that animals like dogs and horses employ to be able to understand human emotion.

### Why do we need SER?

Emotion recognition is part of speech recognition that is gaining more popularity and the need for it increases enormously. Although there are methods to recognize emotion using machine learning techniques, this project attempts to use deep learning to recognize emotions from data.

SER (Speech Emotion Recognition) is used in call centers for classifying calls according to emotions and can be used as the performance parameter for conversational analysis, thus identifying unsatisfied customers, customer satisfaction, and so on, for helping companies improve their services.

It can also be used in-car board systems based on information of the mental state of the driver, providing the system with the ability to initiate safety measures, preventing accidents from happening.

## Dataset

The dataset used in this project is the Toronto emotional speech set (TESS). It contains a total of 2800 audio files with expressions of 7 different emotions. The emotions include anger, disgust, fear, happiness, neutral, sadness, and surprise.

## Preprocessing

The audio data is preprocessed using the librosa library. Preprocessing steps include loading the audio files, extracting features such as MFCC (Mel-Frequency Cepstral Coefficients), and normalizing the feature values.

## Model Architecture

The deep learning model architecture used for this project consists of an LSTM (Long Short-Term Memory) layer followed by fully connected layers. The model is trained to classify input audio features into one of the seven emotion categories.

## Training

The model is trained using the Adam optimizer and categorical cross-entropy loss function. The training process involves splitting the dataset into training and validation sets. Training is performed for 50 epochs with a batch size of 64.

## Evaluation

The trained model achieves an accuracy of approximately 99.5% on the validation set. Evaluation metrics such as accuracy, precision, recall, and F1-score are computed to assess the model's performance.

# Classification of Epileptic EEG Recordings Using Signal Transforms and Convolutional Neural Networks

This repository contains my implementation of the paper "Classification of Epileptic EEG Recordings Using Signal Transforms and Convolutional Neural Networks" by Rubén San-Segundo, Manuel Gil-Martín, Luis Fernando D'Haro-Enríquez, and José Manuel Pardo.

As the original authors did not provide publicly available code, I re-implemented their methodology in Python based on the descriptions in the paper. This project applies their approach to the original EEG dataset used in the study, and additionally explores the generalizability of the method by applying it to a music signal dataset (GZTAN).

Signal Processing Summary paper.pdf - Summarizes everything I've done, including some mathematical explanations of some subjects appearing in the paper

Signal Processing Proof of Concept.ipynb - Implementation of the algorithm on the EEG Epileptic Seizure Recognition dataset https://www.kaggle.com/datasets/harunshimanto/epileptic-seizure-recognition


Signal Processing GZTAN.ipynb - Main Code, Implementing the algorithm on the GZTAN music dataset. Added another feature extraction procedure (Mel-Spectogram as input!)

Signal Processing Extra Statistics.ipynb - Attempting to gain further understanding of the data and our findings. Performing statistical tests to compare the different experiments.


In short, What this paper does it attempt to use different feature extraction methods from the Signal Processing world such as fourier transform, EMD, Wavelet etc. and feed them into a CNN model in order to classify different EEG signals (ictal, non-ictal, etc.) I thought it would make sense to add an additional feature extraction method and take the mel spectogram and input it as a picture to the CNN model.

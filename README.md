# Intro

This repository contains the work and findings of our experiment in high-energy physics, focusing on the classification of jet substructures using Deep Learning techniques. Our aim was to distinguish between jet substructures arising from bosonic decays and those originating from quark-gluon plasma.
## Project Overview
The primary goal of this experiment was to train and evaluate Deep Learning architectures for the classification of hadronic jets in high-energy physics experiments. Specifically, we aimed to identify substructures resulting from bosonic decays and those produced by gluon and quark plasma created in hadronic beam collisions. Given that particle measurements can be projected onto a cylindrical detector and then unrolled into two-dimensional images, our data lends itself well to analysis using computer vision techniques. Hence, hadronic jet classification was performed using Deep Neural Networks trained on simulated detector response data, or alternatively, by creating highly specific high-level features and combining them with shallow Machine Learning algorithms like Boosted Decision Trees.
## Dataset
The dataset utilized in this study is based on simulated events, with collision and immediate decays simulated using MADGRAPH5 v2.2.3, and hadronic showers and hadronization processes using PYTHIA v6.426. The data is available in two formats:

- 32x32 images representing the energy distribution in a calorimeter.
- Arrays containing six high-level features, including jet invariant mass and energy correlation functions.

## Models
We explored two main approaches for this classification task:

1. Decision Tree Classifier using high-level features, optimized with AdaBoost for efficient classification.
2. Deep Neural Network (DNN) based on an 8-layer architecture with locally connected and fully connected layers, specifically designed for the 32x32 image dataset.

Results
Our experiments demonstrate the potential of Deep Learning in the field of high-energy physics, with the DNN model showing a slight advantage over the Decision Tree Classifier in terms of AUC and accuracy. These findings suggest that deep learning architectures can effectively handle complex, high-dimensional datasets typical in physics research.

# Fluid overload predicting using a meta-model with the integration of synthetic data 

This repo aims to provide insight into the workflow of the ["Improving mixed-integer temporal modeling by generating synthetic data using conditional generative adversarial networks: a case study of fluid overload prediction in the intensive care unit"](https://www.sciencedirect.com/science/article/abs/pii/S0010482523012143) paper, not a nuanced analysis and step-by-step coding and achieving the results summarized in the paper. That said, you can easily use and expand the provided workflow and draw the appropriate performance results based on your application and available data.

## Overview
![](Overview.png)

### Objective
The challenge of mixed-integer temporal data, which is particularly prominent for medication use in the critically ill, limits the performance of predictive models. The purpose of this evaluation was to pilot test integrating synthetic data within an existing dataset of complex medication data to improve machine learning model prediction of fluid overload. 
### Materials and Methods
This retrospective cohort study evaluated patients admitted to an ICU ≥ 72 hours. Four machine learning algorithms to predict fluid overload after 48-72 hours of ICU admission were developed using the original dataset. Then, two distinct synthetic data generation methodologies (synthetic minority over-sampling technique (SMOTE) and conditional tabular generative adversarial network (CTGAN)) were used to create synthetic data. Finally, a stacking ensemble technique designed to train a meta-learner was established. Models underwent training in three scenarios of varying qualities and quantities of datasets. 
### Discussion 
The integration of synthetically generated data is the first time such methods have been applied to ICU medication data and offers a promising solution to enhance the performance of machine learning models for fluid overload, which may be translated to other ICU outcomes. A meta-learner was able to make a trade-off between different performance metrics and improve the ability to identify the minority class. 

If you are interested, please cite:

```
@article{RAFIEI2023107749,
title = {Improving mixed-integer temporal modeling by generating synthetic data using conditional generative adversarial networks: A case study of fluid overload prediction in the intensive care unit},
journal = {Computers in Biology and Medicine},
pages = {107749},
year = {2023},
issn = {0010-4825},
doi = {https://doi.org/10.1016/j.compbiomed.2023.107749},
url = {https://www.sciencedirect.com/science/article/pii/S0010482523012143},
author = {Alireza Rafiei and Milad {Ghiasi Rad} and Andrea Sikora and Rishikesan Kamaleswaran},
keywords = {Critical care, Fluid overload, GAN, Machine learning, Mixed-integer temporal modeling, Synthetic data}}
```

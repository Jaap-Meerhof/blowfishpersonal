---
title: "Master Thesis"
date: 2023-06-25T20:53:32+02:00
draft: false
---

For my master thisis I worked at the RIVM (National Dutch Institute for Health and Nature). I investigated the privacy challenges in applying Gradient Boosted Decision Trees in a Federated setting. With the main question being: is your personal health data safe when this data is used in machine learning models where the different parties train together.

## Federated Learning

The RIVM is investigating the viability of using federated learning for a data set that is currently being standardized between hospitals. Different hospitals will carry the same features, for example age, sex and medicine used will be stored for different patients on different hospitals. The hospitals and other health organizations can collaboratively create one model on this standardized data set. Federated Learning could be the Perfect solution for this problem.

## XGBoost

XGBoost is a quite new Gradient Boosted Decision Tree (GBDT) algorithm which builds upon the concept of GBDTs by adding extra regularization parameters and other computational speedups. There are algorithms to use XGBoost in federated settings by numerous papers. [Check my paper (grade=8.0) ](https://essay.utwente.nl/97917/) or [GitHub](https://github.com/Jaap-Meerhof/Federated_XGBoost_Python).

## Results
I was able to create an attack that used extra information retrieved during training to create an attack that was stronger than a "normal" attack.
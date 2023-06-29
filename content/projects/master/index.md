---
title: "Master Thesis"
date: 2023-06-25T20:53:32+02:00
draft: false
---

I'm currently busy with my assignment for the RIVM (National Dutch Institute for Health and Nature). I'm investigating the privacy challenges in applying Gradient Boosted Decision Trees in a Federated setting. With the main question being: is your personal health data safe when this data is used in machine learning models (specifically XGBoost) where the models are shared with other parties.

## Federated Learning

The RIVM is investigating the viability of using federated learning for a data set that is currently being standardized between hospitals. Different hospitals will carry the same features, for example age, sex and medicine used will be stored for different patients on different hospitals. The hospitals and other health organizations can collaboratively create one model on this standardized data set. Federated Learning could be the Perfect solution for this problem.

## XGBoost

XGBoost is a quite new Gradient Boosted Decision Tree (GBDT) algorithm which builds upon the concept of GBDTs by adding extra regularization parameters and other computational speedups. There are algorithms to use XGBoost in federated settings by numerous papers. [Check my preparatory work paper (grade=8.0) ](https://jaapmeerhof.nl/index.php/s/Wpd4JrQoa9QdmPT).

## Outlook
Currently I just finished creating the federated version of XGBoost for binary classification. Which I'll have to adapt to multi-class classification. After that I'll be able to attack the simulated network and hopefully create an attack which takes advantage of the intermediate shared information. 
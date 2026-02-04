# Woosong University Introduction to Machine Learning Project

# Reference Paper
X. Huang et al., "InterDIA: Interpretable prediction of drug-induced autoimmunity through ensemble machine learning approaches," Toxicology, vol. 511, p. 154025, 2025.
https://www.sciencedirect.com/science/article/abs/pii/S0300483X25000204

# Abstract
In pharmaceutical drug development, one challenge is avoiding drug-induced autoimmunity (DIA) where compounds trigger immune responses leading to various autoimmune conditions. 
Several existing computational approaches focus primarily on predicting DIA toxicity but do not address drug-likeness properties essential for therapeutic viability. 
This study attempts DuaSHAP, a dual-model SHAP (SHapley Additive exPlanations) framework which identifies molecular features that optimize both safety (reduced DIA risk) and favorable drug-like properties. Using the InterDIA dataset comprising 597 compounds characterized by 196 RDKit molecular descriptors, two XGBoost classifiers were trained: 
1. DIA toxicity prediction
2. Drug-likeness classification based on Lipinski's Rule of Five criteria.

SHAP values were extracted and normalized and an Antagonistic Feature Matrix categorizing 178 common descriptors into four quadrants was constructed.
As a result, 18 "Sweet Spot" features exhibiting the desirable combination of decreasing DIA risk while enhancing drug-likeness were identified.
Robustness validation was conducted across five random seeds and 13 of these features (72%) remained stable including topological indices such as BalabanJ and Kappa shape indices, and also surface area descriptors like SMR_VSA5.
These findings provide actionable guidance for molecular optimization in drug design to minimize DIA risk and maximizing drug-likeness.

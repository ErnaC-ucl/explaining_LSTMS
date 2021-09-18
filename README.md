# explaining_LSTMS

# Project summary 
This study aims at providing interpretability to a long-short term memory (LSTM) model
that is used to obtain predictions of corporate bonds’ spread changes. Spreads are often
used as an indication of the market’s assessment of credit risk. Accurately predicting
spread changes has important implications for portfolio managers and fixed-income practitioners, as it is one of the main criteria that guides their investment decisions. While LSTM models have high predictive accuracy, they inherently suffer from low explainability.
A key concern is their reputation as “black box” models — i.e., it is hard for decisionmakers to understand the input transformations through multiple layers of the network and obtain insights of why certain predictions are made.

The objective of this thesis is to identify and implement explainable artificial intelligence
(XAI) methods that can shed light into the interpretability of the LSTM model by quantifying the magnitude and the directional impact of individual features on the predicted output. Enhancing model’s interpretability not only helps the end-user build trust on the
predicted output, but it is also an explicitly stated requirement across various regulatory
frameworks such as General Data Protection Regulation (GDPR) set by the European
Union.

A combination of model-specific and model-agnostic XAI methods have been used in this
thesis namely, DeepSHAP which is an approximation of Shapley values applied to deep
learning models, knowledge distillation with SHAP’s tree explainer (using random forest and extreme gradient boosting (XGBoost) as student models), LSTM with layer-wise
propagation, and an interpretable multi-variable LSTM using mixture attention mechanisms.

The original contribution of this project is: 
- i) applying various XAI methods to the LSTM
model and 
- ii) evaluating their performance based on the criteria of interpretability, computational efficiency, accuracy and fidelity. We conclude that knowledge distillation based on the XGBoost student model is the best method for our use case, because it provides
computationally efficient and intuitive explanations with a reasonable level of accuracy and
fidelity. 

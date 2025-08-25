# Dementia-Prediction

## Abstract
Dementia is a progressive neurological disorder that impairs memory, thinking,
 and behavior, posing a growing burden on aging populations worldwide. There
 is no cure; we can only slow down the progression of the disease. This study exam
ines gender-based differences in feature importance for predicting dementia using
 two datasets: the OASIS-1 and a publicly available Kaggle dementia prediction
 dataset. Each dataset was split on the basis of gender and was analysed separately
 using the Random Forest, LightGBM, and Logistic Regression models. The result
 indicated only a slight difference in feature importance between male and female
 sets. Notably, socioeconomic status was seen as a more significant predictor for
 males than females in the OASIS dataset, while the Kaggle dataset showed mini
mal gender related differences. These findings suggest that the minimal differences
 in feature importance across genders may be attributed to the limited and shared
 set of features used in the datasets, which did not include gender-specific factors
 such as hormonal or biological variables

## Result
 From the SHAP analysis of both Random Forest and LightGBM models,
 Depression Status Yes and APOE ε4 consistently emerged as the most influential predic
tors of dementia across both male and female subsets. This aligns with
 epidemiological findings demonstrating that depressive symptoms significantly increase
 dementia risk, particularly in APOE4 carriers. Notably, Smoking Status Current
 Smoker ranked among the top three features in the Random Forest models for both
 genders, though its importance was lower in the LightGBM model in case of female sub
set. Interestingly, the beeswarm plots indicate that being a current smoker is associated
 with a lower likelihood of dementia in this dataset, contradicting the majority of existing
 studies. This inconsistency suggest that there might be some dataset-specific biases,
 unaccounted confounding factors, or sampling imbalances.
 For males, additional contributors such as BloodOxygenLevel, BodyTemperature, and
 Weight featured prominently, with relatively stable rankings between the two models. For
 females, Education Level No School was consistently among the top predictors in both
 models, a factor not observed in the male subset. Other common contributors for fe
males included BloodOxygenLevel and BodyTemperature, though the magnitude and
 ranking varied slightly between Random Forest and LightGBM. Comparing both gen
ders, the dominance of Depression Status Yes and APOE ε4 across both models and
 datasets underscores their robust predictive role in dementia classification. However, the
 gender-specific prominence of Education Level No School in females and its absence in
 the male top rankings suggests possible socio-educational influences on dementia risk
 that may interact differently across genders. Meanwhile, physiological features such as
 BloodOxygenLevel and BodyTemperature remained consistently relevant for both gen
ders, reinforcing their potential as stable clinical indicators despite variations in model
 architecture.

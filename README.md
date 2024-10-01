# Organ-failure
This repository contains the codes and scripts associated with the article titled "Prediction of ICU Needs and Organ Failures in Infectious Patients Using Initial Admission Data: A Machine Learning-Based Multicentre Study."

## Importance:  
Predicting severe outcomes and identifying organ failure early can help reduce medical costs and mortality rates for patients.  

## Objective:  
This study aimed to develop predictive models using data from initial admission to identify hospitalized patients at high risk for intensive care requirements and organ failure.  

## Design, Setting, and Participants:  

This retrospective cohort study included 18,689 patients with confirmed infectious events. Data were collected from the First Affiliated Hospital of Xiamen University (XMFH), where 5,132 patients were admitted between January 1, 2019, and December 31, 2023, and from the Medical Information Mart for Intensive Care (MIMIC)-III and MIMIC-IV databases, which contributed 13,557 patients.  

## Main Outcomes and Measures:  

A total of 49 variables, including demographics, laboratory tests, and comorbidities, were used in the ML model to predict future ICU requirements and organ failure risk. Model performance was assessed using internal five-fold cross-validation and comprehensive external validation with metrics such as accuracy and sensitivity. SHAP analysis was employed to interpret the model, identify key features, and further validate its performance in real-world cases.  

## Results: 

The CatBoost model demonstrated the best performance in ICU model, with an area under the receiver operating characteristic curve (AUC) of 0.956. For organ failure prediction, CatBoost achieved the highest overall AUCs for renal (0.833), cardiac (0.723), respiratory (0.658), and both hepatic and coagulation failures (0.839). The Random Forest model excelled specifically in predicting respiratory and renal failures, with AUCs of 0.677 and 0.836, respectively. Model interpretability was supported by real clinical case analyses, showing that abnormal indicators aligned with key features identified by the models.  

## Conclusions and Relevance:

By leveraging data extracted from the initial admission, our models predict the need for intensive care and identify patients at high risk for organ failure, with the majority of models achieving AUCs exceeding 0.8. These findings can guide early decision-making, optimize resource allocation, ultimately improve survival rates and outcomes.

## Version  
Python 3.11.7.  

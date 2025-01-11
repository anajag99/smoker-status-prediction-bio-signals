# Smoker Status Prediction Using Bio-Signals  

## Project Overview  
This repository focuses on the binary classification of smoker status using bio-signal data. By using machine learning models, the project aims to predict smoking behaviors based on physiological and biochemical attributes, contributing to advancements in public health and smoking cessation efforts.  

---

## Dataset  
### Source  
The dataset is sourced from Kaggle, originally used for predicting smoker status with bio-signals. It includes pre-split training and testing subsets.  

### Features  
The dataset includes the following key attributes:  
- **Demographics**: Age, Height, Weight, Waist Circumference  
- **Vision & Hearing**: Eyesight (left/right), Hearing (left/right)  
- **Blood Metrics**: Systolic/Diastolic Pressure, Fasting Blood Sugar, Cholesterol (Total, HDL, LDL), Triglycerides  
- **Liver Function**: AST, ALT, GTP  
- **Miscellaneous**: Hemoglobin, Urine Protein, Serum Creatinine, Dental Caries  

---

## Methodology  
### Exploratory Data Analysis (EDA)  
- Descriptive statistics (`describe`) for understanding data distribution.  
- KDE plots for visualizing feature distributions.  
- Data type checks and null-value handling for preprocessing.  

### Models Trained  
1. **Logistic Regression**  
   - Linear classifier trained on standardized data.  
   - Evaluation metrics: Accuracy, Confusion Matrix, Classification Report.  

2. **Simple Neural Network**  
   - Single hidden layer with binary cross-entropy loss.  
   - Optimized using the Adam optimizer.  

3. **Radial Basis Function (RBF) SVM**  
   - Kernel-based classifier with RBF kernel for non-linear patterns.  

4. **Multi-Layer Perceptron (MLP)**  
   - Two hidden layers implemented using scikit-learn.  

5. **Feedforward Neural Network (FNN)**  
   - Built with TensorFlow/Keras, featuring two hidden layers.  

---

## Evaluation Metrics  
- **Accuracy**: Overall correctness of predictions.  
- **Precision**: Focus on minimizing false positives.  
- **Recall**: Sensitivity to true positives.  
- **F1-Score**: Harmonic mean of Precision and Recall.  
- **AUC-ROC**: Discriminative ability across thresholds.  
- **Confusion Matrix**: Breakdown of true/false positives and negatives.  

---

## Results  
| Model                  | AUC Score | Testing Accuracy | Training Accuracy |  
|------------------------|-----------|------------------|-------------------|  
| Logistic Regression    | 0.72      | 0.67             | 1.00              |  
| RBF SVM                | 0.75      | 1.00             | 1.00              |  
| Simple Neural Network  | 1.00      | 0.73             | 1.00              |  
| Feedforward NN         | 0.75      | 0.74             | 1.00              |  
| MLP                    | 0.75      | 0.73             | 1.00              |  

---

## Future Enhancements  
1. Expand the dataset to improve model robustness.  
2. Collaborate with healthcare professionals for domain-specific insights.  
3. Integrate predictive models with behavioral intervention strategies.  

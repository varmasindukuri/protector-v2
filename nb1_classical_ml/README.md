## Dataset
CIC-IDS 2018 - 80 network flow features - 358MB CSV

## Models Trained
- One-Class SVM (anomaly detection on benign traffic only)
- Binary SVM (supervised benign vs attack)
- Decision Tree (multi-class attack classification)
- Random Forest (200 estimators, balanced class weights)
- Gaussian Naive Bayes
- Extreme Learning Machine (ELM) - single-pass training
- Isolation Forest (unsupervised)
- Gradient Boosting, Voting Ensemble, AdaBoost, Bagging
- Deep Neural Network (TF/Keras)

## How to Run
1. Add CIC-IDS 2018 dataset on Kaggle
2. Run cells top to bottom
3. Download models/ folder from output tab

   ## Output Files
All .pkl and .keras files saved to models/

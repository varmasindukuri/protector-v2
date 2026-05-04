## Purpose
Adds explainability layer on top of NB1 classical models.

## Methods
- SHAP TreeExplainer - global + per-family feature importance
- SHAP beeswarm plots - shows feature value vs impact distribution
- GradCAM for 1D CNN - attention heatmap over timesteps
- Family Classifier (RF) - BruteForce/DoS/Malware/WebAttack/Normal
- Stacking Ensemble - meta LogisticRegression on base model probabilities

## How to Run
Run after NB1 (needs v2_rf.pkl, v2_gbc.pkl etc from NB1)

## Output Files
v2_shap_explainer.pkl, v2_shap_arr.npy,
v2_family_clf.pkl, v2_ensemble_meta.pkl,
v2_gradcam_model.keras + PNG plots

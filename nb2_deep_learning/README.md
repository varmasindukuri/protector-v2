## Dataset
UNSW-NB15 - 45 features - training-set + testing-set CSVs provided

## Models Trained
- 1D CNN (local pattern detection)
- LSTM + Bidirectional LSTM (temporal modeling)
- GRU (gated recurrent)
- CNN+LSTM hybrid
- ResNet-1D (residual connections)
- GAN (attack sequence synthesis for augmentation)
- LSTM Autoencoder (reconstruction-based anomaly)

## Sequence Design
T=20 timestep sliding window, step=5

## How to Run
Kaggle GPU runtime required (T4 or P100)

## Output Files
All .keras files saved to models/

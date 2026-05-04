## Dataset
BETH - host process logs (testing/training/validation)
     + DNS logs (labelled_2021may-*-dns.csv)

## Methods
- HMM per attack class (normal, sus, evil) - Viterbi + Baum-Welch
- K-Means clustering with elbow and silhouette analysis
- HDBSCAN density clustering (discovers unknown attack families)
- Process2Vec - Word2Vec on syscall event sequences
- PCA2Vec - 95% variance compressed embeddings
- HMM2Vec - encode samples as HMM log-likelihood vectors
- Transfer Learning - freeze encoder, fine-tune on 200 samples

## How to Run
Kaggle CPU runtime (no GPU needed)

## Output Files
.pkl models, .model (Word2Vec), .npy arrays saved to models/

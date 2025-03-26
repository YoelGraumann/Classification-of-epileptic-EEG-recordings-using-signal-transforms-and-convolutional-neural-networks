🎧 EEG-Inspired Deep Learning for Music Genre Classification
This project reimplements and extends the deep learning pipeline from "Classification of epileptic EEG recordings using signal transforms and convolutional neural networks" by San-Segundo et al., originally designed for EEG seizure detection. The core idea is to test the transferability of biomedical signal processing techniques to a completely different domain: music genre classification.

Using the GTZAN dataset, a standard benchmark in music information retrieval, this project applies a CNN architecture coupled with various time-frequency signal transformations—Fourier, Wavelet, Empirical Mode Decomposition (EMD), and Mel Spectrograms—to classify music genres. The model was thoroughly validated using 5-fold cross-validation and extended statistical analysis, including the Friedman and Nemenyi tests, to ensure robustness and compare transform effectiveness.

🚀 Features
📊 Multi-class (10 genres) classification using CNNs

🔁 5-fold Cross-Validation with repeat runs (10 seeds) for robust evaluation

🧠 Signal transforms used as feature extraction methods:

Butterworth filtering

Fourier Transform

Daubechies Wavelets

Empirical Mode Decomposition (EMD)

Mel Spectrograms (added in this project)

Concatenated "ALL" transform (Raw + Fourier + Wavelet + EMD)

🔬 Statistical Evaluation with:

Confusion Matrices

Precision, Recall, and F1 Score

Friedman and Nemenyi tests for significant differences between transforms

📁 Dataset
EEG (San-Segundo et al.) — Used for initial proof of concept

GTZAN — 1000 music clips across 10 genres, 30s each, mono, 22050 Hz sampling rate

📌 Highlights
Implementation built entirely from scratch (TensorFlow 2) based on the paper’s description

Robust experimental design with repeated runs and variable fold-seeds

Mel spectrograms consistently outperformed all other transforms in genre classification

Classical music genre had significantly higher recall across all transforms

Spectral smoothness analysis helps explain genre-specific performance patterns

🧪 Results Summary
🎼 Mel Spectrogram was the top-performing transformation with the highest mean accuracy and statistically significant advantage

🎧 Fourier Transform ranked second

📉 Raw and EMD performed the lowest but were the most stable across runs

📊 Statistical analysis confirms significant differences among signal transformations

🧠 Inspiration
By bridging domains, this project shows how bio-signal processing pipelines can be adapted to musical audio analysis, offering potential insights for transfer learning across seemingly unrelated fields.

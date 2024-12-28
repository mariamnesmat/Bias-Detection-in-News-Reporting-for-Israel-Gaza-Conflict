# Bias Detection in News Reporting: NLP Framework for Israel-Gaza Conflict
This project presents an NLP-based framework for detecting bias in news reporting, focusing on the politically sensitive and polarized context of the Israel-Gaza conflict. The framework leverages Nakba narratives as linguistic resources and uses advanced preprocessing, class imbalance mitigation, and state-of-the-art machine learning models to improve bias detection accuracy.

# Dataset
The dataset consists of multilingual news articles annotated for bias and propaganda, focusing strongly on Arabic texts. The dataset includes:
- **Nakba Narratives**: Linguistic resources for bias analysis.
- **Annotations**: Bias and propaganda labels curated for training and evaluation.

# Methodology
The project explores various approaches, including:
- **Traditional ML Models**: Random Forest, XGBoost, Logistic Regression.
- **Deep Learning Models**: LSTM, Bi-LSTM, Bi-GRU with Attention.
- **Transformer-based Architectures**: AraBERT, T5-small.
- **Generative Models**: Leveraging large-scale pre-trained models for contextual understanding.

Key techniques include:
- **Preprocessing**: Tokenization, stemming, and noise removal.
- **Class Imbalance Handling**: Using Borderline-SMOTE and other augmentation methods.

# Results:
- The proposed framework achieved notable performance in bias detection, particularly with ensemble machine learning methods. Random Forest and XGBoost demonstrated the highest accuracy (93% and 92%, respectively), showcasing their effectiveness in handling the nuanced and imbalanced dataset. Deep learning models, such as LSTM, achieved moderate success (84% accuracy), while Transformer-based models like AraBERT exhibited reasonable performance (58% accuracy) but were limited by the dataset size and domain complexity. Generative models, including T5-small and Silma, struggled in this context, highlighting the challenges of applying generative approaches to bias detection tasks.

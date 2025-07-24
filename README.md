# Bias Detection in News Reporting: NLP Framework for Israel-Gaza Conflict

This project presents an NLP-based framework for detecting bias in news reporting, with a focus on the politically sensitive and polarized context of the Israel-Gaza conflict. The framework leverages **Nakba narratives** as linguistic resources and combines advanced preprocessing, class imbalance handling, and machine learning models to enhance bias detection accuracy.

## 🗂 Dataset

The dataset consists of multilingual news articles, primarily Arabic, annotated for bias and propaganda. It includes:

- **Nakba Narratives**: Used as linguistic indicators of bias and historical framing.
- **Annotations**: Manually labeled for bias direction and propaganda type.

## ⚙️ Methodology

The project explores multiple modeling strategies:

- **Traditional Machine Learning**: Random Forest, XGBoost, Logistic Regression.
- **Deep Learning**: LSTM, Bi-LSTM, Bi-GRU with Attention mechanisms.
- **Transformer Models**: AraBERT, T5-small (pre-trained models fine-tuned for bias detection).
- **Generative Approaches**: Tested large-scale generative LLMs for contextual bias interpretation.

Key techniques used:

- **Text Preprocessing**: Tokenization, stemming, stop-word removal, and normalization.
- **Imbalanced Class Handling**: Applied Borderline-SMOTE and data augmentation techniques.

## 📊 Results

The framework achieved competitive performance across models:

| Model                    | Accuracy |
|--------------------------|----------|
| Random Forest            | 93%      |
| XGBoost                  | 92%      |
| LSTM                     | 84%      |
| AraBERT                  | 58%      |
| T5-small / Silma (LLMs)  | Lower (limited by domain/data) |

Traditional ML models performed best on the imbalanced dataset. Deep learning models showed moderate success. Transformer and generative models struggled due to domain-specific vocabulary and limited training data.

## 📄 Publication

Available at: [ACL Anthology – 2025.nakbanlp-1.12](https://aclanthology.org/2025.nakbanlp-1.12/)

## 📚 Citation

If you use this work, please cite the following paper:

```bibtex
@inproceedings{mohammed-etal-2025-bias,
  title     = "Bias Detection in Media: Traditional Models vs. Transformers in Analyzing Social Media Coverage of the Israeli-{G}aza Conflict",
  author    = "Mohammed, Marryam Yahya and
               Mohamed, Esraa Ismail and
               Esmat, Mariam Nabil and
               Nagib, Yomna Ashraf and
               Radwan, Nada Ahmed and
               Elshaer, Ziad Mohamed and
               Mohamed, Ensaf Hussein",
  editor    = "Jarrar, Mustafa and
               Habash, Habash and
               El-Haj, Mo",
  booktitle = "Proceedings of the First International Workshop on Nakba Narratives as Language Resources",
  month     = jan,
  year      = "2025",
  address   = "Abu Dhabi",
  publisher = "Association for Computational Linguistics",
  url       = "https://aclanthology.org/2025.nakbanlp-1.12/",
  pages     = "114--121",
  abstract  = "Bias in news reporting significantly influences public perception, particularly in sensitive and polarized contexts like the Israel-Gaza conflict. Detecting bias in such cases presents unique challenges due to political, cultural, and ideological complexities, often amplifying disparities in reporting. While prior research has addressed media bias and dataset fairness, these approaches inadequately capture the nuanced dynamics of the Israel-Gaza conflict. To address this gap, we propose an NLP-based framework that leverages Nakba narratives as linguistic resources for bias detection in news coverage. Using a multilingual corpus focusing on Arabic texts, we apply rigorous data cleaning, pre-processing, and methods to mitigate imbalanced class distributions that could skew classification outcomes. Our study explores various approaches, including Machine Learning (ML), Deep Learning (DL), Transformer-based architectures, and generative models. The findings demonstrate promising advancements in automating bias detection, and enhancing fairness and accuracy in politically sensitive reporting."
}

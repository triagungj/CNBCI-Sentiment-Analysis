# 📊 IndoBERT-Based Sentiment Analysis on Indonesian Stock News

This repository contains the complete implementation of a sentiment analysis project using **IndoBERT** from **[IndoNLU](https://github.com/IndoNLP/indonlu)** framework. The research focuses on classifying Indonesian stock news headlines from **CNBC Indonesia** into **positive**, **neutral**, or **negative** sentiments.

---

## 📁 Repository Structure

The repository contains two main folders:

- `Dataset/`: Contains the original and split datasets (ratios 90:10, 80:20, 70:30), along with preprocessed CSV files.
- `Codes/`: Includes Jupyter notebooks for preprocessing and sentiment analysis.

---

## 📚 Overview

- **Model**: IndoBERT-Large (`indobenchmark/indobert-large-p2`)
- **Framework**: IndoNLU
- **Dataset size**: 9,819 headlines
- **Sentiment classes**: `positif`, `netral`, `negatif`
- **Data source**: CNBC Indonesia Market section (2024–2025)

This repository supports reproducible experimentation using stratified shuffle split and includes multiple learning rate scenarios and early stopping configuration.

---

## 🧪 Key Features

- ✅ Fine-tuned IndoBERT for text classification in Bahasa Indonesia
- ✅ Manual sentiment labeling on stock news headlines
- ✅ Dataset split optimization using **Jaccard Similarity**
- ✅ Four learning rate configurations (2e-5, 3e-5, 2e-6, 3e-6)
- ✅ Early stopping based training control
- ✅ Evaluation metrics: Accuracy, Precision, Recall, F1-score
- ✅ Reproducibility with random seed and controlled split

---

## 🚀 Quick Start

This project is intended to be run using **Google Colab**.

### ▶️ Open in Google Colab

You can upload this repository to your Google Drive or GitHub, then open the notebooks:

- `Codes/preprocessing.ipynb`: For cleaning and tokenizing the dataset
- `Codes/sentiment-analyzer.ipynb`: For fine-tuning IndoBERT and running evaluation

Update paths and configuration values as needed inside the scripts.

---

## 📦 Dataset Access

The full labeled dataset used in this project is available on Kaggle:  
🔗 [Kaggle Dataset: Sentiment-Labeled Stock News Headlines](https://www.kaggle.com/datasets/triagungj/cnbc-indonesia-stock-news-sentiment-dataset/data)

---

## 🙏 Acknowledgements

This research leverages:

- IndoNLU GitHub Repository: https://github.com/IndoNLP/indonlu
- **IndoBERT models and IndoNLU framework** developed by **Wilie et al. (2020)**. We deeply appreciate their work, which has been instrumental in enabling high-quality Indonesian NLP research.

  > Wilie, B., Vincentio, K., Winata, G. I., Cahyawijaya, S., et al. (2020). _IndoNLU: Benchmark and Resources for Evaluating Indonesian Natural Language Understanding_.  
  > Proceedings of AACL-IJCNLP 2020, pp. 843–857.  
  > https://doi.org/10.18653/v1/2020.aacl-main.85

- **CNBC Indonesia**, as the source of headline texts used in this study.  
  We sincerely thank CNBC Indonesia for providing access to publicly available financial news. A request for permission was submitted; however, no response was received. This work is conducted under fair use for academic research.

---

## 📚 Citation

If you use this project or dataset, please cite:
_(Hopefully soon)_

---

## ⚖️ License

MIT License – see the `LICENSE` file for details.

---

## 📬 Contact

📧 tj.triagungj@gmail.com  
Feel free to reach out for questions, collaboration, or feedback.

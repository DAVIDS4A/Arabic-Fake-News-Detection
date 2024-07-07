
<h1 align="center" style="color:#6a0dad;">📰 Arabic Fake News Classifier 📰</h1>
<p align="center" style="font-size:20px;color:#4682b4;">A comprehensive project for detecting fake news in Arabic using state-of-the-art NLP models: LSTM, BiLSTM, and BERT.</p>

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-blue.svg">
  <img src="https://img.shields.io/badge/Python-3.8-blue.svg">
  <img src="https://img.shields.io/badge/Keras-2.4.3-orange.svg">
  <img src="https://img.shields.io/badge/transformers-4.5.1-yellow.svg">
</p>

## 📑 Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Models Implemented](#models-implemented)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Comparison](#comparison)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## 📌 Project Overview
This project aims to detect fake news in Arabic using several Natural Language Processing (NLP) techniques. We have implemented and compared three different models:
1. **LSTM (Long Short-Term Memory)**
2. **BiLSTM (Bidirectional Long Short-Term Memory)**
3. **BERT (Bidirectional Encoder Representations from Transformers)**

## 🗂 Dataset
The dataset used in this project was scrapped from popular arabic news websites like:
<ul> <li> Misbar (https://misbar.com/)</li><li>No Rumors (http://norumors.net/)</li>
<li>Verify-Sy (https://verify-sy.com/)</li>
<li>Fatabyyano (https://fatabyyano.net/)</li></ul> 
It's a collection of Arabic news articles labeled as fake or real. The data preprocessing includes text cleaning, tokenization, and splitting into training and testing sets. 

## 🔍 Models Implemented
### 1. LSTM
LSTM is a type of recurrent neural network capable of learning order dependence in sequence prediction problems.

### 2. BiLSTM
BiLSTM is an extension of LSTM that improves model performance on sequence classification problems by providing additional context to the network.

### 3. BERT
BERT is a transformer-based model that has achieved state-of-the-art results in a wide range of NLP tasks.

## ⚙️ Installation
To run this project, ensure you have Python 3.8 and the required libraries installed. You can install the dependencies using:

```bash
pip install -r requirements.txt
```

## 🚀 Usage
To use the models for fake news classification, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/DAVIDS4A/Arabic-Fake-News-Detection/arabic-fake-news-classifier-lstm-bilstm-bert.git
    cd arabic-fake-news-classifier
    ```

2. Install dependencies:
    ```bash
    !pip install -r requirements.txt
    ```

3. Run the Jupyter Notebook:
    ```bash
    jupyter notebook arabic-fake-news-classifier-lstm-bilstm-bert.ipynb
    ```

4. Follow the steps in the notebook to train and evaluate the models.

## 📊 Results
The models were evaluated based on accuracy, precision, recall, and F1-score. Here are the results:

### LSTM Model
**Accuracy:** 99.59%
```plaintext
              precision    recall  f1-score   support

           0       1.00      0.99      1.00      8792
           1       0.99      1.00      1.00      8934

    accuracy                           1.00     17726
   macro avg       1.00      1.00      1.00     17726
weighted avg       1.00      1.00      1.00     17726
```

### BiLSTM Model
**Accuracy:** 98.70%
```plaintext
              precision    recall  f1-score   support

           0       0.99      0.99      0.99      8792
           1       0.99      0.99      0.99      8934

    accuracy                           0.99     17726
   macro avg       0.99      0.99      0.99     17726
weighted avg       0.99      0.99      0.99     17726
```

### AraBert Model
**Accuracy:** 96.21%
```plaintext
              precision    recall  f1-score   support

           0       0.96      0.96      0.96      8792
           1       0.96      0.96      0.96      8934

    accuracy                           0.96     17726
   macro avg       0.96      0.96      0.96     17726
weighted avg       0.96      0.96      0.96     17726
```

## 📈 Comparison
Here is a comparison of the three models based on their performance metrics:

| Model        | Accuracy | Precision | Recall | F1-Score |
|--------------|----------|-----------|--------|----------|
| LSTM         | 99.59%   | 0.99      | 0.99   | 0.99     |
| BiLSTM       | 98.70%   | 0.98      | 0.98   | 0.98     |
| AraBert      | 96.21%   | 0.96      | 0.96   | 0.96     |

The LSTM and BiLSTM models outperform Arabert model in all performance metrics, however, AraBert seems more stable based on the training accuracy and validation loss curves, demonstrating the effectiveness of transformer-based models in NLP tasks.

## 🤝 Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any improvements.

## 📄 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements
Special thanks to the contributors and the community for their support and collaboration.

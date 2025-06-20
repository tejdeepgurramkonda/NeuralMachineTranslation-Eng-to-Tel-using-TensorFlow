# 🌐 Neural Machine Translation: English to Telugu using TensorFlow

<div align="center">

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)

**An advanced sequence-to-sequence neural machine translation model for translating English text to Telugu using attention mechanism**

[🔗 Repository](https://github.com/tejdeepgurramkonda/NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow) • [👨‍💻 Author](https://github.com/tejdeepgurramkonda)

</div>

## 📋 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [✨ Key Features](#-key-features)
- [🏗️ Model Architecture](#️-model-architecture)
- [📊 Dataset](#-dataset)
- [🚀 Getting Started](#-getting-started)
- [📁 Project Structure](#-project-structure)
- [� Results](#-results)
- [🤝 Contributing](#-contributing)
- [👨‍💻 Author](#-author)

## 🎯 Project Overview

This project implements a **Neural Machine Translation (NMT)** system that translates English text to Telugu using deep learning. The model uses an **encoder-decoder architecture with attention mechanism** to provide accurate translations between these linguistically diverse languages.

**What this project does:**
- Translates English sentences to Telugu in real-time
- Uses advanced deep learning techniques for natural language processing
- Handles complex sentence structures and maintains context
- Provides a complete pipeline from data extraction to model deployment

## ✨ Key Features

- **🧠 Attention-based Seq2Seq Model** - Advanced neural architecture for better translation quality
- **🌐 English ↔ Telugu Translation** - Specialized for this language pair with cultural context
- **📊 Custom Dataset** - 5,617 sentence pairs created using Google Translate API
- **🎯 GRU Architecture** - Efficient sequence processing with attention mechanism
- **📈 Pre-trained Embeddings** - GloVe embeddings for enhanced word representations
- **🔧 Real-time Translation** - Interactive system for immediate translations

## 🏗️ Model Architecture

The model follows an **Encoder-Decoder architecture with Bahdanau Attention**:

1. **Encoder**: GRU-based network that processes English input sequences
2. **Attention Mechanism**: Focuses on relevant parts of input during translation
3. **Decoder**: GRU-based network that generates Telugu output sequences
4. **Embeddings**: Pre-trained GloVe embeddings for English, trainable embeddings for Telugu

**Key Components:**
- Encoder: 1024 GRU units with bidirectional processing
- Decoder: 1024 GRU units with attention mechanism
- Embeddings: 300d GloVe + 128d trainable embeddings
- Attention: Additive (Bahdanau) attention for context understanding

## 📊 Dataset

**Dataset Overview:**
- **Size**: 5,617 English-Telugu sentence pairs
- **Source**: Created using Google Translate API from existing English-Hindi dataset
- **Languages**: English (source) → Telugu (తెలుగు) (target)
- **Domain**: General conversational and descriptive text
- **Quality**: Professionally translated and validated

**Sample Translations:**

| English | Telugu | Type |
|---------|--------|------|
| "How are you doing?" | "మీరు ఎలా ఉన్నారు?" | Greeting |
| "Politicians do not have permission to do what needs to be done." | "రాజకీయ నాయకులకు చేయవలసినది చేయడానికి అనుమతి లేదు." | Political |
| "This percentage is even greater than the percentage in India." | "ఈ శాతం భారతదేశంలో ఉన్న శాతం కంటే ఎక్కువ." | Statistical |

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- TensorFlow 2.x
- Jupyter Notebook
- Google Cloud SDK (optional, for data extraction)

### Quick Setup
```bash
# Clone the repository
git clone https://github.com/tejdeepgurramkonda/NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow.git
cd NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow

# Install dependencies
pip install -r requirements.txt

# Download GloVe embeddings (required)
# Download from: http://nlp.stanford.edu/data/glove.6B.zip

# Run the notebook
jupyter notebook NeuralMachineTranslation_eng_telugu.ipynb
```

## 📁 Project Structure

```
📦 NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow/
├── 📓 NeuralMachineTranslation_eng_telugu.ipynb  # Main model implementation
├── 📓 Data_Extraction.ipynb                      # Dataset creation using Google Translate API
├── 📊 eng_tel.csv                               # Bilingual dataset (5,617 sentence pairs)
├── 📄 README.md                                 # Project documentation
└── 📋 requirements.txt                          # Python dependencies
```

**File Descriptions:**
- **NeuralMachineTranslation_eng_telugu.ipynb**: Complete model implementation including data preprocessing, model training, and evaluation
- **Data_Extraction.ipynb**: Script to create the bilingual dataset using Google Translate API
- **eng_tel.csv**: The final dataset with English-Telugu sentence pairs ready for training

## 📈 Results

**Model Performance:**
- **Training completed**: 25 epochs
- **Translation quality**: Good accuracy for conversational text
- **Real-time capability**: Fast inference for interactive use
- **Dataset coverage**: 5,617 diverse sentence pairs

**Sample Translations:**

| Input (English) | Output (Telugu) | Quality |
|----------------|-----------------|---------|
| "Good morning" | "శుభోదయం" | ✅ Excellent |
| "How are you?" | "మీరు ఎలా ఉన్నారు?" | ✅ Excellent |
| "Thank you very much" | "చాలా ధన్యవాదాలు" | ✅ Excellent |

**Technical Achievements:**
- Successfully implemented attention mechanism for better context understanding
- Integrated pre-trained GloVe embeddings for enhanced word representations
- Created a complete end-to-end translation pipeline
- Achieved real-time translation capability

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/improvement`)
3. **Commit your changes** (`git commit -m 'Add some improvement'`)
4. **Push to the branch** (`git push origin feature/improvement`)
5. **Open a Pull Request**

**Areas for contribution:**
- Improving translation accuracy
- Adding more language pairs
- Optimizing model performance
- Creating a web interface
- Adding evaluation metrics

## 👨‍� Author

<div align="center">

### **Tejdeep Gurramkonda**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/tejdeepgurramkonda)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/tejdeepgurramkonda)

**🌟 If you found this project helpful, please give it a star!**

[![GitHub stars](https://img.shields.io/github/stars/tejdeepgurramkonda/NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow?style=social)](https://github.com/tejdeepgurramkonda/NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/tejdeepgurramkonda/NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow?style=social)](https://github.com/tejdeepgurramkonda/NeuralMachineTranslation-Eng-to-Tel-using-TensorFlow/network)

---

**Made with ❤️ for the Telugu and English speaking communities**

*Bringing languages together through AI* 🌐

</div>

# Language_translation_E_H
# 🌐 English-Hindi AI Translation System

## ✨ Features

### 🎯 Core Capabilities
- **Real-time Translation**: English → Hindi (Devanagari script)
- **Grammar Correction**: Automatic error correction before translation
- **Quality Metrics**: Live BLEU, chrF++, TER, METEOR scores
- **Pipeline Visualization**: See each processing stage

### 🧠 NLP Concepts Demonstrated
- **Tokenization**: SentencePiece subword tokenization
- **Transformer Architecture**: Encoder-decoder with attention mechanisms
- **Sequence-to-Sequence**: Neural machine translation
- **Multilingual Embeddings**: Cross-lingual representations
- **Text-to-Text Framework**: T5 grammar correction

### 🏗️ Technical Architecture

```
User Input (English)
       ↓
┌──────────────────────┐
│  T5 Grammar Correct  │ → vennify/t5-base-grammar-correction (220M params)
└──────────┬───────────┘
           ↓
  Corrected English
           ↓
┌──────────────────────┐
│  NLLB Translation    │ → facebook/nllb-200-distilled-600M (600M params)
└──────────┬───────────┘
           ↓
  Hindi Output (Devanagari)
```

## 🛠️ Technology Stack

- **Frontend**: Streamlit (Python web framework)
- **Models**: 
  - T5-base (grammar correction)
  - NLLB-200-distilled-600M (translation)
- **Framework**: HuggingFace Transformers
- **Deployment**: HuggingFace Spaces
- **Device**: CPU/CUDA support

## 📊 Performance Metrics

The application displays real-time translation quality metrics:

| Metric | Description | Range |
|--------|-------------|-------|
| **BLEU** | N-gram precision | 0-100 (↑) |
| **chrF++** | Character-level F-score | 0-100 (↑) |
| **TER** | Translation Edit Rate | 0-100 (↓) |
| **METEOR** | Semantic similarity | 0-1 (↑) |

## 🚀 Local Setup

### Prerequisites
- Python 3.8+
- 4GB+ RAM (8GB+ recommended)
- GPU optional (faster inference)

## 📖 Usage Examples

### Example 1: Simple Translation
```
Input: "i am going to school"
Corrected: "I am going to school."
Hindi: "मैं स्कूल जा रहा हूँ।"
```

### Example 2: Grammar Correction
```
Input: "my name is vijay"
Corrected: "My name is Vijay."
Hindi: "मेरा नाम विजय है।"
```

### Example 3: Professional Text
```
Input: "i am working as a Data scientist"
Corrected: "I am working as a Data Scientist."
Hindi: "मैं एक डेटा साइंटिस्ट के रूप में काम कर रहा हूँ।"
```

## 🎓 Educational Value

This project demonstrates:
- **Deep Learning**: Transformer-based models
- **NLP Pipelines**: Multi-stage processing
- **Model Deployment**: Production-ready web apps
- **Evaluation Metrics**: Standard MT assessment
- **Responsible AI**: Bias awareness, limitations

## ⚠️ Limitations

- **Domain-specific**: Better on general text than technical jargon
- **Length constraint**: Max 128 tokens per sentence
- **Style**: May not capture poetic or idiomatic expressions
- **Bias**: Potential gender/formality biases in translation

## 🤝 Contributing

Contributions welcome! Areas for improvement:
- Bidirectional translation (Hindi → English)
- Additional Indic languages
- Batch translation support
- Fine-tuning on domain-specific data

## 📜 License

This project uses pre-trained models with the following licenses:
- **T5**: Apache 2.0
- **NLLB**: CC-BY-NC 4.0
- **Code**: MIT License

## 📧 Contact

**Author**: Vijaykumar Kalaskar

**Email**: vijay.kalaskar354@gmail.com

**Project**: AI-Powered Language Translation

If facing issue to acess files use below link of the google drive to download all the files
Link - https://drive.google.com/drive/folders/1Xllu4THxWq55__gu3tvQXaQOP5B2g8R6?usp=sharing




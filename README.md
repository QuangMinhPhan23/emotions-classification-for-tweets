# 💬 Emotion Classification in English Tweets using RNN and Transformer Models

## 🧾 Abstract  

Emotion classification in text is a critical task in **Natural Language Processing (NLP)**, with applications in **mental health monitoring**, **social media analysis**, and **human-computer interaction**.  
Despite advances in deep learning, accurately classifying nuanced emotions in short, informal texts like tweets remains challenging due to the **context-dependent nature of human emotions**.  

This project utilizes **RNN** and **Transformer-based models** with various embedding techniques to classify emotions in English Twitter messages using the **[Emotion Dataset](https://huggingface.co/datasets/dair-ai/emotion)** from Hugging Face. The dataset contains six basic emotions:  
> 😢 sadness, 😊 joy, ❤️ love, 😡 anger, 😨 fear, 😲 surprise  

We fine-tune **DistilBERT** and **ELECTRA** on the dataset, and compare their performance against traditional sequence models such as **Bidirectional RNN**, **LSTM**, and **GRU**, using **GloVe** and **BERT embeddings** with **Keras** and **BERT tokenization**.  

Our findings show that **Transformer-based models outperform recurrent models**, achieving **93% accuracy with DistilBERT** and **94% with ELECTRA** — highlighting the power of attention mechanisms for contextual emotion understanding in text.  

---

## 📊 Dataset

**Dataset:** [Emotion Dataset (Hugging Face)](https://huggingface.co/datasets/dair-ai/emotion)  
**Labels:** `sadness`, `joy`, `love`, `anger`, `fear`, `surprise`  
**Total samples:** ≈ 20,000 tweets  

**Dataset Preview:**  
<img width="1871" height="164" alt="image" src="https://github.com/user-attachments/assets/0660ece7-2825-42d3-83d1-5b39e5139466" />


---

## 🧠 Models and Methods

### 🔹 Baseline RNN Models
- **RNN, LSTM, GRU**
- **Embeddings:** GloVe / BERT  
- **Tokenization:** Keras / BERT Tokenizer  

### 🔹 Transformer Models
- **DistilBERT**
- **ELECTRA**
- Fine-tuned using the Hugging Face Transformers library.

---

## 📈 Results

**Model Performance Summary:**  
<img width="1864" height="550" alt="image" src="https://github.com/user-attachments/assets/b47eba4b-9a93-49af-a707-996b740c3ba7" />


| Model | Embedding | Accuracy | F1-Score |
|--------|------------|-----------|-----------|
| Bi-RNN | GloVe | 84% | 0.83 |
| LSTM | GloVe | 86% | 0.85 |
| GRU | GloVe | 87% | 0.86 |
| **DistilBERT** | BERT | **93%** | **0.92** |
| **ELECTRA** | BERT | **94%** | **0.93** |

**DistilBERT Classification Report:**  
<img width="920" height="591" alt="image" src="https://github.com/user-attachments/assets/36db4edc-6877-4341-9725-04c97336b3f3" />


**DistilBERT Confusion Matrix:**  
<img width="640" height="509" alt="image" src="https://github.com/user-attachments/assets/92e932ce-19ff-4e9d-88b6-93d1b2fd3d9e" />


---

## 🧪 Example Prediction

<img width="922" height="333" alt="image" src="https://github.com/user-attachments/assets/7e75143c-111f-4c77-9396-b2313aae65c3" />
<img width="1087" height="189" alt="image" src="https://github.com/user-attachments/assets/7ff4b81c-f581-41e2-ae6d-c9ab1fcc4242" />

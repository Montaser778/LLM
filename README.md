# 🏥 LLM-Based Medical Chatbot

**A Medical Chatbot powered by Large Language Models (LLMs) to provide health-related answers and guidance using advanced Natural Language Processing (NLP).**  
This is the **final AI capstone project 2025**, deployed as a **Hugging Face Space** and demonstrated with an **explanatory video**.

---

## 📌 Overview

This project showcases an **AI-powered medical chatbot** that can:
- Understand medical questions in natural language.
- Provide accurate health-related guidance.
- Leverage **Hugging Face LLM models** with fine-tuning for medical queries.

---

## 🌐 Live Demo & Video

- **Hugging Face Space:**  
  [Montaser7 / LLaMA2 Medical Chatbot](https://huggingface.co/spaces/Montaser7/llama2-medical-chatbot)

- **Demo Video on YouTube:**  
  [LLAMA2-Medical-ChatBot | Final AI Capstone Project 2025](https://www.youtube.com/watch?v=qV_msediEv0&t=9s)

---

## ❓ Example Questions

The model can answer questions like:
1. What are the symptoms of diabetes?  
2. What is high blood pressure?  
3. What are the symptoms of vitamin D deficiency?  
4. What is the difference between the flu and the common cold?  

---

## 📂 Project Structure

```
LLM/
│
├── data/                     # Medical datasets (MedQuAD, PubMedQA, etc.)
├── notebooks/                # Experiments and training notebooks
├── src/                      # Source code
│   ├── model.py               # Model building and fine-tuning
│   ├── inference.py           # Model inference and chatbot logic
│   └── utils.py
│
├── app.py                     # Streamlit or Gradio interface
├── requirements.txt           # Python dependencies
└── README.md
```

---

## 📊 Datasets

We use **Hugging Face Datasets** for medical Q&A:

1. **[MedQuAD](https://huggingface.co/datasets/medquad)** – Medical Q&A pairs from NLM websites.  
2. **[PubMedQA](https://huggingface.co/datasets/pubmed_qa)** – Biomedical Q&A for research-based insights.  
3. **[MedMCQA](https://huggingface.co/datasets/medmcqa)** – Large-scale multiple-choice medical questions.

Example loading:
```python
from datasets import load_dataset
dataset = load_dataset("medquad")
print(dataset['train'][0])
```

---

## 🛠 Installation

```bash
# Clone the repository
git clone https://github.com/Montaser778/LLM.git
cd LLM

# Install dependencies
pip install -r requirements.txt
```

**requirements.txt** should include:
```
transformers
datasets
torch
streamlit
gradio
numpy
pandas
scikit-learn
```

---

## 🚀 Usage

1. **Run the chatbot interface locally:**
```bash
python app.py
```

2. **Or run in Streamlit:**
```bash
streamlit run app.py
```

3. Ask medical questions and get AI-powered answers.

---

## ⚠️ Disclaimer

> This chatbot is for **educational purposes only**.  
> It **does not replace professional medical advice**.

---

## 👤 Author

**Montaser Hussam AbuShawish**  
*AI & Machine Learning Capstone Project 2025*  
- [Hugging Face Space](https://huggingface.co/spaces/Montaser7/llama2-medical-chatbot)  
- [YouTube Demo Video](https://www.youtube.com/watch?v=qV_msediEv0&t=9s)

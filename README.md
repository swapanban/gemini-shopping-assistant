# 🛍️ Personalized Shopping Assistant using Gemini 2.0 Flash & Gradio

This project builds a **Personalized Shopping Assistant** using **Google's Gemini 2.0 Flash Lite model** via **Vertex AI**, combined with a **Retrieval-Augmented Generation (RAG)** architecture. It recommends products based on user preferences and purchase history, using dynamic or fallback product data.

---

## 🚀 Features

- 🔎 Product search and filtering
- 🧠 RAG with Gemini Flash (`gemini-2.0-flash-lite-001`)
- 🧾 Uses Amazon product dataset (Kaggle 2023)
- 💡 Recommendations based on ratings, keywords, and category
- 🎯 Personalization using purchase history
- 📈 Evaluation metrics: `precision@k`, `ndcg@k`, feedback loop
- 🖼️ Simple Gradio UI

---

## 🛠️ Tech Stack

- **LLM**: Google Vertex AI Gemini 2.0 Flash
- **Interface**: Gradio
- **Embeddings**: Sentence Transformers
- **Vector DB**: FAISS
- **Notebook Platform**: Google Colab Pro
- **Dataset**: Kaggle Amazon Products Dataset 2023

---

## 📦 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/gemini-shopping-assistant.git
cd gemini-shopping-assistant
```

### 2. Upload Files to Colab

- Open `Gemini_Shopping_Assistant_FinalVersion.ipynb` in [Google Colab](https://colab.research.google.com/)
- Ensure GPU runtime is enabled

### 3. Set Up Vertex AI Access

- Create a service account in [Google Cloud Console](https://console.cloud.google.com/)
- Enable **Vertex AI API**
- Download service account JSON key and upload to Colab

```python
from google.colab import auth
auth.authenticate_user()

import vertexai
vertexai.init(project="your-gcp-project-id", location="us-central1")
```

---

## 📊 Evaluation Metrics

- `precision_at_k`
- `ndcg_at_k`
- Real-time user feedback collection with Gradio

---

## 📄 Python Package Requirements (Install in Colab)

```bash
pip install pandas numpy gradio faiss-cpu sentence-transformers scikit-learn google-cloud-aiplatform google-auth
```

---

## 📁 Project Structure

```
gemini-shopping-assistant/
├── Gemini_Shopping_Assistant_FinalVersion.ipynb
├── README.md
├── assets/ (screenshots/demo)
```

---

## 🧑‍💻 Author

**Swapan Banerjee**  
**Generative AI**
---

## 📸 Demo

_Add screenshots or a video link here once available._


# 📰 Fake News Detector & Generator using Generative AI & NLP

This project combines **Natural Language Processing (NLP)** with **Generative AI** to create a dual-purpose application that can **detect fake news** and **generate synthetic news text**. It leverages state-of-the-art transformer models like **GPT-2** and **RoBERTa** to showcase both sides of the fake news problem — generation and detection.

## 🚀 What This Project Does

- **Detects Fake News:** Uses a fine-tuned RoBERTa model (`hamzab/roberta-fake-news-classification`) to classify input news text as real or fake.
- **Generates News Text:** Uses GPT-2 (`gpt2-medium`) to generate realistic-sounding news based on a user-provided prompt.
- **Interactive Notebook:** Clean and interactive notebook implementation with real-time model loading, detection, and generation functionalities.

## 🧠 Key Components

### 1. **Fake News Detection**
- 🔍 **Model Used:** RoBERTa fine-tuned on fake news classification.
- 📌 **Pipeline:** `transformers.pipeline("text-classification")`
- 🧪 **Usage:** Paste any news text, and the model will classify it as **REAL** or **FAKE**.

### 2. **Fake News Generation**
- ✍️ **Model Used:** `gpt2-medium`
- ⚙️ **Pipeline:** `transformers.pipeline("text-generation")`
- 💬 **Usage:** Input a topic like *"Breaking News: Government announces"* and GPT-2 generates a realistic news story continuation.

## 💡 How it Works (Brief Overview)

- The notebook starts by installing and importing necessary libraries (`transformers`, `torch`, `pandas`).
- Models are dynamically loaded based on available GPU/CPU.
- Two separate pipelines are initialized:
  - `text_generator` for fake news generation.
  - `fake_news_detector` for classification.
- A clean interface allows users to run:
  - Custom prompts for generating news.
  - Custom news for checking authenticity.
- Results are displayed interactively using `IPython.display`.

## 🖼️ Example Outputs

### ✅ Fake News Detection
> **Input:** "COVID-19 vaccine causes magnetism in humans"  
> **Output:** FAKE

### 🧾 Fake News Generation
> **Prompt:** "Breaking News: AI revolutionizes the healthcare sector"  
> **Generated Text:** *"...hospitals around the world have begun adopting AI-driven systems..."*

## 🛠 Technologies & Libraries Used

- **Transformers** by Hugging Face
- **Torch** for GPU/CPU acceleration
- **GPT-2** for generation
- **RoBERTa** for detection
- **Pandas**, **IPyWidgets**, and **IPython.display**

## 📚 Ideal For

- NLP and AI learners exploring real-world applications
- Those studying misinformation and media manipulation
- Researchers working on adversarial NLP and robustness
- Building tools to help journalists and analysts verify content

## ⚠️ Disclaimer

This project is for **educational and research** purposes only. The generated fake news is synthetic and **must not** be used to mislead or spread misinformation.

# 🧠 Multimodal Visual Question Answering (VQA) System

A multimodal **Visual Question Answering (VQA)** system that integrates **text, voice, and image** inputs with **multilingual support**, enabling natural human–AI interaction.  
Developed as part of an **MSc dissertation**, this project demonstrates how **Large Language Models (LLMs)** and **Retrieval-Augmented Generation (RAG)** can be combined with **multimodal processing** to deliver robust, intelligent question answering.

---

## 🚀 Features

- 🗣️ **Multimodal Input:** Accepts text, voice, and image-based queries  
- 🌍 **Multilingual Support:** Handles diverse linguistic inputs across multiple languages  
- 🔊 **Audio Processing:** Integrates **Whisper** for accurate voice recognition and noise handling  
- 💡 **LLM + RAG Architecture:** Combines reasoning power of LLMs with external knowledge retrieval for context-aware answers  
- 🖥️ **Interactive Gradio UI:** Clean, accessible web interface for user interaction and testing  

---

## 🧩 System Architecture

```text
User Input (Text / Speech / Image)
          ↓
   Audio & Image Processing
          ↓
   Multimodal Fusion Layer
          ↓
   LLM + RAG Inference Engine
          ↓
   Natural Language + Visual Answer
   ```

---

## ⚙️ Tech Stack

- **Language:** Python 3.10+
- **Core Framework:** [Gradio](https://gradio.app/) (for the web UI)
- **LLM / Multimodal Models:** OpenAI / VLM-compatible models (e.g. [LLaVA](https://github.com/haotian-liu/LLaVA))
- **Speech-to-Text:** [OpenAI Whisper](https://github.com/openai/whisper) (robust to noise)
- **Retrieval / RAG:**
  - FAISS (vector index) or similar
  - Embeddings model (OpenAI / Sentence Transformers)
- **Image Processing:** [Pillow (PIL)](https://python-pillow.org/), [OpenCV](https://opencv.org/)
- **Environment:** Google Colab / Local GPU
- **Optional:** [`python-dotenv`](https://pypi.org/project/python-dotenv/) for API keys, [`torch`](https://pytorch.org/) for model inference

---

## 🧠 Example Use Cases

- **Ask visual questions about uploaded images**  
  _e.g._ “What is in this picture?”, “What colour is the car?”, “How many people are in the image?”
- **Use voice input to interact with the model in different languages**  
  _e.g._ speak in Spanish, English, Arabic, or Hindi and get a response in the same or target language
- **Retrieve contextually grounded responses from external documents via RAG**  
  _e.g._ “Based on the uploaded report, what are the main findings?” or “Summarise this image using the product manual”

---

## 📊 Results & Evaluation

The system was evaluated for:

- ✅ **Speech recognition accuracy** under varying noise conditions (microphone distance, background noise, accents)
- ✅ **Multilingual query comprehension** (tested with non-English inputs)
- ✅ **Response relevance and coherence** in multimodal contexts (image + text / speech + image)

---

## 👩‍💻 Role & Contributions

I was responsible for the **end-to-end system design and implementation**, including:

- Developing the **multilingual NLP and audio processing pipeline**
- Integrating **Whisper** for voice input and noise handling
- Building the **Gradio-based user interface** for text / voice / image inputs
- Combining **LLMs with RAG** for enhanced contextual performance
- Conducting **testing, evaluation, and documentation** of the system

- Developing the **multilingual NLP and audio processing pipeline**
- Integrating **Whisper** for voice input and noise handling
- Building the **Gradio-based user interface** for text / voice / image inputs
- Combining **LLMs with RAG** for enhanced contextual performance
- Conducting **testing, evaluation, and documentation** of the system


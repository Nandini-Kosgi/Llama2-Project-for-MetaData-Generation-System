# Llama2 Metadata Generation System

This project automates "metadata generation" from project documents (PDF, text, code) using a Retrieval-Augmented Generation (RAG) pipeline with Llama2, LangChain, FAISS, and HuggingFace**, running fully on a local CPU environment.  

---

## 🚀 Features
- Parse & extract content from multiple file formats (PDF, text, markdown, code).  
- Embed & index data with FAISS for fast similarity search.  
- RAG pipeline with Llama2 to generate accurate, context-aware metadata.  
- Streamlit interface for interactive Q&A and visualization.  
- CPU-optimized workflow for cost-efficient local development.  

---

## 🧰 Tech Stack
- Language: Python 3.10+  
- Libraries:LangChain, HuggingFace Transformers, PyTorch (CPU), Textract, Tika, Streamlit, Pandas, NumPy  
- Model: Llama2 (Quantized GGUF for CPU via `llama-cpp-python`) or HuggingFace compatible models  
- Deployment: Local machine (CPU-only)  

---

## ⚙️ Installation
```bash


# Create virtual environment
python -m venv .venv
source .venv/bin/activate   # On Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

```

**requirements.txt (sample):**
```
langchain
faiss-cpu
torch
transformers
llama-cpp-python
pypdf
textract
tika
streamlit
pandas
numpy
```

---

## 🔐 Model Setup
- Download **Llama2 GGUF quantized weights** compatible with CPU inference.  
- Update `.env` with model path:  
```env
MODEL_BACKEND=llama-cpp
MODEL_PATH=/absolute/path/to/llama-2-7b-chat.Q4_K_M.gguf
```

---

## 🗂 Project Structure
```
llama2-metadata-generation/
├── code/
│   ├── sample_files          
│   ├── main.py        
│   ├── config.py          
│   ├── streamlit_main.py  
│   └── utils.py                              
├── requirements.txt
├── README.md
└── .env
```


---

## 📊 Impact
- Reduced manual metadata documentation effort by **~70%**.  
- Achieved **<2s retrieval latency** on local CPU for medium-sized datasets.  

---

## 🔒 Privacy & Security
- All data and models run locally on CPU.  
- No external API calls; ensures full "data privacy".  

---

## 👤 Author
Nandini Kosgi 


---

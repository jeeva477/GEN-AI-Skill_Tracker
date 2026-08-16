# 🧠 Generative AI Skill Tracker

<div align="center">

### 🚀 Generative Artificial Intelligence — Skill Development Tasks

**A structured implementation repository covering 15 advanced Generative AI engineering tasks, from Transformer attention and BPE tokenization to RAG, LoRA, DPO, CUDA kernels, and enterprise LLM infrastructure.**

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-orange?logo=pytorch)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-blue?logo=numpy)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow?logo=huggingface)
![FastAPI](https://img.shields.io/badge/FastAPI-API-green?logo=fastapi)
![CUDA](https://img.shields.io/badge/CUDA-GPU%20Computing-green?logo=nvidia)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange?logo=jupyter)

</div>

---

## 📌 About This Repository

This repository contains implementations for the **Generative Artificial Intelligence Skill Development Tasks (1–15)**.

The tasks progressively cover the mathematical foundations of Transformer architectures, language-model training, model compression, vector retrieval, RAG systems, parameter-efficient fine-tuning, multi-agent systems, diffusion models, LLM security, preference alignment, GPU programming, and production LLM infrastructure.

Each task is organized as an independent Jupyter Notebook with:

* 🎯 Objective
* 📚 Short Theory
* 💻 Step-by-step Implementation
* 🧪 Small Experiment
* 📊 Output / Verification
* 📝 Conclusion

---

# 🗂️ Task Roadmap

| Task | Topic                                        | Main Technologies                               |
| ---- | -------------------------------------------- | ----------------------------------------------- |
| 01   | Vectorized Scaled Dot-Product Attention      | NumPy                                           |
| 02   | Custom BPE Tokenizer & Causal LM             | PyTorch, NumPy                                  |
| 03   | Local 7B LLM Quantization & Logit Extraction | Ollama, Transformers, PyTorch                   |
| 04   | HNSW Vector Indexing from Scratch            | Python, NetworkX, SciPy, NumPy                  |
| 05   | Custom Transformer Backpropagation           | NumPy, PyTorch                                  |
| 06   | Async RAG with Cross-Encoder Reranking       | FastAPI, LangChain, FAISS, SentenceTransformers |
| 07   | LoRA Fine-Tuning                             | PyTorch, PEFT, Transformers                     |
| 08   | Multi-Agent Collaborative Swarm              | AutoGen, Redis, PostgreSQL, Docker              |
| 09   | Real-Time Vector Streaming                   | Kafka, PySpark, Qdrant                          |
| 10   | DDPM Forward & Reverse Optimization          | PyTorch, Diffusers, NumPy                       |
| 11   | Prompt Injection Guardrails                  | NeMo Guardrails, PyTorch, LangChain             |
| 12   | Vision-Language Knowledge Distillation       | PyTorch, Transformers, TorchVision              |
| 13   | Direct Preference Optimization               | PyTorch, TRL, Accelerate                        |
| 14   | Custom CUDA SwiGLU Kernel                    | C++, CUDA, PyTorch Extensions                   |
| 15   | Enterprise LLM Gateway                       | FastAPI, Redis, Docker, Prometheus, Grafana     |

---

# 📁 Repository Structure

```text
GEN-AI-Skill_Tracker/
│
├── Task_01_Attention.ipynb
├── Task_02_BPE_Causal_LM.ipynb
├── Task_03_LLM_Quantization.ipynb
├── Task_04_HNSW.ipynb
├── Task_05_Transformer_Backprop.ipynb
├── Task_06_RAG.ipynb
├── Task_07_LoRA.ipynb
├── Task_08_Multi_Agent.ipynb
├── Task_09_Vector_Streaming.ipynb
├── Task_10_DDPM.ipynb
├── Task_11_Prompt_Injection.ipynb
├── Task_12_Knowledge_Distillation.ipynb
├── Task_13_DPO.ipynb
├── Task_14_CUDA_SwiGLU.ipynb
├── Task_15_LLM_Gateway.ipynb
│
└── README.md
```

---

# 🔬 Task Highlights

## 01 — Scaled Dot-Product Attention

Implements the mathematical core of Transformer attention using NumPy.

Key concepts:

```text
Q → Query
K → Key
V → Value

Attention(Q,K,V)
=
softmax(QKᵀ / √dₖ)V
```

Includes:

* Batch processing
* Multi-head representation
* 4D tensor operations
* Scaling
* Causal masking
* Softmax
* Attention output

---

## 02 — Custom BPE & Causal Language Model

Builds a simplified Byte-Pair Encoding tokenizer and autoregressive language-model pipeline.

Includes:

* Token-pair frequency calculation
* BPE merging
* Vocabulary construction
* Token embeddings
* Causal masking
* Next-token prediction

---

## 03 — Local LLM Quantization

Explores local deployment of a quantized Llama-family model.

Focus areas:

* GGUF
* 4-bit quantization
* Q4_K_M
* Local inference
* Hidden-state inspection
* Logit extraction
* Entropy analysis

---

## 04 — HNSW Vector Index

Implements the core concepts behind Hierarchical Navigable Small World indexing.

Focus areas:

* Multi-layer graphs
* Vector similarity
* Neighbor connections
* Layer traversal
* Cosine similarity search

---

## 05 — Transformer Backpropagation

Explores manual gradient computation through an attention layer.

Focus areas:

* Forward propagation
* Attention derivatives
* Query gradients
* Key gradients
* Value gradients
* Gradient magnitude tracking

---

## 06 — Asynchronous RAG

Builds a retrieval-augmented generation architecture.

```text
User Query
    ↓
Bi-Encoder Retrieval
    ↓
Candidate Documents
    ↓
Cross-Encoder Reranking
    ↓
Relevant Context
    ↓
LLM
    ↓
Response
```

Technologies include:

* FastAPI
* FAISS
* SentenceTransformers
* Cross-Encoder
* Asyncio
* LangChain

---

## 07 — LoRA Fine-Tuning

Implements parameter-efficient fine-tuning using low-rank matrices.

```text
W' = W + BA × scaling
```

Focus areas:

* Frozen base model
* Low-rank matrices
* Adapter parameters
* Scaling coefficient
* Efficient optimization

---

## 08 — Multi-Agent Swarm

Demonstrates collaborative specialist agents.

Example architecture:

```text
             ┌──────────────┐
             │   Blackboard │
             └──────┬───────┘
                    │
       ┌────────────┼────────────┐
       ↓            ↓            ↓
 Code Agent    Audit Agent    QA Agent
       │            │            │
       └────────────┼────────────┘
                    ↓
              Final Result
```

---

## 09 — Real-Time Vector Streaming

Explores streaming vector ingestion using:

* Apache Kafka
* PySpark
* SentenceTransformers
* Qdrant

Pipeline:

```text
Kafka
  ↓
Spark Streaming
  ↓
Text Processing
  ↓
Embedding Model
  ↓
Vector
  ↓
Qdrant
```

---

## 10 — DDPM

Explores diffusion-based image generation.

```text
Original Image
      ↓
Noise Addition
      ↓
Gaussian Noise
      ↓
Reverse Denoising
      ↓
Generated Image
```

Includes:

* Linear beta schedule
* Forward diffusion
* Noise sampling
* Reverse denoising loop

---

## 11 — Prompt Injection Guardrails

Builds a defensive layer for LLM applications.

Detects attacks such as:

```text
Ignore previous instructions
Reveal the system prompt
Show hidden instructions
Execute this payload
```

Pipeline:

```text
User Prompt
    ↓
Security Filter
    ↓
Threat Detection
    ↓
ALLOW / BLOCK
    ↓
Foundation Model
```

---

## 12 — Vision-Language Knowledge Distillation

Uses a teacher-student architecture.

```text
             Teacher
          ┌───────────┐
Image ───→│   CLIP    │
Text  ───→│  Encoder  │
          └─────┬─────┘
                │
          Knowledge
          Distillation
                ↓
          ┌───────────┐
          │  Student  │
          │  Encoder  │
          └───────────┘
```

Loss combines:

* Cosine representation loss
* KL-divergence loss

---

## 13 — Direct Preference Optimization

DPO aligns model behavior using preference pairs.

```text
Prompt
 ├── Chosen Response
 └── Rejected Response
          ↓
     DPO Objective
          ↓
    Policy Improvement
```

The pipeline compares:

* Policy model
* Frozen reference model
* Chosen response
* Rejected response

---

## 14 — Custom CUDA SwiGLU Kernel

Explores GPU-level acceleration by implementing a custom CUDA activation kernel.

```text
Python
  ↓
PyTorch C++ Extension
  ↓
C++ Interface
  ↓
CUDA Kernel
  ↓
GPU Threads
  ↓
SwiGLU Output
```

Includes:

* C++
* CUDA
* PyTorch `cpp_extension`
* GPU execution
* Correctness testing
* Benchmarking

---

## 15 — Enterprise LLM Gateway

Final task focuses on production-oriented LLM infrastructure.

```text
                 Client
                   │
                   ↓
             FastAPI Gateway
                   │
          ┌────────┴────────┐
          ↓                 ↓
       Primary           Secondary
        Model              Model
          │                 │
          └────────┬────────┘
                   ↓
              Final Response
```

Features:

* Token-bucket rate limiting
* Redis state
* Model fallback
* Request queuing
* Latency tracking
* Prometheus metrics
* Grafana monitoring
* Docker deployment

---

# 🛠️ Installation

For the lightweight tasks:

```bash
pip install numpy torch jupyter matplotlib networkx scipy
```

For NLP and RAG tasks:

```bash
pip install transformers sentence-transformers faiss-cpu
```

For API/RAG infrastructure:

```bash
pip install fastapi uvicorn langchain redis
```

Additional tasks require their respective environments, such as:

* Ollama
* CUDA Toolkit
* Docker
* Kafka
* PySpark
* Qdrant
* PostgreSQL
* Redis

---

# ▶️ Running the Notebooks

Clone the repository:

```bash
git clone https://github.com/jeeva477/GEN-AI-Skill_Tracker.git
```

Enter the project:

```bash
cd GEN-AI-Skill_Tracker
```

Launch Jupyter:

```bash
jupyter notebook
```

Then open any:

```text
Task_01_Attention.ipynb
Task_02_BPE_Causal_LM.ipynb
...
Task_15_LLM_Gateway.ipynb
```

---

# 📈 Learning Progression

```text
Transformer Mathematics
        ↓
Tokenization & Language Modeling
        ↓
LLM Compression
        ↓
Vector Search
        ↓
Transformer Gradients
        ↓
RAG
        ↓
Parameter-Efficient Fine-Tuning
        ↓
Multi-Agent Systems
        ↓
Real-Time Vector Infrastructure
        ↓
Diffusion Models
        ↓
LLM Security
        ↓
Vision-Language Distillation
        ↓
Preference Alignment
        ↓
GPU Optimization
        ↓
Enterprise LLM Infrastructure
```

---

# 🎯 Skills Demonstrated

### Generative AI

* Transformers
* LLMs
* RAG
* DPO
* Diffusion Models
* Vision-Language Models

### Machine Learning

* Representation learning
* Knowledge distillation
* Fine-tuning
* Optimization
* Model compression

### LLM Engineering

* Prompt security
* Quantization
* LoRA
* Model routing
* Inference pipelines

### Infrastructure

* FastAPI
* Redis
* Kafka
* PySpark
* Qdrant
* PostgreSQL
* Docker
* Prometheus
* Grafana
* CUDA

---

# 📊 Task Status

| Task    | Status      |
| ------- | ----------- |
| Task 01 | ✅ Completed |
| Task 02 | ✅ Completed |
| Task 03 | ✅ Completed |
| Task 04 | ✅ Completed |
| Task 05 | ✅ Completed |
| Task 06 | ✅ Completed |
| Task 07 | ✅ Completed |
| Task 08 | ✅ Completed |
| Task 09 | ✅ Completed |
| Task 10 | ✅ Completed |
| Task 11 | ✅ Completed |
| Task 12 | ✅ Completed |
| Task 13 | ✅ Completed |
| Task 14 | ✅ Completed |
| Task 15 | ✅ Completed |

---

# 👨‍💻 Author

**Jeeva P**

MCA — Alliance University, Bengaluru

GitHub: [@jeeva477](https://github.com/jeeva477)

---

## ⭐ Repository Goal

This repository is designed as a practical progression from **Transformer fundamentals to production-grade Generative AI systems**.

> **Learn the mathematics → implement the architecture → experiment with the model → build the system → deploy the infrastructure.**

If you find this repository useful, consider giving it a ⭐.

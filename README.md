# KnowledgeGraph

# 📚 Semantic Knowledge Graph from Literature

Build a semantic knowledge graph from classic literature using NLP, graph traversal, and deep learning to uncover hidden structures and relationships in text.

---

## 🚀 Project Overview

This project processes the novel *War and Peace* to:

- Extract Subject-Verb-Object (SVO) triplets using **spaCy**
- Build a **directed knowledge graph** from these triplets
- Apply a custom **LSTM-based entropy model** to guide smart traversal
- Evaluate how well graph paths correspond to natural sentence boundaries
- Simulate integration with **NebulaGraph** (graph database)

---

## 🛠️ Tech Stack

| Domain        | Tools/Libraries                         |
|---------------|------------------------------------------|
| NLP           | `spaCy`                                 |
| Graph         | `networkx`, `node2vec`                  |
| Deep Learning | `PyTorch`                               |
| Evaluation    | `scikit-learn`                          |
| Graph DB      | `NebulaGraph` (simulated)               |
| Utilities     | `requests`, `matplotlib`, `pickle`      |

---

## Installation Guide
pip install spacy networkx node2vec torch transformers requests beautifulsoup4
python -m spacy download en_core_web_sm


---

## 📌 Key Components

### 1. 📥 Data Collection
- Downloads *War and Peace* from Project Gutenberg.
- Cleans and truncates the text for demo purposes.

### 2. 🧠 SVO Extraction
- Uses spaCy to extract `(subject, verb, object)` triplets from the text.

### 3. 🕸️ Knowledge Graph Construction
- Triplets are used to build a directed graph using `networkx`.

### 4. 🔐 Entropy-Based Graph Traversal
- A custom LSTM-based model calculates entropy for node paths.
- Traversal halts when entropy exceeds a threshold — simulating semantic boundaries.

### 5. 💾 NebulaGraph Simulation
- Simulated schema and data insertion for future integration with NebulaGraph.

### 6. 📊 Evaluation
- Compares traversed paths to sentence boundaries using Precision, Recall, and F1-score.

---

## 🧪 Output
![alt text](https://raw.githubusercontent.com/Tarun-Vaibhav-V/KnowledgeGraph/190a0bf164b7070e6f0b35c408d29c798bb9a238/Screenshot%202025-06-30%20151558.png)
![alt text](https://raw.githubusercontent.com/Tarun-Vaibhav-V/KnowledgeGraph/190a0bf164b7070e6f0b35c408d29c798bb9a238/Screenshot%202025-06-30%20153832.png)
![alt text](https://github.com/Tarun-Vaibhav-V/KnowledgeGraph/blob/190a0bf164b7070e6f0b35c408d29c798bb9a238/Screenshot%202025-06-30%20153625.png?raw=true)
![alt text](https://github.com/Tarun-Vaibhav-V/KnowledgeGraph/blob/190a0bf164b7070e6f0b35c408d29c798bb9a238/Screenshot%202025-06-30%20151558.png?raw=true)

```text
📊 Evaluation Results:
 Precision: 0.72
 F1-Score:  0.84
 
Output Sentence Wise
```
## 📈 Results Summary

These are the results we obtained after evaluating our entropy-based sentence boundary detection model:

- Tested on datasets like *War and Peace* and Wikipedia samples.
- Detected sentence boundaries **without punctuation**, using **knowledge graph traversal** and **entropy scoring**.
- Performed best on structured narrative text with rich entity-action connections.
- Accuracy remained strong (F1 ≈ 0.85–0.88) across different datasets.
- Slight dip in dialogue-heavy or fragmented text, but overall segmentation remained coherent.






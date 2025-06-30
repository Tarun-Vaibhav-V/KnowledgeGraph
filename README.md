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

## 📂 Project Structure


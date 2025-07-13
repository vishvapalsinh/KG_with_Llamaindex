# 🚀 Remote Embeddings and Knowledge Graph Querying with Neo4j and LlamaIndex

A Python project that fetches data from Wikipedia, creates embeddings using remote models, builds a knowledge graph with Neo4j, and allows querying using LLMs.

---

## 📝 Description

This project demonstrates how to:

- Fetch and store data from Wikipedia.
- Generate text embeddings using remote instructor models.
- Build and persist a knowledge graph index in Neo4j.
- Query the knowledge graph using large language models.
- Visualize graph data interactively with PyVis.

Perfect for anyone exploring NLP, knowledge graphs, and graph-based question answering!

---

## ⚙️ Features

- Fetch Wikipedia articles using `WikipediaReader`.
- Generate embeddings via remote APIs with `RemoteInstructorEmbeddings`.
- Build knowledge graph indexes with LlamaIndex.
- Persist graph data into a Neo4j database.
- Query knowledge graph with natural language using LLMs.
- Visualize graph relationships interactively in HTML.

---

## 🛠️ Installation

1. Clone the repo:

```bash
git clone https://github.com/yourusername/yourrepo.git
cd yourrepo

```

1. Setup environment using `llmrag.yml` (see next section).

---

## 📦 Environment Setup

Create and activate the conda environment with all dependencies:

```bash
conda env create -f llmrag.yml
conda activate llmrag

```

Make sure you have [conda](https://docs.conda.io/en/latest/) installed.

---

## 🌟 Usage

1. Update your API keys and Neo4j credentials in the config section of the code.
2. Run the notebook or scripts to:
- Fetch Wikipedia data.
- Generate embeddings.
- Build and save knowledge graph index.
- Query the knowledge graph.
- Visualize graph data.

Example query snippet:

```python
response = query_engine.query("Tell me more about Rocket")
print(response)

```

---

## 🔍 How It Works

1. **Data Loading**: Uses `WikipediaReader` to fetch article text.
2. **Embedding Generation**: Text is sent to remote embedding services via `RemoteInstructorEmbeddings`.
3. **Knowledge Graph Construction**: The documents and embeddings build a knowledge graph stored in Neo4j.
4. **Query Engine**: A query engine is created from the graph to answer natural language queries.
5. **Visualization**: Graph data is extracted and visualized using PyVis in an interactive HTML.

---

## 🧑‍💻 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

Please ensure code style consistency and include tests if applicable.

---

## 🙏 Acknowledgments

- [LlamaIndex](https://github.com/jerryjliu/llama_index)
- [Neo4j](https://neo4j.com/)
- [PyVis](https://pyvis.readthedocs.io/en/latest/)
- Remote embedding service hosted by University of Passau

---

## 📄 License

This project is licensed under the MIT License — see the LICENSE file for details.
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

# 🔗 LangChain - Basic Components Overview

LangChain provides a modular framework to build LLM-powered applications by integrating data from different sources, transforming it, generating embeddings, and enabling semantic search using vector databases.

---

## 🚀 LangChain Core Pipeline

### 1. Data Ingestion (Loaders)

Load data from various sources:

| Loader Type     | Example Source           |
|-----------------|---------------------------|
| Text Loader     | `.txt` files              |
| PDF Loader      | `.pdf` files              |
| Web Loader      | Any Website URL           |
| Arxiv Loader    | Research Articles from Arxiv |
| Wikipedia Loader| Wikipedia Search Results  |

> Example:
```python
from langchain.document_loaders import WikipediaLoader
loader = WikipediaLoader(query="Artificial Intelligence", lang="en")
documents = loader.load()

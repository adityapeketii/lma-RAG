# RAG: Baseline vs. Cross-Encoder Re-Ranking

Compares a bi-encoder baseline with cross-encoder re-ranking for RAG over the
[Magic: The Gathering Comprehensive Rules](https://magic.wizards.com/en/rules) (effective 25 Sept 2026).

| Component | Model |
|---|---|
| Bi-encoder | `sentence-transformers/all-MiniLM-L6-v2` + FAISS (cosine) |
| Cross-encoder | `cross-encoder/ms-marco-MiniLM-L-6-v2` |
| Generator | Gemini (`gemini-3-flash-preview`) |

## Run

```bash
uv sync
# add your GEMINI_API_KEY in a .env and run
```

Open `rag_reranking.ipynb` with the `.venv` kernel and run all cells.

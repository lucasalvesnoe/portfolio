# PACK Copilot — clinical RAG that refuses to hallucinate

| | |
|---|---|
| **Client** | Medinsights |
| **Sector** | Healthcare |
| **Period** | 2026-06-06 → 2026-09-08 |
| **Commits** | 14 |
| **Languages** | TypeScript 98%, Shell 1%, HTML 1% |
| **Source code** | private repository — read access on request |

## What it is

A clinical copilot with RAG over the PACK Brasil Adulto 2025 (Practical Approach to Care Kit, Porto Alegre version). The thesis the project exists to prove is refusal: every answer shows the protocol passages that support it, with page and similarity score, and an out-of-scope question gets "not covered in PACK Brasil Adulto" instead of an invented, plausible answer. Ingestion is offline — the PDF goes through `pdftotext -layout`, loses its footer, and is sliced into ~314 chunks. The runtime has two providers, interchangeable via an environment variable: the default is lexical BM25 with extractive generation, which runs with no API key and at no cost; the alternative uses `gemini-embedding-001` dense embeddings with cosine similarity and generation by `gemini-2.5-flash`. In-memory flat-file store, with no external infrastructure. React 19 + TypeScript + Vite, with the API key isolated in a server-side Netlify Function.

## Declared dependencies

Extracted from the repository manifests.

```
@anthropic-ai/sdk · @google/genai · react · react-dom · zod
```

## Repository composition

61 versioned files, excluding dependencies and build artefacts.

| Folder | Files | Size |
|---|---|---|
| `(raiz)` | 14 | 171 KB |
| `src` | 40 | 147 KB |
| `specs` | 3 | 21 KB |
| `docs` | 1 | 8 KB |
| `scripts` | 2 | 5 KB |
| `netlify` | 1 | 1 KB |

---

[← back to index](../README.md)

# PACK Copilot — RAG clínico que se recusa a alucinar

| | |
|---|---|
| **Cliente** | Medinsights |
| **Setor** | Saúde |
| **Período** | 2026-06-06 → 2026-09-08 |
| **Commits** | 14 |
| **Linguagens** | TypeScript 98%, Shell 1%, HTML 1% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Copiloto clínico com RAG sobre o PACK Brasil Adulto 2025 (Practical Approach to Care Kit, versão Porto Alegre). A tese que o projeto existe para provar é a recusa: toda resposta exibe os trechos do protocolo que a fundamentam, com página e score de similaridade, e pergunta fora do escopo recebe "não consta no PACK Brasil Adulto" em vez de uma resposta plausível inventada. A ingestão é offline — PDF passa por `pdftotext -layout`, perde o rodapé, é fatiado em ~314 chunks. O runtime tem dois provedores intercambiáveis por variável de ambiente: o default é BM25 lexical com geração extrativa, que roda sem nenhuma chave de API e sem custo; o alternativo usa embeddings densos `gemini-embedding-001` com similaridade de cosseno e geração por `gemini-2.5-flash`. Store em arquivo plano na memória, sem infraestrutura externa. React 19 + TypeScript + Vite, com a chave de API isolada numa Netlify Function server-side.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@anthropic-ai/sdk · @google/genai · react · react-dom · zod
```

## Composição do repositório

61 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `(raiz)` | 14 | 171 KB |
| `src` | 40 | 147 KB |
| `specs` | 3 | 21 KB |
| `docs` | 1 | 8 KB |
| `scripts` | 2 | 5 KB |
| `netlify` | 1 | 1 KB |

---

[← voltar ao índice](../README.md)

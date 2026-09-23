# PubliVeo — vídeo em conteúdo multicanal

| | |
|---|---|
| **Setor** | Produto próprio e plataforma |
| **Período** | 2026-05-15 → 2026-06-12 |
| **Commits** | 230 |
| **Linguagens** | TypeScript 73%, Python 25%, CSS 2%, Mako 0% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Plataforma SaaS que transforma um vídeo gravado em conteúdo publicável nas redes do criador, sem edição manual. É o projeto com o histórico mais longo do acervo, com 230 commits. O pipeline vai de upload a transcrição, sugestão de cortes com score por trecho e geração de copy adaptada a cada canal — LinkedIn, Instagram, YouTube e blog — cada um com preview nativo do formato da plataforma e histórico de versões. Sobre o pipeline há uma camada de produto completa: autenticação Supabase, perfil com nickname, página pública por criador, sistema de créditos e checkout com Stripe. O repositório mostra prática de engenharia deliberada — specs de design versionadas antes da implementação, planos técnicos por fase, e refatoração registrada de uma página monolítica de 1005 linhas em painéis separados.

## Composição do repositório

222 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `PDF-BLOG` | 2 | 2099 KB |
| `frontend` | 113 | 1007 KB |
| `docs` | 25 | 534 KB |
| `backend` | 76 | 262 KB |
| `(raiz)` | 5 | 99 KB |
| `.github` | 1 | 0 KB |

---

[← voltar ao índice](../README.md)

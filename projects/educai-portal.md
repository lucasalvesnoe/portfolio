# EducAI — portal de capacitação de servidores

| | |
|---|---|
| **Cliente** | Setor público — capacitação de servidores |
| **Setor** | Setor público |
| **Período** | 2026-03-11 → 2026-06-16 |
| **Commits** | 101 |
| **Linguagens** | TypeScript 68%, HTML 23%, JavaScript 5%, Python 3% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Portal de capacitação para servidores públicos, e o projeto de maior volume de histórico do acervo: 101 commits. Angular standalone com Supabase, organizado em `core` (guards de rota, interceptor de autenticação, modelos, serviços) e `features` por domínio. O catálogo de cursos e trilhas é só a superfície: tem geração de conteúdo por IA, copiloto de estudo, prompt studio para o administrador ajustar os prompts sem tocar em código, emissão de certificado em PDF (jsPDF), gamificação com ranking, área de eventos, exportação para planilha, gestão de usuários, trilha de auditoria persistida e integração com HeyGen e Higgsfield para vídeo com avatar. Autenticação em dois caminhos (Supabase e Postgres direto) e cobrança via AbacatePay.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@angular/common · @angular/compiler · @angular/core · @angular/forms · @angular/platform-
browser · @angular/router · @supabase/supabase-js · cors · dotenv · express · jspdf · rxjs ·
tslib · xlsx
```

## Composição do repositório

277 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `Docs` | 29 | 12433 KB |
| `educai-backend` | 91 | 5358 KB |
| `test-screenshots` | 33 | 3182 KB |
| `public` | 6 | 1829 KB |
| `src` | 60 | 858 KB |
| `Arquitetura` | 7 | 387 KB |
| `(raiz)` | 18 | 360 KB |
| `poc-catalogo-v2` | 18 | 190 KB |
| `scripts` | 10 | 81 KB |
| `netlify` | 1 | 16 KB |
| `.vscode` | 4 | 2 KB |

---

[← voltar ao índice](../README.md)

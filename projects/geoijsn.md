# IJSN — plataforma inteligente de dados

| | |
|---|---|
| **Cliente** | IJSN — Instituto Jones dos Santos Neves / Governo do ES |
| **Setor** | Setor público |
| **Período** | 2026-02-12 → 2026-06-08 |
| **Commits** | 26 |
| **Linguagens** | HTML 84%, JavaScript 12%, CSS 3% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Plataforma de acesso a dados públicos do Espírito Santo, construída para o Instituto Jones dos Santos Neves (IJSN) e entregue como PoC para handoff ao time Azure do cliente. Reúne num só portal painéis Power BI embarcados, um assistente de IA com RAG local e fallback para o EvaGPT, e módulos analíticos próprios — o GeoIJSN, com mapa e comparativo entre municípios, e a Curadoria IA. Tem controle de acesso por papel (cliente e admin), com telas distintas por papel, e um painel administrativo que monitora uso. O repositório traz a documentação de arquitetura e a lista explícita dos pontos que precisam mudar antes de ir a produção — backend real, RAG vetorial e autenticação com JWT no lugar do mock da PoC.

## Composição do repositório

39 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `(raiz)` | 27 | 728 KB |
| `docs` | 10 | 86 KB |
| `.netlify` | 2 | 0 KB |

---

[← voltar ao índice](../README.md)

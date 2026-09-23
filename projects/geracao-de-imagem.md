# Lab de geração de imagem com identidade travada

| | |
|---|---|
| **Setor** | Agentes, infraestrutura e ferramentas |
| **Período** | 2026-09-11 → 2026-09-22 |
| **Commits** | 154 |
| **Linguagens** | Python 74%, HTML 16%, Shell 5%, CSS 3% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Laboratório de geração de imagem com identidade consistente, rodando em GPU alugada por hora — 154 commits, o segundo maior histórico do acervo. O trabalho não acontece no ComfyUI: são três telas locais próprias, uma para o elenco e a bancada de criação, uma para acompanhar a hidratação da GPU byte a byte, e uma para o mercado de GPU com o histórico das rodadas de aluguel. O problema técnico central é travar a identidade de um personagem entre gerações, que é o que separa uma imagem bonita de um personagem utilizável; o secundário é econômico — subir uma GPU sob demanda, carregar os modelos, trabalhar e derrubar antes que a hora vire custo morto. Uso interno.

## Composição do repositório

320 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `krea_bot` | 137 | 30821 KB |
| `runpod` | 60 | 1948 KB |
| `workflows-lucas` | 33 | 875 KB |
| `docs` | 25 | 790 KB |
| `(raiz)` | 16 | 309 KB |
| `pod` | 17 | 122 KB |
| `bot` | 20 | 119 KB |
| `anaconda_projects` | 1 | 32 KB |
| `graphify-out` | 9 | 25 KB |
| `workflows` | 1 | 10 KB |
| `.virtual_documents` | 1 | 2 KB |

---

[← voltar ao índice](../README.md)

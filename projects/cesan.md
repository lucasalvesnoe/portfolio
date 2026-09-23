# CESAN — troca de titularidade por WhatsApp com OCR

| | |
|---|---|
| **Cliente** | CESAN — Companhia Espírito Santense de Saneamento |
| **Setor** | Setor público |
| **Período** | 2026-05-13 → 2026-06-15 |
| **Commits** | 20 |
| **Linguagens** | HTML 58%, JavaScript 20%, Python 11%, CSS 11% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Chatbot conversacional que conduz o cliente da CESAN por todo o processo de alteração de titularidade da conta de água pelo WhatsApp, sem passar por atendimento humano no caminho comum. O cliente fotografa os documentos na própria conversa; o OCR roda em cima de visão computacional do Claude e extrai os campos direto da imagem, sem template fixo por tipo de documento. O que a IA extrai não vira decisão sozinha — cai num painel administrativo onde um operador revisa, corrige e aprova antes de efetivar. São três superfícies no mesmo backend: o chat que simula o WhatsApp, o portal do cliente e o painel de revisão. Backend em Python 3.11 com FastAPI e SQLite; o repositório versiona também PRD, changelog, cronograma e a linha do tempo da PoC.

## Composição do repositório

196 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `docs` | 28 | 22567 KB |
| `frontend` | 156 | 7449 KB |
| `backend` | 9 | 67 KB |
| `(raiz)` | 3 | 2 KB |

---

[← voltar ao índice](../README.md)

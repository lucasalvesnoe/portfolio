# Escriba — reunião gravada e transcrita no próprio Mac

| | |
|---|---|
| **Setor** | Agentes, infraestrutura e ferramentas |
| **Período** | 2026-08-10 → 2026-08-30 |
| **Commits** | 32 |
| **Linguagens** | Python 50%, Swift 21%, JavaScript 18%, CSS 8% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Grava, transcreve e resume reuniões no Mac sem bot entrando na chamada, sem driver de áudio virtual e sem áudio saindo da máquina. Funciona com qualquer coisa que faça barulho — Teams, Meet, Zoom, WhatsApp, Discord, FaceTime, vídeo no navegador — porque captura o áudio do sistema via ScreenCaptureKit, não a API de um app específico. O microfone é capturado em paralelo por uma trilha separada com AVAudioEngine, e são essas duas trilhas distintas que dão a separação de quem falou, sem diarização estatística. A transcrição roda localmente com whisper.cpp acelerado por Metal, ao vivo. No fim, o CLI do Claude gera resumo, memória e índice em Markdown. Python com componentes em Swift para as APIs nativas do macOS.

## Composição do repositório

59 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `docs` | 11 | 432 KB |
| `escriba` | 25 | 190 KB |
| `web` | 8 | 114 KB |
| `(raiz)` | 5 | 98 KB |
| `native` | 8 | 85 KB |
| `tools` | 1 | 7 KB |
| `bin` | 1 | 0 KB |

---

[← voltar ao índice](../README.md)

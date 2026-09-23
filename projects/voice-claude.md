# Claudinho — interface de voz para o Claude Code

| | |
|---|---|
| **Setor** | Agentes, infraestrutura e ferramentas |
| **Período** | 2026-06-03 → 2026-06-04 |
| **Commits** | 9 |
| **Linguagens** | Python 56%, HTML 37%, Swift 4%, Shell 3% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Interface de voz em português para o Claude Code — falar e o agente executar comando, editar arquivo e rodar script, sem perder nenhuma ferramenta pelo caminho. Na versão 1.6 o Claude Agent SDK é o cérebro único: o stream estruturado dele (texto, chamada de ferramenta, raciocínio, resultado) é renderizado limpo num terminal xterm.js, em vez de rodar um segundo processo `claude` em PTY — o que garante uma sessão só e faz o TTS ler apenas a prosa da resposta, nunca o ruído de ferramenta. Funciona sem fone de ouvido, porque o cancelamento de eco usa o `VoiceProcessingIO` do macOS, o mesmo AEC do Siri e do FaceTime. Transcrição local com whisper.cpp, TTS neural, e interface escura nativa.

## Composição do repositório

16 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `(raiz)` | 15 | 119 KB |
| `ui` | 1 | 51 KB |

---

[← voltar ao índice](../README.md)

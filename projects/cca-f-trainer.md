# CCA-F Trainer — preparatório para certificação

| | |
|---|---|
| **Setor** | Produto próprio e plataforma |
| **Período** | 2026-06-11 → 2026-06-24 |
| **Commits** | 44 |
| **Linguagens** | TypeScript 74%, Python 24%, CSS 2%, JavaScript 0% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

App de estudo para a certificação Claude Certified Architect – Foundations. Banco de 271 questões bilíngues PT-BR/EN com troca instantânea dentro do quiz, em três modos: revisão com feedback por questão, cronometrado, e simulado completo de 60 questões em 110 minutos com score escalado de 100 a 1000, igual à prova real. Cada questão tem um tutor de IA que conversa — explica por que cada alternativa errada erra e liga ao domínio — e a chave da API é do próprio usuário (BYOK), guardada só na aba do navegador e nunca no servidor. Multiusuário com login Clerk e verificação de e-mail, progresso sincronizado entre aparelhos via Upstash Redis chaveado por usuário, mais gamificação com XP, níveis, streak e conquistas.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@anthropic-ai/sdk · @supabase/ssr · @supabase/supabase-js · @upstash/ratelimit ·
@upstash/redis · @vercel/analytics · @vercel/speed-insights · canvas-confetti · lucide-react
· next · react · react-dom · zod
```

## Composição do repositório

97 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `data` | 2 | 939 KB |
| `(raiz)` | 13 | 313 KB |
| `src` | 73 | 300 KB |
| `scripts` | 7 | 90 KB |
| `docs` | 2 | 14 KB |

---

[← voltar ao índice](../README.md)

# MedInsights — copiloto clínico sobre HIS

| | |
|---|---|
| **Cliente** | SoulMV / HSCMV |
| **Setor** | Saúde |
| **Período** | 2026-04-16 → 2026-08-11 |
| **Commits** | 10 |
| **Linguagens** | TypeScript 97%, CSS 2%, JavaScript 1%, HTML 0% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

PoC do copiloto clínico demonstrada sobre a interface do SoulMV/HSCMV, sistema de gestão hospitalar. Analisa o prontuário em tempo real cruzando três fontes que normalmente ninguém lê juntas: a evolução escrita pelo médico, as anotações da enfermagem e o histórico de exames. Daí saem dois tipos de alerta — inconsistência, quando o que o médico relata contradiz o sinal vital que a enfermagem aferiu, e tendência, quando a série de exames indica piora sutil que não aparece numa leitura pontual, como lesão renal aguda em curso. Exibe o raciocínio clínico em cadeia que levou a cada conclusão, para que o médico possa discordar com base. O painel lateral empurra o conteúdo em vez de cobri-lo, e tem modo minimizado. Geração por Gemini 2.5 Pro.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@anthropic-ai/sdk · @google/genai · react · react-dom
```

---

[← voltar ao índice](../README.md)

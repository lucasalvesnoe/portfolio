# NIST 800-53 — plataforma de conformidade

| | |
|---|---|
| **Cliente** | Camata |
| **Setor** | Financeiro, jurídico e conformidade |
| **Arquivos de código** | 25 |
| **Linhas de código** | 2.948 |
| **Extensões** | `.js` ×13, `.jsx` ×8, `.sh` ×2, `.html` ×1, `.css` ×1 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

Plataforma SaaS de gestão de conformidade com o NIST 800-53, com backend e frontend separados. Organiza os controles do framework em módulos por categoria, aplica questionários interativos de diagnóstico, e consolida o resultado num dashboard de status de conformidade com análise de risco. Tem um assistente conversacional que responde perguntas sobre os controles — o ponto é que ninguém precisa ter o catálogo NIST decorado para operar a ferramenta. O repositório traz instalador, guia de início rápido e roteiro de apresentação ao cliente.

## Dependências declaradas

Extraídas do `package.json` / `requirements.txt` do projeto.

```
react · react-dom · react-router-dom · axios · lucide-react · recharts · express · mongoose
· cors · dotenv · express-rate-limit
```

## Estrutura

```
backend/
frontend/
```

---

[← voltar ao índice](../README.md)

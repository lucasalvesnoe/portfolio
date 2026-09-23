# Conciliação bancária automatizada em n8n

| | |
|---|---|
| **Setor** | Financeiro, jurídico e conformidade |
| **Arquivos de código** | 9 |
| **Linhas de código** | 1.772 |
| **Extensões** | `.js` ×6, `.html` ×2, `.sql` ×1 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

Automação de conciliação bancária em n8n, integrada ao Supabase — a versão orquestrada do mesmo problema que o KPI Gestão resolve em aplicação. Aceita extrato em CSV, XLSX, XLS, PDF e imagem, com detecção de encoding, mapeamento de coluna e OCR para os formatos que não têm texto. Faz o casamento por data e valor contra o que já está no Supabase, devolve prévia antes de confirmar e relatório final por webhook ou e-mail, com tratamento de erro em cada etapa do fluxo. Traz painel de monitoramento e bateria de testes própria.

## Dependências declaradas

Extraídas do `package.json` / `requirements.txt` do projeto.

```
axios · form-data · xlsx
```

## Estrutura

```
config/
scripts/
tests/
workflow/
```

---

[← voltar ao índice](../README.md)

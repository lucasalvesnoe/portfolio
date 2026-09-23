# AIsquad — time de agentes sobre o contexto da empresa

| | |
|---|---|
| **Setor** | Agentes, infraestrutura e ferramentas |
| **Arquivos de código** | 942 |
| **Linhas de código** | 195.443 |
| **Extensões** | `.ts` ×646, `.tsx` ×163, `.sql` ×41, `.py` ×40, `.sh` ×30 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

AIsquad — um time de agentes de IA que trabalha sobre o contexto real da empresa: as pastas de projeto, o e-mail, o Teams e o CRM. Roda inteiro na máquina, sobre o Paperclip, e conversa pelo Telegram. É o maior sistema do acervo: 942 arquivos e cerca de 195 mil linhas, sem contar o upstream vendorizado. A decisão de arquitetura que define tudo é a fronteira entre disco e agente — a coleta e a filtragem são determinísticas e não chamam modelo nenhum: scripts leem o cache local do Teams v2, o store do Mail.app e do Outlook, as reuniões e o CRM, filtram por projeto e escrevem um `digest.md` na pasta daquele projeto. Só depois um agente lê o digest, e só aí se gasta token. Tudo que acontece antes da fronteira custa zero, então todo filtro mora antes dela, nunca depois. São seis plugins de coleta (contexto local, mail local sem Azure nem Graph API, Teams local, escriba que transforma reunião gravada em issue com itens de ação, HubSpot somente-leitura, e um grafo de conhecimento sobre as pastas), mais seis módulos de trabalho determinístico — arquivista que varre evidência para fechar issue, conciliador que cruza issue aberta contra estágio do negócio, financeiro de comissão e previsão de caixa, auditor com tabela append-only de incidente e vocabulário fixo, vigia de consumo de token e tier, e auditoria dos workspaces. A interface é o Telegram com um Mini App próprio (board, ficha de agente, consumo). O repositório é publicado como molde: dado real de cliente, faturamento e as instruções dos agentes ficam fora pelo `.gitignore`, e nenhum segredo entra em arquivo — chave e token moram no Keychain do macOS, e a config guarda só o nome do item, nunca o valor. Falta de chave para o script na hora, dizendo qual, em vez de seguir com `undefined` e quebrar três funções adiante.

## Estrutura

```
arquivista/
auditor/
conciliador/
contexto/
docs/
financeiro/
intelliway-hq/
miniapp/
paperclip-plugin-contexto-local/
paperclip-plugin-escriba/
paperclip-plugin-graph/
paperclip-plugin-hubspot/
paperclip-plugin-mail-local/
paperclip-plugin-teams-local/
quota/
skills-lucas/
telegram/
tools/
tr00x-msp/
wireguard-air/
```

---

[← voltar ao índice](../README.md)

# DIRECTFUEL — abastecimento externo de frota

| | |
|---|---|
| **Cliente** | Grupo Águia Branca / VIXPAR |
| **Setor** | Transporte e logística |
| **Período** | 2026-07-28 → 2026-07-31 |
| **Commits** | 25 |
| **Linguagens** | TypeScript 92%, JavaScript 4%, Rich Text Format 2%, Shell 1% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

MVP de gestão de abastecimento externo de frota, construído para um piloto de 60 dias no Grupo Águia Branca / VIXPAR e apresentado ao cliente sob a marca DIRECTFUEL. Três perfis no mesmo fluxo: o motorista solicita pelo celular, o frentista confirma na bomba, o gestor audita no painel. Traz rule engine antifraude e evidência fotográfica obrigatória, mas a restrição que moldou a arquitetura é outra — posto de estrada não tem sinal, então a operação é offline por inteiro e sincroniza depois. Stack com Postgres em Docker Compose, Prisma para schema e seed, e autenticação por JWT com PIN para o motorista. Nenhuma senha de seed tem valor default no código: o seed falha se as variáveis de ambiente não forem preenchidas com o mínimo de comprimento exigido.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
@prisma/client · prisma · tsx
```

## Composição do repositório

112 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `docs` | 6 | 5057 KB |
| `(raiz)` | 15 | 525 KB |
| `apps` | 75 | 457 KB |
| `packages` | 8 | 33 KB |
| `prisma` | 5 | 30 KB |
| `tests` | 2 | 17 KB |
| `scripts` | 1 | 3 KB |

---

[← voltar ao índice](../README.md)

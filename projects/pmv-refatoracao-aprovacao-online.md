# PMV — refatoração do Aprovação Online

| | |
|---|---|
| **Cliente** | Prefeitura Municipal de Vitória |
| **Setor** | Setor público |
| **Período** | 2026-09-01 → 2026-09-17 |
| **Commits** | 10 |
| **Linguagens** | JavaScript 32%, C# 27%, TypeScript 20%, HTML 10% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Prova de que dá para modernizar um sistema em produção sem a reescrita de uma vez só. O alvo é o Aprovação Online da Prefeitura de Vitória: Angular 8 de 2019, rodando. O repositório contém os dois sistemas originais da PMV, a engenharia reversa completa feita sobre eles, e uma fatia reconstruída em Angular 22 que roda de verdade — lado a lado com o legado, contra o mesmo servidor. Um comando sobe os três serviços: o legado dentro de um container `node:12.13.1`, o mesmo `FROM` do Dockerfile original, para não instalar nada de 2019 na máquina de ninguém; a fatia nova; e um simulador da API com Swagger. Os dois lados gravam no mesmo arquivo de log, e é essa equivalência de requisição — não a semelhança das telas — que sustenta o argumento. A documentação numera os achados da engenharia reversa e marca, em cada um, o grau de confiança e o que ainda não se sabe.

## Composição do repositório

2733 arquivos versionados, excluídas dependências e artefatos de build.

| Pasta | Arquivos | Peso |
|---|---|---|
| `aprovacao-online-api` | 1077 | 29397 KB |
| `aprovacao-online` | 1419 | 10485 KB |
| `poc` | 209 | 6393 KB |
| `docs` | 22 | 278 KB |
| `ferramentas` | 5 | 34 KB |
| `(raiz)` | 1 | 7 KB |

---

[← voltar ao índice](../README.md)

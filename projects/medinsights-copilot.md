# medinsights-copilot

> Medinsights — copiloto clínico em extensão Chrome: análise cruzada do atendimento + ditado da evolução, no Rede Bem Estar e no Clínica nas Nuvens

| | |
|---|---|
| **Período de desenvolvimento** | 2026-06-06 → 2026-09-22 |
| **Commits** | 22 |
| **Linguagens** | TypeScript 99.0%, HTML 1.0% |
| **Volume de código** | 139 KB versionados |
| **Setor** | Saúde |
| **Código-fonte** | privado — acesso concedido sob solicitação |

## O que é

Extensão Chrome (Manifest V3) que injeta o **Medinsights**, copiloto clínico com RAG, dentro do PEP da **Rede Bem Estar (RBE)**. O widget lê o atendimento aberto, analisa adesão ao **PACK Brasil Adulto 2025** e só libera o "Registrar" depois que o médico revisa as condutas sugeridas (gate).

## Dependências declaradas

Extraído de `package.json` do repositório.

```
@vitejs/plugin-react · react · react-dom
```

## Estrutura de primeiro nível

```
dist-live/
dist-preview/
docs/
public/
src/
CHANGELOG.md
CLAUDE.md
README.md
index.html
manifest.json
package-lock.json
package.json
tsconfig.json
vite.config.ts
… e mais 1 arquivo(s) na raiz
```

---

[← voltar ao índice](../README.md)

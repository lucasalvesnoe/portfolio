# ceturb-anonimizador

> POC Anonimizador de Documentos LGPD — CETURB-ES

| | |
|---|---|
| **Período de desenvolvimento** | 2026-05-20 → 2026-05-28 |
| **Commits** | 6 |
| **Linguagens** | JavaScript 71.3%, HTML 27.1%, CSS 1.1%, Python 0.5%, Dockerfile 0.0% |
| **Volume de código** | 1405 KB versionados |
| **Setor** | Governo e setor público |
| **Código-fonte** | privado — acesso concedido sob solicitação |

## O que é

Prova de conceito para anonimização automática de dados pessoais e sensíveis (LGPD/GDPR) em documentos PDF, com identidade visual CETURB/ES.

## Dependências declaradas

Extraído de `requirements.txt` do repositório.

```
flask · flask-cors · pymupdf · anthropic · python-dotenv · gunicorn
```

## Estrutura de primeiro nível

```
ceturb/
ceturb_files/
templates/
CHANGELOG.md
Dockerfile
README.md
index.html
requirements.txt
… e mais 3 arquivo(s) na raiz
```

---

[← voltar ao índice](../README.md)

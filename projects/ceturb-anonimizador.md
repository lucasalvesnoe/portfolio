# CETURB-ES — anonimizador de PDF para LGPD

| | |
|---|---|
| **Cliente** | CETURB-ES — Companhia de Transportes Urbanos da Grande Vitória |
| **Setor** | Setor público |
| **Período** | 2026-05-20 → 2026-05-28 |
| **Commits** | 6 |
| **Linguagens** | JavaScript 71%, HTML 27%, CSS 1%, Python 0% |
| **Código-fonte** | repositório privado — acesso de leitura sob solicitação |

## O que é

Anonimizador automático de PDF para conformidade com LGPD, feito para a CETURB-ES com a identidade visual do portal original. O fluxo não é regex: o texto é extraído com PyMuPDF, enviado ao Claude com um prompt de classificação LGPD que devolve JSON com as entidades sensíveis encontradas — CPF, CNPJ, RG, e-mail, telefone, CEP, nome, endereço, dados bancários e cartão — e cada ocorrência volta ao PDF como tarja preta real via `add_redact_annot` + `apply_redactions`. Isso importa: a tarja é aplicada na camada do documento, então o texto por baixo é destruído, não apenas coberto. A resposta traz o PDF anonimizado em base64 mais a lista auditável de tudo que foi mascarado. Flask + Python 3, com login e healthcheck.

## Dependências declaradas

Extraídas dos manifestos do repositório.

```
flask · flask-cors · pymupdf · anthropic · python-dotenv · gunicorn
```

---

[← voltar ao índice](../README.md)

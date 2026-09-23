# Águia Branca — otimização de escala de motoristas

| | |
|---|---|
| **Cliente** | Viação Águia Branca |
| **Setor** | Transporte e logística |
| **Arquivos de código** | 39 |
| **Linhas de código** | 8.438 |
| **Extensões** | `.py` ×35, `.html` ×2, `.js` ×2 |
| **Código-fonte** | não versionado no GitHub — disponível sob solicitação |

## O que é

Motor de otimização de escala de motoristas e veículos para a Viação Águia Branca. O problema é de pesquisa operacional, não de CRUD: gerar escala que atenda 100% da demanda operacional respeitando as restrições de jornada da categoria. Tem camada de dados com carga real, API de demonstração, frontend próprio, modelagem de custo e empacotamento em Docker com Compose. Python, ~8,4 mil linhas.

## Dependências declaradas

Extraídas do `package.json` / `requirements.txt` do projeto.

```
fastapi · uvicorn · pydantic · pydantic-settings · ortools · pulp · scipy · numpy ·
sqlalchemy · alembic · psycopg2-binary · redis · asyncpg · pandas · openpyxl · python-
dateutil · httpx · python-multipart · python-jose · passlib · python-dotenv · reportlab ·
jinja2 · matplotlib · seaborn · celery · flower · prometheus-client · python-json-logger ·
pytest · pytest-asyncio · pytest-cov · faker · black · flake8 · mypy · pre-commit · mkdocs ·
mkdocs-material
```

## Estrutura

```
data/
docs/
examples/
frontend/
src/
```

---

[← voltar ao índice](../README.md)
